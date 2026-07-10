BenchmarkOneScript v0.9.0, OneScript v2.1.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                                           |     Mean |    StdErr |   StdDev |  Op/s | Allocated |
|--------------------------------------------------|---------:|----------:|---------:|------:|----------:|
| Retry + Circuit Breaker + Timeout                | 252.9 us |  2.664 us | 10.32 us | 3,954 |  95.55 KB |
| Retry + Circuit Breaker + Rate Limiter + Timeout | 299.9 us |  3.382 us | 13.10 us | 3,334 | 114.68 KB |
| Retry + Timeout                                  | 419.2 us | 16.930 us | 65.57 us | 2,386 |  75.72 KB |
