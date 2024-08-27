# CuHook support glibc 2.34+

The original cuHook has been abandoned science it use an invalid dlsym inercept call, we using dlvsym to fix that.

https://stackoverflow.com/questions/15599026/how-can-i-intercept-dlsym-calls-using-ld-preload/18825060#18825060

### Support

CUDA 10, 11, 12
with glibc 2.34+

