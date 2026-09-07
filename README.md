# kernel

A kernel is only faster if the server got faster. Kernel measures that.

You edit a Triton kernel that already lives in vLLM, same function signature, and then run one command. We compare your version to the last previous (i.e. latest committed in vLLM) version.  


Simple cmd: 

```
kernel bench my_kernel.py
```

  
What you get:

- Did the new kernel match the old one? If not: `INVALID`.
- How fast is the kernel by itself?
- How fast is vLLM with it in?
- Final answer for the server: `IMPROVED` / `REGRESSED` / `EQUIVALENT` / `INCONCLUSIVE` / `INVALID`.

