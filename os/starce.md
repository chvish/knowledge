# The magic of strace

* To start strace on a process
```
strace -fp <pid>
```

* To get a profile of a process
```
strace -c -p <pid>
```

* To filter only specific system calls
```
strace -e select,poll -p <pid>
```
