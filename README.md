# LinkedList Bench

Benchmarks for creation of linked lists in Java and Scala

## OpenJDK 11.0.1 + Scala 2.13.0
```
sbt -java-home /usr/lib/jvm/openjdk-11 -no-colors ++2.13.0! clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                                (size)   Mode  Cnt          Score        Error  Units
[info] LinkedListBenchmark.javaListOfBooleans        1  thrpt    5  115964833.994 ± 639176.541  ops/s
[info] LinkedListBenchmark.javaListOfBooleans       10  thrpt    5   21369838.875 ±  37165.116  ops/s
[info] LinkedListBenchmark.javaListOfBooleans      100  thrpt    5    2356905.688 ±   3751.665  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans       1  thrpt    5  141307886.627 ± 528269.675  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans      10  thrpt    5   17389859.809 ±  56264.840  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans     100  thrpt    5    1739506.407 ±   6290.083  ops/s
```

## OpenJDK 11.0.1 + Scala 2.12.8
```
sbt -java-home /usr/lib/jvm/openjdk-11 -no-colors ++2.12.8! clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                                (size)   Mode  Cnt          Score         Error  Units
[info] LinkedListBenchmark.javaListOfBooleans        1  thrpt    5  116268500.122 ±  229868.288  ops/s
[info] LinkedListBenchmark.javaListOfBooleans       10  thrpt    5   21320881.892 ±   86340.034  ops/s
[info] LinkedListBenchmark.javaListOfBooleans      100  thrpt    5    2356684.128 ±    5464.050  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans       1  thrpt    5  217337686.185 ± 1106176.949  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans      10  thrpt    5   23973040.911 ±   96581.869  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans     100  thrpt    5    1955847.520 ±    7049.663  ops/s
```

## OpenJDK 11.0.1 + Scala 2.11.12
```
sbt -java-home /usr/lib/jvm/openjdk-11 -no-colors ++2.11.12! clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                                (size)   Mode  Cnt          Score        Error  Units
[info] LinkedListBenchmark.javaListOfBooleans        1  thrpt    5  116301240.826 ± 261179.954  ops/s
[info] LinkedListBenchmark.javaListOfBooleans       10  thrpt    5   21358627.038 ±  34014.497  ops/s
[info] LinkedListBenchmark.javaListOfBooleans      100  thrpt    5    2356476.562 ±   7604.223  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans       1  thrpt    5  184808032.564 ± 333719.844  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans      10  thrpt    5   17463601.690 ± 165511.007  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans     100  thrpt    5    2510096.965 ±  10260.141  ops/s
```

## GraalVM CE 19.1.0 + Scala 2.13.0
```
sbt -java-home /usr/lib/jvm/graalvm-ce-19 -no-colors ++2.13.0! clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                                (size)   Mode  Cnt          Score         Error  Units
[info] LinkedListBenchmark.javaListOfBooleans        1  thrpt    5  136740329.223 ±  328022.258  ops/s
[info] LinkedListBenchmark.javaListOfBooleans       10  thrpt    5   28039602.026 ±   91503.686  ops/s
[info] LinkedListBenchmark.javaListOfBooleans      100  thrpt    5    3141197.916 ±   10653.924  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans       1  thrpt    5   37580954.666 ± 3821572.767  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans      10  thrpt    5    6151102.268 ±   10186.068  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans     100  thrpt    5     686512.459 ±    3835.357  ops/s
```

## GraalVM CE 19.1.0 + Scala 2.12.8
```
sbt -java-home /usr/lib/jvm/graalvm-ce-19 -no-colors ++2.12.8! clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                                (size)   Mode  Cnt          Score        Error  Units
[info] LinkedListBenchmark.javaListOfBooleans        1  thrpt    5  137054509.968 ± 186986.294  ops/s
[info] LinkedListBenchmark.javaListOfBooleans       10  thrpt    5   28093012.787 ±  39659.809  ops/s
[info] LinkedListBenchmark.javaListOfBooleans      100  thrpt    5    3149120.773 ±  10792.567  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans       1  thrpt    5  238798855.781 ± 422758.748  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans      10  thrpt    5   30969607.972 ± 159296.508  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans     100  thrpt    5    2960262.075 ±   8304.218  ops/s
```

## GraalVM CE 19.1.0 + Scala 2.11.12
```
sbt -java-home /usr/lib/jvm/graalvm-ce-19 -no-colors ++2.11.12! clean 'bench/jmh:run LinkedListBenchmark'
...
[info] REMEMBER: The numbers below are just data. To gain reusable insights, you need to follow up on
[info] why the numbers are the way they are. Use profilers (see -prof, -lprof), design factorial
[info] experiments, perform baseline and negative tests that provide experimental control, make sure
[info] the benchmarking environment is safe on JVM/OS/HW level, ask for reviews from the domain experts.
[info] Do not assume the numbers tell you what you want them to tell.
[info] Benchmark                                (size)   Mode  Cnt          Score         Error  Units
[info] LinkedListBenchmark.javaListOfBooleans        1  thrpt    5  136586394.396 ±  631996.755  ops/s
[info] LinkedListBenchmark.javaListOfBooleans       10  thrpt    5   27967059.830 ±  165596.117  ops/s
[info] LinkedListBenchmark.javaListOfBooleans      100  thrpt    5    3139565.454 ±    6639.934  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans       1  thrpt    5  232773825.074 ± 1095799.042  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans      10  thrpt    5   30824629.685 ±   61961.937  ops/s
[info] LinkedListBenchmark.scalaListOfBooleans     100  thrpt    5    3188630.918 ±   15823.874  ops/s
```
 