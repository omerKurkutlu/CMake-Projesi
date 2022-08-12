# CMake

CMake, derleyiciden bağımsız bir yöntem kullanarak yazılımın oluşturulması, otomasyonu, test edilmesi, paketlenmesi ve kurulumu için platformlar arası ücretsiz ve açık kaynaklı bir yazılımdır. CMake bir derleme sistemi değildir, bunun yerine başka bir sistemin derleme dosyalarını oluşturur.

## Execution

GitHub'tan projeyi indin ve size uygun IDE'de programı açın.(VSCode tavsiye edilir, CMake extension kullanarakta çalıştırabilirsiniz veya Terminal yardımıı ile...) <br/>

### 1-Dosyayi indirdiginiz yerde saga tiklayip, ternimal ac secenegini tiklayiniz 


### 2-'build' dosyasına girin

```bash
cd build
```

### 3-Programı execute etmek için once 

```bash
cmake ..
```
### 3-Sonra

```bash
make
```
### 3-Programı calistirmak icinde

```bash
./Deneme
```

### OUTPUT Şu şekilde olmalı

```bash
Greetings POLONOM

Student name=Omer KURKUTLU
Student Id=15

Hence, we succesfully  implemented CMake
```

