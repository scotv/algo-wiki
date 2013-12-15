<a name="math" />
# Math
The basic extensions for Math.

|| *Call* || *Meaning* ||
|| `Math.mod(i, n): number` || returns `x`, where `i == k * n + x (x > 0)` ||
|| `Math.range(start = 0, end, step = 1): []` || gets an array of range from start to end (exclusive), with that step ||
|| `Math.randomInteger(a = 0, b): number` || gets an integer from a to b (inclusive), where a equals 0 by default ||

## Math.Stats
The basic of statistics. 

|| *Call* || *Meaning* ||
|| `max(arr): number` || gets the max number of an array ||
|| `min(arr): number` || gets the min number of an array ||
|| `sum(arr): number` || gets the sum of an array ||
|| `mean(arr): number` || gets the average of an array ||
|| `var(arr): number` || gets sample variance of an array ||
|| `stddev(arr): number` || gets the standard deviation of an array ||
|| `linearLeastSquare( X, Y, fn=(x=>x) ): [number, number]` || gets the `[a, b]`, where `fn(Y) = a fn(X) + b`. passes `Math.log` to get linear least square for `Y = c X^a` ||

[Back to top](#math)

## Math.Point
The point for the vector.

|| *Call* || *Meaning* ||
|| `new Math.Point(arr)` || builds new point by coordinates array ||

[Back to top](#math)

## Math.Vector
The vector in `n` dimension.

### Constructors and Static
|| *Call* || *Meaning* ||
|| `new Math.Vector(arr)` || builds new vector by coordinates array ||
|| `new Math.Vector(arr1, arr2)` || builds new vector by coordinates array of two point ||
|| `new Math.Vector(point1, point2)` || builds new vector by two Math.Point ||
|| `Math.Vector.norm(vec): number` || gets the length of the vec ||
|| `Math.Vector.dot(v1, v2): number` || calculates the `dot` result of two vectors ||
|| `Math.Vector.cos(v1, v2): number` || calculates the `cos` result of two vectors ||

### Members
|| `norm(): number` || gets the length of the vec itself ||
|| `dot(that): number` || calculates the `dot` result of this and that ||
|| `cos(that): number` || calculates the `cos` result of this and that ||

[Back to top](#math)