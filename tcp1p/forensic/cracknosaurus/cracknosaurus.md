# Cracknosaurus

Pada challenge ini, diberikan file flag.zip yang diberikan yang terenkrip

<image src="./zip.png" />

pendekatan pertama yang saya lakukan adalah dengan menggunakan john the ripper menggunakan zip2john untuk mengekstrak hash yang ada pada flag.zip untuk digunakan oleh jtr

<image src="./1.png"/>

lalu menggunakan wordlist rockyou pada keluaran dari zip2john sebelumnya menggunakan kode berikut 

<image src="./2.png"/>

dengan menggunakan option --show maka akan muncul password dari file zipnya 

<image src="./3.png"/>

keluaran dari file zip tersebut adalah sebuah image berikut 

<image src="./flag.jpeg"/>

setelah menggunakan aperisolve, saya tidak menemukan hal yang mencurigakan selain terdapat file yang terenkripsi di dalam gambar tersebut sehingga saya menggunakan stegseek dengan wordlist rockyou 

<image src="./4.png"/>

setelah mendapatkan passphrasenya menggunakan stegseek, filenya tinggal saya cat dan muncullah flagnya 

<image src="./5.png"/>

Flag = TCP1P\{{m4st3r1ng_cr4ck1ng_w1th_r0cky0u!!!}\}

