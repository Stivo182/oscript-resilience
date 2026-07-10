BenchmarkOneScript v0.9.0, OneScript v2.1.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                       | Baseline |      Mean |     StdErr |    StdDev | Ratio | RatioSD |   Op/s | Allocated |
|------------------------------|----------|----------:|-----------:|----------:|------:|--------:|-------:|----------:|
| Запуск: Действие             | Yes      |  80.30 us | 1,802.4 ns |  6.981 us |  1.00 |    0.00 | 12,453 |  39.13 KB |
| Запуск: Лямбда               | No       | 215.20 us |   645.7 ns |  2.501 us |  2.70 |    0.20 |  4,647 |  81.56 KB |
| Асинхронный запуск: Действие | No       | 248.05 us | 4,214.9 ns | 16.324 us |  3.11 |    0.30 |  4,031 |  78.73 KB |
| Асинхронный запуск: Лямбда   | No       | 417.69 us | 4,943.7 ns | 19.147 us |  5.23 |    0.45 |  2,394 | 121.19 KB |
