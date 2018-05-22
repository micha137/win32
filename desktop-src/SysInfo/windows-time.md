---
Description: 'Windows time is the number of milliseconds elapsed since the system was last started.'
ms.assetid: '95c00204-bfdf-4376-9aae-8d8139ba6750'
title: Windows Time
---

# Windows Time

*Windows time* is the number of milliseconds elapsed since the system was last started. This format exists primarily for backward compatibility with 16-bit Windows. To ensure that applications designed for 16-bit Windows continue to run successfully, the [**GetTickCount**](gettickcount.md) function returns the current Windows time.

You typically use the [**GetTickCount**](gettickcount.md) or [**GetTickCount64**](gettickcount64.md) function to compare the current Windows time with the time returned by the [**GetMessageTime**](_win32_getmessagetime_cpp) function. **GetMessageTime** returns the Windows time when the specified message was created. **GetTickCount** and **GetTickCount64** are limited to the resolution of the system timer, which is approximately 10 milliseconds to 16 milliseconds. The elapsed time retrieved by **GetTickCount** or **GetTickCount64** includes time the system spends in sleep or hibernation.

If you need a higher resolution timer, use the [**QueryUnbiasedInterruptTime**](queryunbiasedinterrupttime.md) function, a [multimedia timer](https://msdn.microsoft.com/library/windows/desktop/dd743609), or a [high-resolution timer](_win32_about_timers_cpp). The elapsed time retrieved by the **QueryUnbiasedInterruptTime** function includes only time that the system spends in the working state.

**Windows Server 2008, Windows Vista, Windows Server 2003 and Windows XP/2000:** The [**QueryUnbiasedInterruptTime**](queryunbiasedinterrupttime.md) function is available starting with Windows 7 and Windows Server 2008 R2.

You can use the System Up Time performance counter to obtain the number of seconds elapsed since the computer was started. This performance counter can be retrieved from the performance data in the registry key **HKEY\_PERFORMANCE\_DATA**. The value returned is an 8-byte value. For more information, see [Performance Counters](https://msdn.microsoft.com/library/windows/desktop/aa373083).

 

 


