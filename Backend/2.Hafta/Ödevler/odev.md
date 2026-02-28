# 🎓 Java Proje Ödevi

## 📌 Konu: Konsol Tabanlı Öğrenci Not Yönetim Sistemi

Bu projede, şimdiye kadar öğrendiğin **tüm Java temel konularını birlikte kullanarak** çalışan bir konsol uygulaması geliştirmen beklenmektedir.

Amaç: Java’nın sadece parçalarını değil, **bir programın tamamını kurabildiğini** göstermek.

---

## 🎯 Projenin Amacı

Bir öğretmenin öğrencilerin notlarını girebildiği ve takip edebildiği bir sistem geliştirilecektir.

Program:

* Öğrenci ekleyebilecek
* Öğrencileri listeleyebilecek
* En başarılı öğrenciyi bulabilecek
* Öğrencinin geçip kalma durumunu belirleyebilecek

---

## 🧠 Bu Projede Kullanman Gereken Konular

Bu ödev özellikle aşağıdaki konuları **aktif olarak kullanman** için hazırlanmıştır:

* Java syntax kuralları
* Değişkenler ve veri tipleri
* Scanner ile veri alma
* if / else yapıları
* switch-case
* Döngüler (for, while, foreach)
* Diziler
* Class & Object mantığı
* Constructor
* this anahtar kelimesi
* Method yazımı
* Method overloading
* Paket (package) yapısı
* Access modifiers (private, public)

---

## 🏗 Proje Senaryosu

Sistemde her öğrenci için şu bilgiler tutulacaktır:

* Adı
* Numarası
* 3 adet ders notu

Program bu notlara göre:

* Ortalama hesaplayacak
* "Geçti" veya "Kaldı" durumunu belirleyecek
* Tüm öğrencileri listeleyecek
* En yüksek ortalamaya sahip öğrenciyi gösterecek

---

## 📦 Zorunlu Paket Yapısı

Projen aşağıdaki klasör yapısında olmalıdır:

```
school/
 ├── Main.java
 ├── model/
 │     └── Student.java
 └── service/
       └── StudentService.java
```

---

## 👤 Student Sınıfı (model paketi)

Bu sınıf bir öğrenciyi temsil eder.

### Alanlar (private olmalı):

* name
* number
* note1
* note2
* note3

### Constructor:

Öğrenci oluşturulurken tüm bilgiler alınmalıdır.

### Metotlar:

| Metot              | Görev                                      |
| ------------------ | ------------------------------------------ |
| calculateAverage() | Notların ortalamasını hesaplar             |
| getStatus()        | Ortalama ≥ 50 ise "Geçti", değilse "Kaldı" |
| Getter metotları   | Bilgilere erişim için                      |

---

## ⚙️ StudentService Sınıfı (service paketi)

Bu sınıf öğrenci işlemlerini yönetecektir.

Bir dizi kullanılmalıdır:

```
Student[] students = new Student[100];
int count = 0;
```

### Metotlar:

| Metot                 | Açıklama                   |
| --------------------- | -------------------------- |
| addStudent(Student s) | Yeni öğrenci ekler         |
| listStudents()        | Tüm öğrencileri listeler   |
| findBestStudent()     | En yüksek ortalamayı bulur |
| showMenu()            | Menü yazdırır              |

---

## 🖥 Main Sınıfı

Programın başlangıç noktasıdır.

Program bir döngü içinde çalışmalıdır.

### Menü:

```
1 - Öğrenci Ekle
2 - Öğrencileri Listele
3 - En Başarılı Öğrenciyi Göster
4 - Çıkış
```

---

## 🔧 Zorunlu Kullanımlar

| Konu               | Nerede Kullanılacak                      |
| ------------------ | ---------------------------------------- |
| Scanner            | Kullanıcıdan veri almak                  |
| while döngüsü      | Menü sistemi                             |
| switch             | Menü seçimleri                           |
| if-else            | Geçme kalma kontrolü                     |
| for                | En iyi öğrenciyi bulma                   |
| foreach            | Listeleme                                |
| break/continue     | Menü kontrolü                            |
| Casting            | Not girişlerinde                         |
| Method overloading | Ortalama hesaplama için alternatif metot |

---

## 📋 Teslim Şartları

* Kodlar paket yapısına uygun olmalı
* Her sınıf ayrı dosyada olmalı
* Kod içinde açıklama satırları bulunmalı
* Program hatasız çalışmalı

---

💡 **Amaç sadece çalışan kod değil; doğru yapı, doğru tasarım ve konuları doğru kullanmandır.**

