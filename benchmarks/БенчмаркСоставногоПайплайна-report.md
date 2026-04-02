> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                                           |     Mean |    StdErr |    StdDev |  Op/s | Allocated |
|--------------------------------------------------|---------:|----------:|----------:|------:|----------:|
| Retry + Circuit Breaker + Timeout                | 202.3 us |  1.474 us |  5.710 us | 4,943 |  81.52 KB |
| Retry + Circuit Breaker + Rate Limiter + Timeout | 234.7 us |  1.559 us |  6.038 us | 4,262 |  92.43 KB |
| Retry + Timeout                                  | 397.2 us | 15.187 us | 58.818 us | 2,517 |  72.07 KB |
