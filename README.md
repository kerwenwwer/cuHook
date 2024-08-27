# CuHook support glibc 2.34+

The original cuHook has been abandoned since it used an invalid dlsym intercept call. We are now using dlvsym to fix that issue.

https://stackoverflow.com/questions/15599026/how-can-i-intercept-dlsym-calls-using-ld-preload/18825060#18825060

## Usage
```bash
# Build the sample
make

# Run the sample
LD_PRELOAD=/path/to/libcuhook.so.1 ./cuHook
```

Result will be
```
Received memory allocation callback!
Received memory de-allocation callback!
Received context destroy event!
Sample finished successfully.
```


### Support

CUDA 10, 11, 12
with glibc 2.34+

