# learn-css-secret
Record some beautiful and interesting css style tips.

## Some Note
- use css to implement effect instead of image can reduce Http request.
- some css effects are partially supported,we need to consider graceful degradation.
- if some css effects need much code to implement and are not DIY,please use mixin to improve code reuse.
- Fitts’ Law: T = a + b log2(D/W+1).
```
T = length of time required for moving device;
a, b is the empirical constant;
D = the distance from the start of the device to the target position;
W = the width of the target.
```