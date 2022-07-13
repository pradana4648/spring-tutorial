# Hal - hal yang ada pada Java Spring

- Application Context

  Menggunakan IoC (Inversi of Control) / Container.

- Singleton :

  Object yang hanya dibuat 1 kali saja, jika membuat object baru akan mengembalikan object sama lagi.

- Bean :

  Saat masuk ke dalam IoC disebut Bean, secara default Bean adalah singleton dan Bean otomatis akan dibuat dan dipanggil di IoC.

  **_Dalam membuat Bean harus terdapat anotasi @Configuration_**

  - Duplicate Bean:

    Bean bisa menggunakan tipe data yang sama, jika sama harus membuat nama Bean yang berbeda dan untuk mengaksesnya harus menggunakan nama Bean yang telah dibuat.

  - Primary Bean :

    Bean yang hanya bisa dipilih menjadi paling utama untuk mengaksesnya, secara otomatis saat dipanggil maka primary bean-nya akan terpilih.

  - Mengubah nama Bean :

    Secara default nama Bean menggunakan nama method, pada dasarnya Bean adalah unik dan tidak boleh sama, maka dari itu mengubah Bean berguna jika terjadi bentrok antar Bean yang sama. Mengubah nama Bean dengan menambah method value di dalam anotasi @Bean().

- Dependency Injection :

  DI adalah konsep membuat obyek secara otomatis yang bergantung pada obyek lainnya atau disebut dependencies, otomatis DI akan masuk (inject) ke dalam obyek yang dibutuhkan.
  Konsepnya sama dengan IoC
  Tanpa DI akan sulit untuk membuat relasi antar dependencies.

  - Spring DI :

    Spring sejak awal menggunakan DI
    Membuat method untuk Bean bisa menggunakan parameter  
    Secara otomatis Spring akan mencari bean sesuai dengan tipe parameter tersebut
    Terjadi error jika tidak ada Bean yang cocok dan terdapat lebih dari 1 Bean kecuali terdapat Primary Bean

# Sumber belajar

[Youtube here](https://www.youtube.com/watch?v=VM3rwdMBORY)

# TODO

- [x] IoC / Container
- [x] Application Context
- [x] Singleton
- [x] Bean
- [x] Duplicate Bean
- [x] Primary Bean
- [x] Mengubah Nama Bean
- [x] Dependency Injection
- [ ] Memilih Dependency
- [ ] Circular Dependencies
- [ ] Depends On
- [ ] Lazy Bean
- [ ] Scope
- [ ] Membuat Scope
- [ ] Life Cycle
- [ ] Life Cycle Annotation
- [ ] Import
- [ ] Component Scan
- [ ] Component
- [ ] Constructor-based Dependency Injection
- [ ] Setter-based Dependency Injection
- [ ] Field-based Dependency Injection
- [ ] Qualifier
- [ ] Optional Dependency
- [ ] Factory Bean
- [ ] Inheritance
- [ ] Bean Factory
- [ ] Bean Post Processor
- [ ] Ordered
- [ ] Aware
- [ ] Bean Factory Post Processor
- [ ] Event Listener
- [ ] Event Listener Annotation
- [ ] Spring Boot Application
- [ ] Startup Failure
- [ ] Banner
- [ ] Customizing Spring Application
- [ ] Spring Application Event
- [ ] Command Line Runner
- [ ] Application Runner
- [ ] Spring Boot Plugin
