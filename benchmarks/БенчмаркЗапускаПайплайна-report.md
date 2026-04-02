> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                       | Baseline |        Mean |   StdErr |    StdDev | Ratio | RatioSD |     Op/s | Allocated |
|------------------------------|----------|------------:|---------:|----------:|------:|--------:|---------:|----------:|
| Запуск: Действие             | Yes      |    80.08 us | 3.779 us | 14.636 us |  1.00 |    0.00 | 12,486.9 |  37.74 KB |
| Асинхронный запуск: Действие | No       |   225.25 us | 2.358 us |  9.134 us |  2.87 |    0.37 |  4,439.5 |  77.16 KB |
| Запуск: Лямбда               | No       | 1,384.16 us | 3.689 us | 14.288 us | 17.66 |    2.15 |    722.5 | 520.70 KB |
| Асинхронный запуск: Лямбда   | No       | 1,603.03 us | 5.917 us | 22.917 us | 20.45 |    2.50 |    623.8 | 560.42 KB |
