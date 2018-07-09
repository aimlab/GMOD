# GMOD
GMOD

# Usage 

- include mallocNew.cuh file into application.
- before launching user kernels,  add my_ctor() function to initialize GMOD and launch guard kernel.
- after completing user kernels, add my_dtor() function to stop guard kernel.

## fine-grained memory management

- replace malloc and free function with mallocN and freeN function.

## fine-grained memory management

- replace cudaMalloc and cudaFree function with cudaMallocN and cudaFreeN function.

# compiling

add **-default-stream per-thread** flag to make guard kernel and user kernel  concurrently run.

