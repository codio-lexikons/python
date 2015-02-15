# Numbers
You can create numbers as follows. You would typically use them as follows

```python
number = 1000
```

where this shows the creation of an integer variable. The following table shows how you create numbers of different types. Unless you are a real maths geek, you don't need to worry about the Complex type. Integer and Float are the two you'll *need* to know.

|integer	|float|	complex|
|-|-|-|
|10|		0.0|	3.14j
|100|	15.20|	45.j
|-786|	-21.9	|9.322e-36j
|080|	32.3+e18|	.876j
|-0490|	-90.|	-.6545+0J
|-0x260	|-32.54e100|	3e+26J
|0x69 |	70.2-E12|	4.53e-7j

## Hexadecimal
Hex numbers are represented as 

```python
hexNumber = 0x12FF
```

## Number type summary

- **int** (signed integers): often called just integers or ints, are positive or negative whole numbers with no decimal point.

- **long** (long integers ): or longs, are integers of unlimited size, written like integers and followed by an uppercase or lowercase L.

- **float** (floating point real values) : or floats, represent real numbers and are written with a decimal point dividing the integer and fractional parts. Floats may also be in scientific notation, with E or e indicating the power of 10 (2.5e2 = 2.5 x 102 = 250).

- **complex** (complex numbers) : are of the form a + bJ, where a and b are floats and J (or j) represents the square root of -1 (which is an imaginary number). a is the real part of the number, and b is the imaginary part. Complex numbers are not used much in Python programming.

## Number type conversion (casting) functions
If you want to convert a number of one type to another, you use a conversion function.

```python
intNumber = 123
floatNumber = float(intNumber)
newIntNumber = int(floatNumber)
```

## Mathematical Functions
You have the following standard functions available.

### Constants
[Python Reference](https://docs.python.org/3/library/math.html#constants)

| Function | Description |
|-|-|
|math.pi|The mathematical constant π = 3.141592..., to available precision.
|math.e|The mathematical constant e = 2.718281..., to available precision.


### Number-theoretic and representation functions
[Python Reference](https://docs.python.org/3/library/math.html#number-theoretic-and-representation-functions)

| Function | Description |
|-|-|
|math.ceil(x)|Return the ceiling of x, the smallest integer greater than or equal to x. If x is not a float, delegates to x.__ceil__(), which should return an Integral value.|
|math.copysign(x, y)|Return a float with the magnitude (absolute value) of x but the sign of y. On platforms that support signed zeros, copysign(1.0, -0.0) returns -1.0.
|math.fabs(x)|Return the absolute value of x.
|math.factorial(x)|Return x factorial. Raises ValueError if x is not integral or is negative.
|math.floor(x)|Return the floor of x, the largest integer less than or equal to x. If x is not a float, delegates to x.__floor__(), which should return an Integral value.
|math.fmod(x, y)|Return fmod(x, y), as defined by the platform C library. 
|math.frexp(x)|Return the mantissa and exponent of x as the pair (m, e). m is a float and e is an integer such that x == m * 2**e exactly. If x is zero, returns (0.0, 0), otherwise 0.5 <= abs(m) < 1. This is used to “pick apart” the internal representation of a float in a portable way.
|math.fsum(iterable)|Return an accurate floating point sum of values in the iterable. 
|math.isfinite(x)|Return True if x is neither an infinity nor a NaN, and False otherwise. (Note that 0.0 is considered finite.)
|math.isinf(x)|Return True if x is a positive or negative infinity, and False otherwise.
|math.isnan(x)|Return True if x is a NaN (not a number), and False otherwise.
|math.ldexp(x, i)|Return x * (2**i). This is essentially the inverse of function frexp().
|math.modf(x)|Return the fractional and integer parts of x. Both results carry the sign of x and are floats.
|math.trunc(x)|Return the Real value x truncated to an Integral (usually an integer). Delegates to x.__trunc__().

### Power and logarithmic functions
[Python Reference](https://docs.python.org/3/library/math.html#power-and-logarithmic-functions)

| Function | Description |
|-|-|
|math.exp(x)|Return e**x.
|math.expm1(x)|Return e**x - 1. 
|math.log(x[, base])|With one argument, return the natural logarithm of x (to base e). With two arguments, return the logarithm of x to the given base, calculated as log(x)/log(base).
|math.log1p(x)|Return the natural logarithm of 1+x (base e). The result is calculated in a way which is accurate for x near zero.
|math.log2(x)|Return the base-2 logarithm of x. This is usually more accurate than log(x, 2).
|math.log10(x)|Return the base-10 logarithm of x. This is usually more accurate than log(x, 10).
|math.pow(x, y)|Return x raised to the power y. 
|math.sqrt(x)|Return the square root of x.

### Trigonometric functions
[Python Reference](https://docs.python.org/3/library/math.html#trigonometric-functions)

| Function | Description |
|-|-|
|math.acos(x)|Return the arc cosine of x, in radians.
|math.asin(x)|Return the arc sine of x, in radians.
|math.atan(x)|Return the arc tangent of x, in radians.
|math.atan2(y, x)|Return atan(y / x), in radians. The result is between -pi and pi. 
|math.cos(x)|Return the cosine of x radians.
|math.hypot(x, y)|Return the Euclidean norm, sqrt(x*x + y*y). This is the length of the vector from the origin to point (x, y).
|math.sin(x)|Return the sine of x radians.
|math.tan(x)|Return the tangent of x radians.

### Angular conversion
[Python Reference](https://docs.python.org/3/library/math.html#angular-conversion)

| Function | Description |
|-|-|
|math.degrees(x)|Converts angle x from radians to degrees.
|math.radians(x)|Converts angle x from degrees to radians.

### Hyperbolic functions
[Python Reference](https://docs.python.org/3/library/math.html#hyperbolic-functions)

| Function | Description |
|-|-|
|math.acosh(x)|Return the inverse hyperbolic cosine of x.
|math.asinh(x)|Return the inverse hyperbolic sine of x.
|math.atanh(x)|Return the inverse hyperbolic tangent of x.
|math.cosh(x)|Return the hyperbolic cosine of x.
|math.sinh(x)|Return the hyperbolic sine of x.
|math.tanh(x)|Return the hyperbolic tangent of x.

### Special functions
[Python Reference](https://docs.python.org/3/library/math.html#special-functions)

| Function | Description |
|-|-|
|math.erf(x)|Return the error function at x.
|math.erfc(x)|Return the complementary error function at x. The complementary error function is defined as 1.0 - erf(x). It is used for large values of x where a subtraction from one would cause a loss of significance.
|math.gamma(x)|Return the Gamma function at x.
|math.lgamma(x)|Return the natural logarithm of the absolute value of the Gamma function at x.

