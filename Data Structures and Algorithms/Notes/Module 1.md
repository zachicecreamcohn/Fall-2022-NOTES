# Module 1

## 2.1 Algorithm efficiency
- <u>Algorithm efficiency</u>
  - Typically measured by algorithm's <u>Computational Complexity</u>
- <u>Computational Complexity</u>
  - The amount of resources used by the algorithm
    - Common resources
      - Runtime
      - Memory usage
      - Network communication
- <u>Runtime Complexity</u>
  - a function, `T(N)`, that represents the number of constant time operations performed by algorithm on an input of size `N`
  - Algorithm's <u>Best Case</u>
    - The scenario where the algorithm does the _minimum possible number of operations_
  - Algorithm's <u>Worst Case</u>
    - The scenario where the algorithm does the _maximum possible number of operations_
- <u>Space Complexity</u>
  - a function, `S(N)`, that represents the number of fixed-size memory units used by algorithm for an input of size `N`
  - _example_
    - _The space complexity of an algorithm that duplicates a list of numbers is `S(N) = 2N + k`, where `k` is a constant representing memory used for things like the loop counter and list pointers_
  - Algorithm's <u>Auxiliary Space Complexity</u> is the space complexity _not including the input data_
    - _example_
      - _An algorithm to find the max number in a list will have space complexity of `S(N) = N + k`, but an auxiliary space complexity of `S(N) = k`, where k is a constant

## 2.2 Constant time operations
- <u>Constant Time Operation</u>
  - An operation that, for a given processor, always operates in the same amount of time, regardless of input values
  - Used to consider runtime without discussing nanoseconds (nanoseconds can change based on the speed of the processor)
  - _examples_
    - _A CPU multiplies values `10` and `20` at the same speed as `1000` and `2000`. Multiplication of fixed-size integers is a constant-time operations_
    - _A loop that iterates `x` number of times is not constant time since it can take longer if the loop iterates over a larger set of values_
    - _A loop with a constant number of iterations (e.x. `10`) can be a constant time operation.
    - _String concatenation is not constant time since more characters must be copied for larger strings, taking longer_

### Common constant time operations
| Operation                                                                                          | Example                                                    |
|----------------------------------------------------------------------------------------------------|------------------------------------------------------------|
| Addition, subtraction, multiplication, and division of fixed size integer or floating point values | `w = 10.4`<br>`x = 3.4`<br>`y = 2.0`<br>`z = (w - x) / y`  |
| Assignment of a reference, pointer, or other fixed size data value                                 | `x = 1000`<br>`y = x`<br>`a = true`<br>`b = a`             |
| Comparison of two fixed size data values                                                           | `a = 100`<br>`b = 200`<br>`if (b > a) {`<br>`...`<br>`}`   |
| Read or write an array element at a particular index                                               | `x = arr[index]`<br>`arr[index + 1] = x + 1`               |


## 2.3 Growth of functions and complexity

### Upper and Lower Bounds
- An algorithm with runtime complexity `T(N)` has a lower bound and an upper bound
- <u>Lower Bound</u>
  - A function `f(N)` that is <= the best case `T(N)`, for all values N >= 1
- <u>Upper Bound</u>
  - A function `f(N)` that is >= the worst case `T(N)`, for all values N >= 1

### Growth rates and asymptotic notations
- <u>O notation</u>
  - provides a growth rate for an algorithm's upper bound.
- <u>Ω notation</u>
  - provides a growth rate for an algorithm's lower bound.
- <u>Θ notation</u>
  - provides a growth rate that is both an upper and lower bound.

### Notations for algorithm complexity analysis
| Notation | General Form    | Meaning                                                                      |
|----------|-----------------|------------------------------------------------------------------------------|
| O        | T(N) = O(f(N))  | a positive constant `c` exists such that, for all N >= 1, T(N) <= `c` * f(N) |
| Ω        | T(N) = Ω(f(N))  | a positive constant `c` exists such that, for all N >= 1, T(N) >= `c` * f(N) |
| Θ        | T(N) = Θ(f(N))  | T(N) = O(f(N)) and T(N) = Ω(f(N))                                            |

## 2.4 Algorithm analysis
### Worst-case algorithm analysis
- <u>Worst-case runtime</u>
  - The runtime complexity for an input that results in the longest execution.

## 2.5 O notation
### Rules for determining Big O notation of composite functions
| Composite Function | Big O notation |
|--------------------|----------------|
| c * O(f(N))        | O(f(N))        |
| c + O(f(N))        | O(f(N))        |
| g(N) * O(f(N))     | O(g(N) * f(N)) |
| g(N) + O(f(N))     | O(g(N) + f(N)) |

1