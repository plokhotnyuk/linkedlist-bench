# LinkedList Bench

Benchmarks for creation of linked lists in Java and Scala

## OpenJDK 11.0.1
```
sbt -java-home /usr/lib/jvm/openjdk-11 -no-colors clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                            (size)   Mode  Cnt          Score         Error  Units
[info] LinkedListBenchmark.javaList              1  thrpt    5  116207382.581 ±  197850.132  ops/s
[info] LinkedListBenchmark.javaList             10  thrpt    5   21295005.020 ±  192641.262  ops/s
[info] LinkedListBenchmark.javaList            100  thrpt    5    2355628.317 ±    6767.822  ops/s
[info] LinkedListBenchmark.scalaListAddOne       1  thrpt    5  217049301.066 ± 1650171.022  ops/s
[info] LinkedListBenchmark.scalaListAddOne      10  thrpt    5   32620951.821 ±  246666.870  ops/s
[info] LinkedListBenchmark.scalaListAddOne     100  thrpt    5    3429731.014 ±   16137.659  ops/s
[info] LinkedListBenchmark.scalaListPlusEq       1  thrpt    5  141254979.461 ±  345515.997  ops/s
[info] LinkedListBenchmark.scalaListPlusEq      10  thrpt    5   17388370.217 ±   23588.614  ops/s
[info] LinkedListBenchmark.scalaListPlusEq     100  thrpt    5    1737871.713 ±   18028.245  ops/s
```

## GraalVM CE 19.1.0
```
sbt -java-home /usr/lib/jvm/graalvm-ce-19 -no-colors clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                            (size)   Mode  Cnt          Score        Error  Units
[info] LinkedListBenchmark.javaList              1  thrpt    5  136128776.288 ± 401935.046  ops/s
[info] LinkedListBenchmark.javaList             10  thrpt    5   27972807.011 ± 156080.759  ops/s
[info] LinkedListBenchmark.javaList            100  thrpt    5    3134062.142 ±   3123.994  ops/s
[info] LinkedListBenchmark.scalaListAddOne       1  thrpt    5   38021472.997 ± 239313.419  ops/s
[info] LinkedListBenchmark.scalaListAddOne      10  thrpt    5    6180593.997 ±  23436.434  ops/s
[info] LinkedListBenchmark.scalaListAddOne     100  thrpt    5     701707.535 ±   2277.735  ops/s
[info] LinkedListBenchmark.scalaListPlusEq       1  thrpt    5   37923287.712 ± 115229.993  ops/s
[info] LinkedListBenchmark.scalaListPlusEq      10  thrpt    5    6026320.459 ±  30268.899  ops/s
[info] LinkedListBenchmark.scalaListPlusEq     100  thrpt    5     680228.559 ±   1209.837  ops/s
```

## GraalVM EE 19.1.0
```
sbt -java-home /usr/lib/jvm/graalvm-ee-19 -no-colors clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                            (size)   Mode  Cnt          Score        Error  Units
[info] LinkedListBenchmark.javaList              1  thrpt    5  157896297.222 ± 827162.501  ops/s
[info] LinkedListBenchmark.javaList             10  thrpt    5   30265347.922 ± 155535.146  ops/s
[info] LinkedListBenchmark.javaList            100  thrpt    5    3446605.182 ±  12733.358  ops/s
[info] LinkedListBenchmark.scalaListAddOne       1  thrpt    5   37297458.023 ± 935716.406  ops/s
[info] LinkedListBenchmark.scalaListAddOne      10  thrpt    5    6044791.828 ±   8597.697  ops/s
[info] LinkedListBenchmark.scalaListAddOne     100  thrpt    5     737495.480 ±   1199.901  ops/s
[info] LinkedListBenchmark.scalaListPlusEq       1  thrpt    5   37291784.212 ± 848327.468  ops/s
[info] LinkedListBenchmark.scalaListPlusEq      10  thrpt    5    5684613.811 ±   7260.125  ops/s
[info] LinkedListBenchmark.scalaListPlusEq     100  thrpt    5     738569.769 ±    906.034  ops/s
```
