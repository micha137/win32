---
Description: 'Use the Device Power programming elements to manage the way devices perform while the system is in a sleep state.'
ms.assetid: '44479f5d-2e92-4802-a633-3e0bb7d61e94'
title: Using the Device Power API
---

# Using the Device Power API

Use the Device Power programming elements to manage the way devices perform while the system is in a sleep state.

## Opening and closing the device list

Opening and closing the device list is a costly process in terms of CPU time. The [**DevicePowerOpen**](devicepoweropen.md) and [**DevicePowerClose**](devicepowerclose.md) functions that do this are only necessary if the application needs to query the device list multiple times.

If [**DevicePowerOpen**](devicepoweropen.md) is called, [**DevicePowerClose**](devicepowerclose.md) must be called when device-list queries are complete. [**DevicePowerEnumDevices**](devicepowerenumdevices.md) and [**DevicePowerSetDeviceState**](devicepowersetdevicestate.md) will not close the device list if it has been explicitly opened by **DevicePowerOpen**.

## Enumerating devices

The [**DevicePowerEnumDevices**](devicepowerenumdevices.md) function detects whether the device list is open, and if not, opens it. **DevicePowerEnumDevices** enumerates the devices based on the specified search criteria. If the device list was opened by the function, it is closed before the function returns.

## Enabling and disabling a device from waking the system

The [**DevicePowerSetDeviceState**](devicepowersetdevicestate.md) function, similar to [**DevicePowerEnumDevices**](devicepowerenumdevices.md), detects whether the device list is open, and if not, opens it. **DevicePowerSetDeviceState** then sets the specified criteria for the specified device. If the device list was opened by the function, it is closed before the function returns.

## Example Code

The following example demonstrates the use of the Device Power API.


```C++
#define _WIN32_WINNT 0x0600
#include <Windows.h>
#include <PowrProf.h>
#include <stdio.h>
#include <tchar.h>

#pragma comment(lib, "PowrProf.lib")

int __cdecl main()
{
 // Define and initialize our return variables.
 LPWSTR  pRetBuf = NULL;
 ULONG bufSize = MAX_PATH * sizeof(WCHAR);
 ULONG uIndex = 0;
 BOOLEAN bRet = FALSE;

 // Open the device list, querying all devices
 if (!DevicePowerOpen(0)) 
  {
   printf("ERROR: The device database failed to initialize.\n");
   return FALSE;
  }

 // Enumerate the device list, searching for devices that support 
 // waking from either the S1 or S2 sleep state and are currently 
 // present in the system, and not devices that have drivers 
 // installed but are not currently attached to the system, such as 
 // in a laptop docking station.

 pRetBuf = (LPWSTR)LocalAlloc(LPTR, bufSize);

 while (NULL != pRetBuf &amp;&amp; 
        0 != (bRet = DevicePowerEnumDevices(uIndex,
           DEVICEPOWER_FILTER_DEVICES_PRESENT,
           PDCAP_WAKE_FROM_S1_SUPPORTED|PDCAP_WAKE_FROM_S2_SUPPORTED,
           (PBYTE)pRetBuf,
           &amp;bufSize)))
  {
   printf("Device name: %S\n", pRetBuf);

   // For the devices we found that have support for waking from 
   // S1 and S2 sleep states, disable them from waking the system.
   bRet = (0 != DevicePowerSetDeviceState((LPCWSTR)pRetBuf, 
                                  DEVICEPOWER_CLEAR_WAKEENABLED, 
                                  NULL));

   if (0 != bRet) 
    {
     printf("Warning: Failed to set device state.\n");
    }
   uIndex++;
  }

 // Close the device list.
 DevicePowerClose();
 if (pRetBuf!= NULL) LocalFree(pRetBuf);
 pRetBuf = NULL;

 return TRUE;
}
```



In this example the device list is opened once, and closed once. If the [**DevicePowerOpen**](devicepoweropen.md) and [**DevicePowerClose**](devicepowerclose.md) functions were not called, the device list would have been opened and closed by each call to [**DevicePowerEnumDevices**](devicepowerenumdevices.md) and [**DevicePowerSetDeviceState**](devicepowersetdevicestate.md). By using **DevicePowerOpen** and **DevicePowerClose** we saved opening the device list two unnecessary times.

 

 


