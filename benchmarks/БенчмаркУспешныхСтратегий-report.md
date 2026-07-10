BenchmarkOneScript v0.9.0, OneScript v2.1.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method          | Baseline |      Mean |     StdErr |     StdDev | Ratio | RatioSD |   Op/s | Allocated |
|-----------------|----------|----------:|-----------:|-----------:|------:|--------:|-------:|----------:|
| Пустой пайплайн | Yes      |  35.04 us |   778.8 ns | 3,016.1 ns |  1.00 |    0.00 | 28,536 |  13.57 KB |
| Fallback        | No       |  42.99 us |   136.0 ns |   526.7 ns |  1.24 |    0.12 | 23,260 |  21.20 KB |
| Rate Limiter    | No       |  59.12 us |   440.8 ns | 1,707.2 ns |  1.70 |    0.17 | 16,915 |  30.51 KB |
| Circuit Breaker | No       |  72.65 us |   199.8 ns |   773.8 ns |  2.09 |    0.21 | 13,764 |  31.34 KB |
| Retry           | No       |  77.50 us |   388.5 ns | 1,504.8 ns |  2.23 |    0.22 | 12,904 |  39.13 KB |
| Bulkhead        | No       |  90.24 us |   239.4 ns |   927.3 ns |  2.60 |    0.26 | 11,081 |  35.65 KB |
| Timeout         | No       | 132.66 us | 1,430.6 ns | 5,540.6 ns |  3.82 |    0.40 |  7,538 |  47.87 KB |
