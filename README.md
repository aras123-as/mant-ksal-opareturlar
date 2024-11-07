#      MANTIKSAL OPERATÖRLER
Mantıksal operatörler, genellikle bilgisayar bilimleri ve matematikte, doğruluk değerleri (true/false veya 1/0) ile çalışarak mantıksal ifadeleri değerlendiren araçlardır. Bu operatörler, özellikle programlama dillerinde ve mantık sistemlerinde kullanılır. En yaygın mantıksal operatörler şunlardır:

#    1. AND (VE) Operatörü:
Mantıksal AND operatörü, iki veya daha fazla ifadenin aynı anda doğru olup olmadığını kontrol eder. Tüm ifadeler doğru ise sonuç doğru olur, aksi takdirde yanlış olur.

Simge: && veya &
Tablo (2 girişli):
A	B	A AND B
0	0	0
0	1	0
1	0	0
1	1	1
Örnek:
(A && B) → A ve B'nin ikisi de doğru (1) olursa, sonuç doğru (1) olur.

#   2. OR (VEYA) Operatörü:
Mantıksal OR operatörü, verilen ifadelerden en az birinin doğru olup olmadığını kontrol eder. Eğer en az bir ifade doğruysa, sonuç doğru olur.

Simge: || veya |
Tablo (2 girişli):
A	B	A OR B
0	0	0
0	1	1
1	0	1
1	1	1
Örnek:
(A || B) → A veya B'den en az biri doğru (1) olduğunda, sonuç doğru (1) olur.

#    3. NOT (DEĞİL) Operatörü:
Mantıksal NOT operatörü, bir ifadenin doğruluk değerini tersine çevirir. Eğer ifade doğruysa, sonuç yanlış olur; eğer yanlışsa, sonuç doğru olur.

Simge: !
Tablo (1 girişli):
A	NOT A
0	1
1	0
Örnek:
!A → Eğer A doğruysa (1), NOT A yanlış olur (0); eğer A yanlışsa (0), NOT A doğru olur (1).

#   4. XOR (ÖZEL VEYA) Operatörü:
Mantıksal XOR (Exclusive OR) operatörü, yalnızca bir ifadenin doğru olması durumunda doğru döner. Yani, her iki ifade de aynıysa (ikisi de doğru veya ikisi de yanlış), sonuç yanlıştır. Ancak birinin doğru, diğerinin yanlış olması durumunda sonuç doğrudur.

Simge: ^
Tablo (2 girişli):
A	B	A XOR B
0	0	0
0	1	1
1	0	1
1	1	0
Örnek:
(A ^ B) → A ve B'nin değerleri farklıysa, sonuç doğru (1) olur.

#  5. NAND (NOT AND) Operatörü:
Mantıksal NAND operatörü, AND operatörünün tersine çalışır. Yani, iki ifade doğruysa, sonuç yanlış olur; diğer durumlarda sonuç doğru olur.

Simge: NAND
Tablo (2 girişli):
A	B	A NAND B
0	0	1
0	1	1
1	0	1
1	1	0
Örnek:
(A NAND B) → A ve B ikisi de doğru olduğunda, sonuç yanlış olur.

 #   6. NOR (NOT OR) Operatörü:
Mantıksal NOR operatörü, OR operatörünün tersine çalışır. Yani, iki ifade doğru olduğunda sonuç yanlış olur, diğer tüm durumlarda sonuç doğru olur.

Simge: NOR
Tablo (2 girişli):
A	B	A NOR B
0	0	1
0	1	0
1	0	0
1	1	0
Örnek:
(A NOR B) → A ve B'nin ikisi de yanlış olduğunda sonuç doğru olur.

Mantıksal Operatörler Nerelerde Kullanılır?
Programlamada: Mantıksal operatörler, koşul ifadeleri (if, else, while, for) ve mantıksal denetimlerde kullanılır. Örneğin, bir programda belirli bir koşulun sağlanıp sağlanmadığını kontrol etmek için mantıksal operatörler kullanılır.
Dijital Elektronikte: Dijital devrelerde mantıksal kapılar (AND, OR, NOT vb.) kullanılarak ikili sistemlerde çeşitli hesaplamalar yapılır.
Veritabanlarında: SQL sorgularında mantıksal operatörler (AND, OR, NOT) kullanılarak sorgulara filtreleme ve şart eklenir.
Matematiksel Mantıkta: Mantıksal operatörler, çeşitli mantıksal ifadeleri çözümlemek için kullanılır.



#                  ÖRNEKLER
#  1. AND (VE) Operatörü Örneği:
Bir kullanıcı, belirli bir yaşın üzerinde ve belirli bir üyelik türüne sahip olmalıdır. Her iki şartın da sağlanıp sağlanmadığını kontrol etmek için AND operatörü kullanılır.

Koşul:

Yaş >= 18 ve üyelik türü = "premium" olmalı.
Programlama Örneği (Python):

python
Kodu kopyala
yas = 25
uyelik_turu = "premium"

if yas >= 18 and uyelik_turu == "premium":
    print("Erişim izni verildi.")
else:
    print("Erişim izni verilmedi.")
Açıklama:
Bu örnekte, hem yas >= 18 hem de uyelik_turu == "premium" koşullarının her ikisi de doğru olmalıdır. Eğer her ikisi de sağlanıyorsa, "Erişim izni verildi." mesajı yazdırılır.

#      2. OR (VEYA) Operatörü Örneği:
Bir kullanıcı, ya belirli bir yaşın üzerinde ya da belirli bir üyelik türüne sahip olmalıdır. OR operatörü kullanılarak, herhangi bir şartın sağlanıp sağlanmadığı kontrol edilir.

Koşul:

Yaş >= 18 veya üyelik türü = "premium" olmalı.
Programlama Örneği (Python):

python
Kodu kopyala
yas = 16
uyelik_turu = "basic"

if yas >= 18 or uyelik_turu == "premium":
    print("Erişim izni verildi.")
else:
    print("Erişim izni verilmedi.")
Açıklama:
Burada, yas >= 18 veya uyelik_turu == "premium" koşullarından biri doğru olursa, "Erişim izni verildi." mesajı yazdırılır. Eğer her ikisi de yanlışsa, "Erişim izni verilmedi." mesajı gösterilir.

#       3. NOT (DEĞİL) Operatörü Örneği:
Bir kullanıcının admin olup olmadığına göre işlem yapılacaktır. Eğer kullanıcı admin değilse, "Kısıtlı erişim" mesajı gösterilecektir. Burada NOT operatörü, admin olup olmadığını tersine çevirmek için kullanılır.

Koşul:

Kullanıcı admin değilse, "Kısıtlı erişim" mesajı gösterilsin.
Programlama Örneği (Python):

python
Kodu kopyala
admin = False

if not admin:
    print("Kısıtlı erişim")
else:
    print("Admin erişimi")
Açıklama:
Burada, not admin ifadesi False olduğu için, sonuç "Kısıtlı erişim" olacaktır. Eğer admin = True olsaydı, sonuç "Admin erişimi" olurdu.

#        4. XOR (ÖZEL VEYA) Operatörü Örneği:
Bir programda, kullanıcı ya 18 yaşından büyük olmalı ya da "vip" üyelik türüne sahip olmalı, ancak ikisinin birden olması durumu geçersiz sayılacaktır. Bu durumda XOR operatörü kullanılabilir.

Koşul:

Yaş >= 18 veya üyelik türü = "vip", ancak ikisi de aynı anda doğru olamaz.
Programlama Örneği (Python):

python
Kodu kopyala
yas = 25
uyelik_turu = "basic"

if (yas >= 18) != (uyelik_turu == "vip"):
    print("Erişim izni verildi.")
else:
    print("Erişim izni verilmedi.")
Açıklama:
Burada != operatörü, XOR mantığına benzer bir şekilde çalışır: Yaş >= 18 ve üyelik türü "vip" aynı anda doğru olursa, erişim izni verilmez.

#       5. NAND (NOT AND) Operatörü Örneği:
Bir kullanıcı, hem bir yetkili olmalı hem de belirli bir şifreyi girmelidir. Ancak, NAND operatörü ile, her iki koşulun da doğru olduğu durum hariç, erişim verilecektir.

Koşul:

Ya yetkili olmalı ya da doğru şifreyi girmeli, ancak ikisinin de doğru olduğu durum hariç.
Programlama Örneği (Python):

python
Kodu kopyala
yetkili = True
dogru_sifre = False

if not (yetkili and dogru_sifre):
    print("Erişim izni verildi.")
else:
    print("Erişim izni verilmedi.")
Açıklama:
Bu örnekte, her iki koşul da doğru olursa (yetkili = True ve dogru_sifre = True), "Erişim izni verilmedi." mesajı yazdırılır. Diğer tüm durumlarda ise "Erişim izni verildi." mesajı gösterili







