# BUG_NET_01 — Infinite Loading Spinner When Saving Attendance in Offline Network Condition

## Summary
When a teacher attempts to save student attendance while the network is offline, the system enters an infinite loading state with no error message or recovery option.

## Environment
- Application: HyGo College Portal  
- Module: Attendance  
- User Role: Teacher  
- Browser: Chrome 144.0.7559.60  
- Operating System: Windows 10  
- Network Condition: Offline (Chrome DevTools → Network → Offline)  

## Preconditions
- Teacher account exists and is logged in successfully.  
- Teacher has access to the Attendance module.  
- Student list is available for marking attendance.  
- Network condition is set to **Offline** using Chrome DevTools.  

## Steps to Reproduce
1. Log in as a Teacher.
2. Navigate to the **Attendance** module.
3. Mark attendance for one or more students.
4.  Open Chrome DevTools and navigate to the **Network** tab.
5.  Set the network condition to **Offline**.
6.  Click **Save Attendance**.  

## Expected Result
- The system should display a clear error message such as:  
  > *"Network unavailable. Please check your connection and try again."*  
- The loading spinner should stop.   

## Actual Result
- The system shows an infinite loading spinner.  
- No error message is displayed.  

## Impact
- Blocks a core academic workflow (attendance submission).  
- High likelihood in real-world low-network environments.  
- Causes poor user experience and potential uncertainty about whether data was saved.  

## Severity
Major  

## Priority
High  

## Evidence
- Video: Loom recording of reproduction steps - https://www.loom.com/share/e7b04d0ae41b4d6e9dc01af41eba419f

