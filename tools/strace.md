---
description: The magic of strace
---

# strace

* To start strace on a process

  ```text
  strace -fp <pid>
  ```

* To get a profile of a process

  ```text
  strace -c -p <pid>
  ```

* To filter only specific system calls

  ```text
  strace -e select,poll -p <pid>
  ```

