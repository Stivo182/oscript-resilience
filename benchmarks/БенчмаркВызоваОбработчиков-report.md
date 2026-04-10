> BenchmarkOneScript v0.8.0, OneScript v2.0.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                         | Baseline |      Mean |    StdErr |     StdDev | Ratio | RatioSD |    Op/s | Allocated |
|--------------------------------|----------|----------:|----------:|-----------:|------:|--------:|--------:|----------:|
| Прямой вызов                   | Yes      |  4.563 us | 438.69 ns | 1,699.0 ns |  1.00 |    0.00 | 219,130 |  1.211 KB |
| Обработчик-делегат             | No       |  6.618 us |  30.54 ns |   118.3 ns |  1.68 |    0.65 | 151,107 |  2.258 KB |
| Обработчик-лямбда              | No       |  9.172 us |  50.20 ns |   194.4 ns |  2.33 |    0.89 | 109,026 |  4.078 KB |
| Обработчик-лямбда с параметром | No       | 10.230 us |  54.24 ns |   210.1 ns |  2.60 |    1.00 |  97,755 |  4.641 KB |
