> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method          | Baseline |      Mean |      StdErr |     StdDev | Ratio | RatioSD |   Op/s | Allocated |
|-----------------|----------|----------:|------------:|-----------:|------:|--------:|-------:|----------:|
| Пустой пайплайн | Yes      |  33.26 us | 1,511.10 ns | 5,852.5 ns |  1.00 |    0.00 | 30,063 |  13.57 KB |
| Fallback        | No       |  35.68 us |    99.77 ns |   386.4 ns |  1.11 |    0.21 | 28,023 |  19.96 KB |
| Rate Limiter    | No       |  41.38 us |   310.10 ns | 1,201.0 ns |  1.28 |    0.24 | 24,168 |  22.98 KB |
| Circuit Breaker | No       |  41.62 us |   267.25 ns | 1,035.1 ns |  1.29 |    0.25 | 24,027 |  21.70 KB |
| Bulkhead        | No       |  48.60 us |   356.49 ns | 1,380.7 ns |  1.51 |    0.29 | 20,577 |  26.98 KB |
| Retry           | No       |  76.86 us |   334.27 ns | 1,294.6 ns |  2.39 |    0.45 | 13,011 |  38.95 KB |
| Timeout         | No       | 132.74 us | 2,335.39 ns | 9,044.9 ns |  4.12 |    0.82 |  7,534 |  47.98 KB |
