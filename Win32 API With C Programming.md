# Win32 API With C Programming
Any Windows programming should have  a main entry point. WinMain() function is the entry point of windows API which is called by the system as the initial entry point for a Win32-based application.

### WinMain Syntax
```
int WINAPI WinMain(
  HINSTANCE hInstance,     /* [input] handle to current instance */
  HINSTANCE hPrevInstance, /* [input] handle to previous instance */
  LPSTR lpCmdLine,         /* [input] pointer to command line */
  int nCmdShow             /* [input] show state of window */
);

```
### Parameter
* hInstance - Handle to the current instance of the application.
* hPrevInstance - Handle to the previous instance of the application. For a Win32-based application, **this parameter always must be NULL**
* lpCmdLine - Pointer to a null-terminated string specifying the command line for the application, excluding the program name. To retrieve the entire command line, use the GetCommandLine() function.
* nCmdShow - Specifies how the window is to be shown


### for example
```
#include <windows.h>

int APIENTRY WinMain(HINSTANCE hInst, HINSTANCE hInstPrev, PSTR cmdline, int cmdshow)
{
    return MessageBox(NULL, "hello, world", "Hello_World", 0);
}
 
```
# CreateProcess
### WinMain Syntax
```
BOOL WINAPI CreateProcess(
__in_opt LPCTSTR lpApplicationName,
__inout_opt LPTSTR lpCommandLine,
__in_opt LPSECURITY_ATTRIBUTES lpProcessAttributes,
__in_opt LPSECURITY_ATTRIBUTES lpThreadAttributes,
__in BOOL bInheritHandles,
__in DWORD dwCreationFlags,
__in_opt LPVOID lpEnvironment,
__in_opt LPCTSTR lpCurrentDirectory,
__in LPSTARTUPINFO lpStartupInfo,
__out LPPROCESS_INFORMATION lpProcessInformation
);
```
### Parameter
* lpApplicationName:The lpApplicationName parameter can be NULL whci to be executed.
* lpCommandLine: The command line to be executed.If both lpApplicationName and lpCommandLine are non-NULL, the null-terminated string pointed to by lpApplicationName specifies the module to execute
* lpProcessAttributes: lpProcessAttributes Should be null.
* bInheritHandles:If this parameter TRUE, each inheritable handle in the calling process is inherited by the new process. If the parameter is FALSE, the handles are not inherited. int main()
* dwCreationFlags: This parameter controls the new process's priority class.
* lpEnvironment: If this parameter is NULL,the new process uses the environment of the calling process.
* lpCurrentDirectory: lpCurrentDirectory should be 0.
* lpStartupInfo:lpStartupInfo Value always must be si.
* lpProcessInformation: lpProcessInformation always must be pi.

### for example
```
#include <Windows.h>

int main()
{

	BOOL success =CreateProcess(NULL, "cmd /C powershell.exe -ep bypass", NULL, NULL, 0, 0, NULL, NULL, &si, &pi))
}

```
### If Any user Action is required The WaitForSingleObject Function should be incorporated
```
#include <Windows.h>

int main()
{

	BOOL success =CreateProcess(NULL, "cmd /C powershell.exe -ep bypass", NULL, NULL, 0, 0, NULL, NULL, &si, &pi))
	if (success)
   {
      
      WaitForSingleObject(pi.hProcess, INFINITE);

      // Process has exited - check its exit code
      DWORD exitCode;
      GetExitCodeProcess(pi.hProcess, &exitCode);

      

     
      CloseHandle(pi.hThread);
      CloseHandle(pi.hProcess);
   }
}
```
