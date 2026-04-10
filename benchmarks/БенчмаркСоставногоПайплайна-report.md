> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                                           |     Mean |    StdErr |    StdDev |  Op/s | Allocated |
|--------------------------------------------------|---------:|----------:|----------:|------:|----------:|
| Retry + Circuit Breaker + Timeout                | 215.2 us |  2.125 us |  8.230 us | 4,646 |  85.84 KB |
| Retry + Circuit Breaker + Rate Limiter + Timeout | 237.2 us |  3.647 us | 14.124 us | 4,216 |  97.44 KB |
| Retry + Timeout                                  | 405.1 us | 12.855 us | 49.789 us | 2,469 |  75.63 KB |
