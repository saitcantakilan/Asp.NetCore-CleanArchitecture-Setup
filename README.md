# .NET-CleanArchitecture-Setup

Bu repo, .NET 7 kullanılarak oluşturulmuş bir kod merkezidir ve Clean Architecture prensiplerine uygun olarak tasarlanmıştır. Bu merkez, MediatR, Fluent Validation, Serilog gibi popüler paketleri kullanmaktadır ve Dependency Injection kullanımını desteklemektedir.

## Gereksinimler

- .NET 7 SDK yüklü olmalıdır. İndirmek için [buraya](https://dotnet.microsoft.com/download/dotnet/7.0) tıklayabilirsiniz.

## Proje Yapısı

Bu repo, aşağıdaki projelerden oluşmaktadır:

- `.API`: ASP.NET 7 Core Web API projesidir ve dış dünyayla iletişimi sağlar.
- `.Application`: Uygulama katmanıdır ve iş mantığını uygular.
- `.Domain`: Domain katmanıdır ve iş mantığı kurallarını içerir.
- `.Infrastructure`: Altyapı katmanıdır ve veritabanı erişimi, harici servis entegrasyonu gibi işlemleri gerçekleştirir.
- `.Presentation:` Sunum katmanıdır ve kullanıcı arayüzü ile etkileşim sağlar.



## Kullanım

Bu repo, Clean Architecture prensiplerine dayalı olarak tasarlanmıştır ve genel olarak aşağıdaki adımları takip eder:

1. API projeleri, gelen istekleri yönlendirir ve cevapları döndürür.
2. Uygulama katmanı, iş mantığını uygular ve gerektiğinde domain katmanını kullanır.
3. Domain katmanı, iş mantığı kurallarını içerir ve varlık (entity) sınıflarını tanımlar.
4. Altyapı katmanı, veritabanı erişimi, harici servis entegrasyonu gibi işlemleri gerçekleştirir.

#### Bu repo, MediatR paketini kullanarak CQRS (Command Query Responsibility Segregation) tasarım desenini uygular. Buna ek olarak, Fluent Validation paketi giriş doğrulama işlemleri için kullanılır ve Serilog paketi ise günlük (log) tutmak için kullanılır.
