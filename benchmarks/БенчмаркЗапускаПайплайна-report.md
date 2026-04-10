> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                       | Baseline |      Mean |   StdErr |    StdDev | Ratio | RatioSD |   Op/s | Allocated |
|------------------------------|----------|----------:|---------:|----------:|------:|--------:|-------:|----------:|
| Запуск: Действие             | Yes      |  80.16 us | 2.254 us |  8.728 us |  1.00 |    0.00 | 12,476 |  38.95 KB |
| Запуск: Лямбда               | No       | 212.95 us | 1.385 us |  5.364 us |  2.68 |    0.25 |  4,696 |  81.81 KB |
| Асинхронный запуск: Действие | No       | 230.93 us | 2.763 us | 10.700 us |  2.91 |    0.29 |  4,330 |  78.66 KB |
| Асинхронный запуск: Лямбда   | No       | 399.80 us | 3.681 us | 14.257 us |  5.04 |    0.49 |  2,501 | 121.62 KB |
