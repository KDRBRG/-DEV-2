# -DEV-2
PROGRAMLAMA DİLLERİNİN İŞLEM SÜRELERİ

1.)C++
#include <iostream>
 #include <ctime>
 int main() {
 clock_t start = clock();
 std::cout << "Merhaba MIS, algoritma ve programlama \n";
 clock_t end = clock();
 double time_spent = (double)(end- start) /
 CLOCKS_PER_SEC;
 std::cout << "C++ işlem süresi: " << time_spent << "
 saniye\n";
 return 0;
 }

Sonuç: merhaba MIS,algoritma ve programlma 
C++işlem süresi:1.5e-05saniye

2.) C
#include <stdio.h>
#include <time.h>

int main(){
  clock_t end =clock();
  printf("Merhaba MIS,algoritma ve programlama \n");
  double time_spent=(double)(end)/
CLOCKS_PER_SEC;
  printf("C işlem süresi:%f saniye\n",time_spent);
  return 0;
}

SONUÇ: Merhaba MIS,algoritma ve programlama 
C işlem süresi:0.003730 saniye

3.) PYTHON
import time
 start = time.time()
 print("Merhaba MIS, algoritma ve programlama
 dersi başladı")
 end = time.time()
 print(f"Python işlem süresi: {end- start} saniye")
 
SONUÇ:Merhaba MIS,algoritma ve programlama dersi başladı
python işlem süresi :2.5033950805664062e-05 saniye

4.) JAVA
public class Main {
    public static void main(String[] args) {
        long startTime =System.nanoTime();
        
        System.out.println("Merhaba MIS,algoritma ve programlama dersi başladı");
        
        long endTime =System.nanoTime();
        double duration = (endTime - startTime)/
    1_000_000.0;// milisaniye cinsine çevir
        System.out.println("Java işlem süresi:"+duration+"milisaniye");
  }
}

SONUÇ: Merhaba MIS,algoritma ve programlama dersi başladı
Java işlem süresi:0.407749milisaniye

5.)C#
using System;
using System.Diagnostics;

class Program
{
    static void Main()
    {
        Stopwatch stopwatch = new Stopwatch();
        stopwatch.Start();
        
        Console.WriteLine("Merhaba MIS,algoritma ve programlma dersi başladı");
        
        stopwatch.Stop();
        Console.WriteLine($"C# işlem süresi: {stopwatch.Elapsed.TotalSeconds}saniye");
    }
}

SONUÇ: Merhaba MIS,algoritma ve programlma dersi başladı
C# işlem süresi: 0.0382918saniye

6.) PERL
use Time::HiRes qw(time);
 my $start = time();
 print "Merhaba MIS, algoritma ve programlama\n";
 my $end = time();
 printf "Perl işlem süresi: %f saniye\n", $end- $start;
 
SONUÇ: Merhaba MIS, algoritma ve programlamaPerl işlem süresi: 0.000013 saniye

7.)RUBY
start = Time.now
 puts "Merhaba MIS, algoritma ve programlama"
 finish = Time.now
 puts "Ruby işlem süresi: #{finish- start} saniye"
 
SONUÇ: Merhaba MIS, algoritma ve programlama
Ruby işlem süresi: 1.7114e-05 saniye

8.) RUST
use std::time::Instant;
 fn main() {
 let start = Instant::now();
 println!("Merhaba MIS, algoritma ve programlama");
 let duration = start.elapsed();
 println!("Rust işlem süresi: {:?}", duration);
 }
 
 SONUÇ: Merhaba MIS, algoritma ve programlama
Rust işlem süresi: 9.554µs

9.) GO
package main
 import (
 "fmt"
 "time"
 )
 func main() {
 start := time.Now()
 fmt.Println("Merhaba MIS, algoritma ve programlama")
 elapsed := time.Since(start)
 fmt.Printf("Go işlem süresi: %s saniye\n", elapsed)
 }
 
SONUÇ: Merhaba MIS, algoritma ve programlama
Go işlem süresi: 56.827µs saniye

10.) JAVASCRİPT
const startTime = process.hrtime();
 console.log("Merhaba MIS, algoritma ve programlama dersi
 başladı");
 const endTime = process.hrtime(startTime);
 const duration = endTime[0] * 1e3 + endTime[1] / 1e6; //
 milisaniye cinsine çevir
 console.log(`JavaScript işlem süresi: ${duration.toFixed(3)} milisaniye`);
 
SONUÇ: Merhaba MIS, algoritma ve programlama dersi başladı
JavaScript işlem süresi: 5.780
 Milisaniye


 using System;
 using System.Diagnostics;
 class Program
 {
 static void Main()
 {
 Stopwatch stopwatch = new Stopwatch();
 stopwatch.Start();
 Console.WriteLine("Merhaba MIS, algoritma ve programlama dersi başladı");
 stopwatch.Stop();
 Console.WriteLine($"C# işlem süresi: {stopwatch.Elapsed.TotalSeconds} saniye");
 }
 }





