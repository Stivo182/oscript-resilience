BenchmarkOneScript v0.9.0, OneScript v2.1.0, Microsoft Windows NT 10.0.20348.0
Intel Core i7-8700 CPU 3.20GHz (Coffee Lake), 1 CPU, 12 logical and 6 physical cores

| Method                         | Baseline |      Mean |    StdErr |     StdDev | Ratio | RatioSD |    Op/s | Allocated |
|--------------------------------|----------|----------:|----------:|-----------:|------:|--------:|--------:|----------:|
| Прямой вызов                   | Yes      |  3.291 us | 289.80 ns | 1,122.4 ns |  1.00 |    0.00 | 303,827 |  1.211 KB |
| Обработчик-делегат             | No       |  6.674 us |  32.91 ns |   127.5 ns |  2.17 |    0.46 | 149,827 |  2.258 KB |
| Обработчик-лямбда              | No       |  9.148 us |  48.79 ns |   189.0 ns |  2.98 |    0.62 | 109,319 |  4.078 KB |
| Обработчик-лямбда с параметром | No       | 10.827 us | 160.96 ns |   623.4 ns |  3.53 |    0.76 |  92,359 |  4.641 KB |
