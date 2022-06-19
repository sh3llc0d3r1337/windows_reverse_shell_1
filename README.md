# windows_reverse_shell_1
Windows Reverse Shell shellcode

Compile the shellcode.asm:

  make
  
Compile the test program:

  make test
  
The ReverseShell.cpp contains the original reverse shell.


The Cpp source
Before we can use the socket library and call any of its function, we have to call the WSAStartup function. This initializes the socket library.

We can execute cmd.exe with calling CreateProcess.

STARTF_USESHOWWINDOW is necessary to hide the command window of cmd.exe.

Streams can be redirected with specifying the STARTF_USESTDHANDLES flag and setting the hStd… members of the STARTUPINFO to the socket handle.
