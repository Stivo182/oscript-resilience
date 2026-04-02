> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                         | Baseline |      Mean |    StdErr |      StdDev | Ratio | RatioSD |    Median |    Op/s | Allocated |
|--------------------------------|----------|----------:|----------:|------------:|------:|--------:|----------:|--------:|----------:|
| Прямой вызов                   | Yes      |  3.509 us | 401.30 ns | 1,554.21 ns |  1.00 |    0.00 |  2.674 us | 284,988 |  1.211 KB |
| Обработчик-делегат             | No       |  6.545 us |  25.41 ns |    98.41 ns |  2.11 |    0.58 |  6.518 us | 152,788 |  2.258 KB |
| Обработчик-лямбда              | No       |  9.011 us |  32.40 ns |   125.48 ns |  2.91 |    0.80 |  9.008 us | 110,979 |  4.078 KB |
| Обработчик-лямбда с параметром | No       | 10.212 us |  28.93 ns |   112.04 ns |  3.29 |    0.91 | 10.209 us |  97,923 |  4.641 KB |
