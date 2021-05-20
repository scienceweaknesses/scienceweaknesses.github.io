## A change-centric technique to DETECT and FIX weaknesses in configurable systems

### Abstract

Configurable systems developed in C use #ifdef directives to deal with variability and portability. Developing and evolving highly configurable systems is a complex task because developers need to deal with many configurations at the same time and weaknesses can be easily added and difficult to detect since some weaknesses belong to only a few specific configurations. This process makes the task of detecting and fixing weaknesses even more challenging because most static analysis tools are not variability-aware. In addition, to the best of our knowledge, there is a lack of studies that analyze how to automate the process of fixing weaknesses in configurable systems. We study two types of weaknesses (Null Pointer Dereference and Memory Leak) and observe a pattern used by many developers to fix them. In this work, we propose a change-centric technique to detect and fix weaknesses in configurable systems. We evaluate our proposal in 14 open projects available in the GitHub repository. To confirm the weaknesses detected and fixed, we send 12 pull requests to fix 65 Null Pointer Dereference and 5 Memory Leak. So far, experts analyzed 6 pull requests and confirmed all weaknesses reported in these patches (27 Null Pointer Dereference and 5 Memory Leak). The other pull requests are still open waiting for the developers to evaluate

### TECHNIQUE

![Drag Racing](technique.jpeg)

### PULL REQUESTS

| Project        | Status   | Weaknesses  |
|----------------|----------|------------ |
| Expat          | Accepted |             |
| Git            | Accepted |             |
| LZ4            | Accepted |             |
| Masscan        | Accepted |             |
| FreeTDS        | Accepted |             |
| MemCached      | Accepted |             |
| Nanomsg        | Open     |             |
| Dynomite       | Open     |             |
| Dial-reference | Open     |             |
| Libsmbios      | Open     |             |
| Tig            | Open     |             |
| FVWM3          | Open     |             |
| Openlldp       | Open     |             |

### COMPILATION ERRORS

| Project | File      | Compilation error                              | Status   |
|---------|-----------|------------------------------------------------|----------|
| LIbGD   | gdcache.c | First argument of 'main' should be 'int'       | Accepted |
| LIbGD   | gdcache.c | Second argument of 'main' should be char **    | Accepted |
| LIbGD   |           | Too few argument to function                   | Accepted |
| FreeTDS |           | Natural language text that should be a comment | Accepted |
| FreeTDS |           | Natural language text that should be a comment | Accepted |

### MODEL TO BUILD TEH CONFIGURABLE SYSTEMS

We create a model to compile the configurable systems using the CFLAGS and CPPFLAGS variables according to the definitions below:

##### Expat
Always enabled:

Always disabled:

##### Git
Always enabled:

Always disabled:

##### Masscan
Always enabled:

Always disabled:

##### FreeTDS
Always enabled:

Always disabled:

##### MemCached
Always enabled:

Always disabled:

##### Nanomsg
Always enabled:

Always disabled:

##### Dynomite
Always enabled:

Always disabled:

##### Dial-referenc
Always enabled:

Always disabled:

##### Libsmbios
Always enabled:

Always disabled:

##### Tig
Always enabled:

Always disabled:

##### FVWM3
Always enabled:

Always disabled:

##### Openlldp
Always enabled:

Always disabled:



