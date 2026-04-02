> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method          | Baseline |      Mean |     StdErr |     StdDev | Ratio | RatioSD |   Op/s | Allocated |
|-----------------|----------|----------:|-----------:|-----------:|------:|--------:|-------:|----------:|
| Пустой пайплайн | Yes      |  32.43 us | 2,496.2 ns | 9,667.8 ns |  1.00 |    0.00 | 30,831 |  13.05 KB |
| Fallback        | No       |  36.10 us |   625.7 ns | 2,423.5 ns |  1.20 |    0.31 | 27,698 |  18.75 KB |
| Rate Limiter    | No       |  39.41 us |   156.1 ns |   604.5 ns |  1.31 |    0.33 | 25,371 |  21.77 KB |
| Circuit Breaker | No       |  40.09 us |   119.6 ns |   463.2 ns |  1.33 |    0.34 | 24,942 |  20.48 KB |
| Bulkhead        | No       |  44.78 us |   151.7 ns |   587.4 ns |  1.49 |    0.38 | 22,333 |  24.58 KB |
| Retry           | No       |  78.63 us | 1,079.4 ns | 4,180.4 ns |  2.61 |    0.67 | 12,718 |  37.74 KB |
| Timeout         | No       | 120.73 us | 1,976.2 ns | 7,653.6 ns |  4.01 |    1.04 |  8,283 |  45.04 KB |