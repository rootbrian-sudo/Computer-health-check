# Computer-health-check.
before running install
#sudo apt install python3-requests
This Python file consists of a script to check disk and cpu usage. You can see shutil and psutil modules are imported here.

The shutil module offers a number of high-level operations on files and collections of files. In particular, it provides functions that support file copying and removal. It comes under Python's standard utility modules. disk_usage() method is used to get disk usage statistics of the given path. This method returns a named tuple with the attributes total, used, and free. The total attribute represents the total amount of space, the used attribute represents the amount of used space, and the free attribute represents the amount of available space, in bytes.

psutil (Python system and process utilities) is a cross-platform library for retrieving information on the processes currently running and system utilization (CPU, memory, disks, network, sensors) in Python. It's useful mainly for system monitoring, profiling, limiting process resources, and managing running processes. cpu_percent() returns a float showing the current system-wide CPU use as a percentage. When the interval is 0.0 or None (default), the function compares process times to system CPU times elapsed since the last call, returning immediately (non-blocking). That means that the first time it's called it will return a meaningful 0.0 value. When the interval is > 0.0, the function compares process times to system CPU times elapsed before and after the interval (blocking).

This script begins with a line containing the #! character combination, which is commonly called hash bang or shebang and continues with the path to the interpreter.

#!/usr/bin/env python3 uses the operating system env command, which locates and executes Python by searching the PATH environment variable.
Requests is a Python module that you can use to send all kinds of HTTP requests. It's an easy-to-use library with a lot of features ranging from passing parameters in URLs to sending custom headers and SSL verification. You can add headers, form data, multi-part files, and parameters with simple Python dictionaries.You can then access the response data using the same request.

To use the requests module, you first need to install it. Use the following command to install the request module.