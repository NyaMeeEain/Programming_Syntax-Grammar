# Win32 API With C Programming
Any Windows programming should have  a main entry point. WinMain() function is the entry point of windows API which is called by the system as the initial entry point for a Win32-based application.

###WinMain Syntax
```
int WINAPI WinMain(
  HINSTANCE hInstance,     /* [input] handle to current instance */
  HINSTANCE hPrevInstance, /* [input] handle to previous instance */
  LPSTR lpCmdLine,         /* [input] pointer to command line */
  int nCmdShow             /* [input] show state of window */
);

```
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
