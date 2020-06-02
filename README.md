# Ujian kelompok 10


## Anggota
Terdapat enam orang anggota pada kelompok 10 ini dengan fraksi kontribusinya pada pengerjaan tiap soal dapat dilihat dalam tabel berikut.

| NIM      | Nama                  | Peran pada soal (dan fraksi kontribusinya)   |
|----------|-----------------------|----------------------------------------------|
|          |                       |                                              |
| 10212083 | Sidi Janardhana G P   | 1 (0.16) 2 (0.16) 3 (0.16) 4 (0.16) 5 (0.16) |
| 10216022 | Maria Ulfa Fidarain   | 1 (0.16) 2 (0.16) 3 (0.16) 4 (0.18) 5 (0.16) |
| 10216023 | Elma Alifa Nadya      | 1 (0.16) 2 (0.16) 3 (0.16) 4 (0.16) 5 (0.18) |
| 10216076 | Muhammad Choliq	   | 1 (0.16) 2 (0.16) 3 (0.16) 4 (0.18) 5 (0.16) |
| 10217005 | Fajar Mochamad Ramdan | 1 (0.20) 2 (0.18) 3 (0.16) 4 (0.16) 5 (0.16) |
| 10217060 | Adnan M.Lazuardi      | 1 (0.16) 2 (0.18) 3 (0.20) 4 (0.16) 5 (0.16) |
|          |                       |                                              |
|          | Total                 | 1 (1.00) 2 (1.00) 3 (1.00) 4 (1.00) 5 (1.00) |



# Jawaban
##Soal 1. Sistem Bandul dengan koordinat kartesian (Dapat dilihat menggunakan editor)
###a. Gaya yang bekerja pada bandul tersebut adalah gaya tegangan tali, gaya gesekan udara, gaya sentrifugal, dan gaya berat.
Kita tuliskan terlebih dahulu gaya-gaya yang bekerja tersebut :
Gaya Berat :
\begin{equation}
\label{eqn:nlode-w}
\vec{w} = -{mg}\hat{y}
\end{equation}

Gaya Tegangan Tali :
\begin{equation}
\label{eqn:nlode-T}
\vec{T} = -{mgcos{\theta}}\hat{r}
\end{equation}

\begin{equation}
\label{eqn:nlode-T1}
=-{mgcos{\theta}}{(sin{\theta}\hat{x} + cos{\theta}\hat{y})}
\end{equation}

\begin{equation}
\label{eqn:nlode-T2}
=-{mg}{(sin{\theta}cos{\theta}\hat{x} + cos^2{\theta}\hat{y})}
\end{equation}

dengan :
\begin{equation}
\label{eqn:nlode-Sin}
sin{\theta} = \frac{x}{\sqrt{x^2 + y^2}}
\end{equation}
dan
\begin{equation}
\label{eqn:nlode-Cos}
cos{\theta} = \frac{y}{\sqrt{x^2 + y^2}}
\end{equation}
didapatkan :

\begin{equation}
\label{eqn:nlode-Tn}
\vec{T} = - {mg}{(\frac{xy}{x^2 + y^2}\hat{x} + \frac{y^2}{x^2+y^2}\hat{y})}
\end{equation}

\begin{equation}
\label{eqn:nlode-Tx}
T_x = - {mg}\frac{xy}{x^2 + y^2} \\ T_y = - {mg}\frac{y^2}{x^2 + y^2}
\end{equation}

dengan
\begin{equation}
\label{eqn:nlode-l}
l^2 = x^2 + y^2
\end{equation}

maka didapatkan :
\begin{equation}
\label{eqn:nlode-Txn}
T_x = - {mg}\frac{xy}{l^2} \\ T_y = - {mg}\frac{y^2}{l^2}
\end{equation}

Untuk gaya gesekan udara :
\begin{equation}
\label{eqn:nlode-fkx}
f_x = bv_x
\end{equation}

\begin{equation}
\label{eqn:nlode-fky}
f_y = bv_y
\end{equation}

dengan
\begin{equation}
\label{eqn:nlode-b}
b = 3\pi\eta{D}
\end{equation}

didapatkan
\begin{equation}
\label{eqn:nlode-fkx1}
f_x = (3\pi\eta{D})\dot{x} \\ f_y = (3\pi\eta{D})\dot{y}
\end{equation}

Untuk Gaya Sentrifugal :
didapatkan
\begin{equation}
\label{eqn:nlode-fsg}
\vec{f_{sg}}= ma_{sg}\hat{r}\\
\vec{f_{sg}}=m\frac{v^2}{r}\hat{r}\\
\vec{f_{sg}}=m\frac{v^2}{r}{(sin{\theta}\hat{x}+cos{\theta}\hat{y})}
\end{equation}

dengan
\begin{equation}
\label{eqn:nlode-fsg1}
l=r\\v^2={v_x}^2+{v_y}^2\\sin{\theta} = \frac{x}{\sqrt{x^2 + y^2}}
\\cos{\theta} = \frac{y}{\sqrt{x^2 + y^2}}
\end{equation}

didapatkan :
\begin{equation}
\label{eqn:nlode-fsg2}
{f_{sgx}}= m\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x}\\
{f_{sgy}}= m\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y}
\end{equation}

Untuk penyelesaian persamaan diferensial nonlinier pada sumbu x :
\begin{equation}
\sum{F_x}= ma_x\\
\sum{F_x}=m\ddot{x}\\
f_{sgx} - T_x - f_x = m\ddot{x}\\
m\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x} - {mg}\frac{xy}{l^2} - (3\pi\eta{D})\dot{x} = m\ddot{x}
\end{equation}
semua ruas dibagi m, maka akan didapatkan :

\begin{equation}
\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x} - {g}\frac{xy}{l^2} -(\frac{(3\pi\eta{D})}{m})\dot{x} = \ddot{x}\\
\ddot{x} + (\frac{(3\pi\eta{D})}{m})\dot{x} - \frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x} + {g}\frac{xy}{l^2}= 0
\end{equation}
dengan menggunakan gaya-gaya yang telah disebutkan sebelumnya dan tambahan gaya berat (hanya pada sumbu y saja), maka akan didapatkan :
\begin{equation}
\sum{F_y}= ma_y\\
\sum{F_y}=m\ddot{y}\\
f_{sgy} - T_y - f_y - w = m\ddot{x}\\
m\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y} - {mg}\frac{y^2}{l^2} - (3\pi\eta{D})\dot{y} - mg = m\ddot{y}
\end{equation}
semua ruas dibagi m, maka akan didapatkan :

\begin{equation}
\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y} - {g}\frac{y^2}{l^2} -(\frac{(3\pi\eta{D})}{m})\dot{y} - g = \ddot{y}\\
\ddot{y} + (\frac{(3\pi\eta{D})}{m})\dot{y} - \frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y} + {g}\frac{y^2}{l^2}= -g
\end{equation}

###b. Untuk suku pada ruas kiri pada sumbu x dan sumbu y sama, maka penjelasan berikut berlaku untuk kedua sumbu tersebut.
Untuk suku pertama merupakan percepatan total yang akan ditempuh oleh bandul untuk masing-masing sumbu. Lalu, untuk suku kedua merupakan gayak gesek udara yang dapat memperkecil laju dari bandul tersebut. Kemudian untuk suku ketiga merupakan gaya sentrifugal, yang merupakan lawan dari gaya sentripental yang bekerja pada sistem, gaya ini dapat memperbesar laju dari bandul. Setelah itu untuk suku keempat merupakan gaya tegangan tali yang dapat memperkecil laju dari bandul.
Pada sumbu y, terdapat g disumbu kanan, yang merupakan akibat dari gaya berat yang terjadi pada bandul. Percepatan gravitasi bumi tersebut hanya terdapat pada sumbu y saja, sehingga akan memperlambat laju dari bandul tersebut.

###c.Untuk benda jatuh bebas :
Persamaan 2 :
\begin{equation}
\sum{F_x}= ma_x\\
\sum{F_x}=m\ddot{x}\\
f_{sgx} - T_x  = m\ddot{x}\\
m\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x} - {mg}\frac{xy}{l^2}  = m\ddot{x}
\end{equation}
semua ruas dibagi m, maka akan didapatkan :

\begin{equation}
\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x} - {g}\frac{xy}{l^2} = \ddot{x}\\
\ddot{x}  - \frac{(\dot{x}^2+\dot{y}^2)}{l^2}{x} + {g}\frac{xy}{l^2}= 0
\end{equation}
Persamaan 3 :
\begin{equation}
\sum{F_y}= ma_y\\
\sum{F_y}=m\ddot{y}\\
f_{sgy} - T_y  - w = m\ddot{x}\\
m\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y} - {mg}\frac{y^2}{l^2} - mg = m\ddot{y}
\end{equation}
semua ruas dibagi m, maka akan didapatkan :

\begin{equation}
\frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y} - {g}\frac{y^2}{l^2} - g = \ddot{y}\\
\ddot{y} - \frac{(\dot{x}^2+\dot{y}^2)}{l^2}{y} + {g}\frac{y^2}{l^2}= -g
\end{equation}

Parameter eta tersebut merupakan koefisien dari gaya gesek udara, ketika bandul tersebut mengalami jatuh bebas, maka dapat menghambat gerak dari bandul tersebut (sebelum menyentuh tanah), namun dalam kondisi ini kita asumsikan bahwa tidak ada pengaruh dari gaya gesek udara. Lalu untuk parameter l, yang merupakan panjang dari tali bandul tersebut, ketika bandul mengalami jatuh bebas maka, maka dapat menghambat gerak dari bandul tersebut karenna pengaruh dari tegangan akibat tali terhadap bandul.

###d.Untuk bandul dengan simpangan kecil, maka tidak ada pengaruh dari gaya sentrifugal. Disini kita asumsikan juga tidak ada pengaruh dari gaya gesek udara, maka didapatkan :

Persamaan 2 :
\begin{equation}
\sum{F_x}= ma_x\\
\sum{F_x}=m\ddot{x}\\
 - T_x  = m\ddot{x}\\
 - {mg}\frac{xy}{l^2}  = m\ddot{x}
\end{equation}
semua ruas dibagi m, maka akan didapatkan :

\begin{equation}
 - {g}\frac{xy}{l^2} = \ddot{x}\\
\ddot{x}  + {g}\frac{xy}{l^2}= 0
\end{equation}

Persamaan 3 :
\begin{equation}
\sum{F_y}= ma_y\\
\sum{F_y}=m\ddot{y}\\
 - T_y  - w = m\ddot{x}\\
 - {mg}\frac{y^2}{l^2} - mg = m\ddot{y}
\end{equation}
semua ruas dibagi m, maka akan didapatkan :

\begin{equation}
 - {g}\frac{y^2}{l^2} - g = \ddot{y}\\
\ddot{y}  + {g}\frac{y^2}{l^2}= -g
\end{equation}

Penjelasan untuk sumbu x dan sumby pada ruas kiri sama, yaitu untuk suku pertama merupakan perecepatan total dari gerak yang dilakukan oleh bandul. Dari percepatan terebut bisa kita cari persamaan geraknya. Lalu untuk suku kedua merupakan pengaruh gaya tegangan tali terhadap bandul, yang mana dapat menghambat gerak dari bandul tersebut (gerak bandul akan tergantung pula terhadap tali tersebut). Lalu untuk sumbu y, terdapat pengaruh langsung dari percepatan gravitasi bumi, yang dapat menghambat gerak dari bandul tersebut. 

##Soal 2.Sistem bandul dalam koordinat polar (dapat dilihat dengan menggunakan editor)
###a. Persamaan differensial
Percepatan pada koordinat polar dinyatakan oleh
\begin{equation}
\vec{a}=\hat{r}(\ddot{r}-r\dot{\theta}^2)+\hat{\theta}(r\ddot{\theta}+2\dot{r}\dot{\theta})
\end{equation}


Tinjau dengan menggunakan Hukum 2 Newton untuk arah $\hat{\theta}$
\begin{equation}
\sum F_{\theta}=m(r\ddot{\theta}+2\dot{r}\dot{\theta})
\end{equation}

Karena $r=l$, $\dot{r}=0$, dan $\ddot{r}=0$,
\begin{equation}
\sum F_{\theta}=m(r\ddot{\theta}) \\
-mg\sin\theta=m(r\ddot{\theta}) \\
\frac{g}{l}\sin\theta=m\ddot{\theta}
\end{equation}

Tinjau dengan menggunakan Hukum 2 Newton untuk arah $\hat{r}$
\begin{equation}
\sum F_{r}=m(\ddot{r}-r\dot{\theta}^2) \\
\sum F_{r}=-mr\dot{\theta}^2 \\
-T+mg\cos\theta=-ml\dot{\theta}^2 \\
\frac{T}{ml}-\frac{g}{l}\cos\theta=-\dot{\theta}^2
\end{equation}
###c. Solusi analitik
Solusi analitik untuk nilai $\theta$ kecil,
karena $\theta$ kecil maka $\sin\theta\approx\theta$ sehingga
\begin{equation}
\ddot{\theta}+\frac{g}{l}\theta=0
\end{equation}

Diketahui solusi umumnya
\begin{equation}
\theta(t)=A\sin\omega t+B\cos\omega t \\
\ddot{\theta}(t)=-\omega^2(A\sin\omega t+B\cos\omega t) \\
\ddot{\theta}(t)=-\omega^2\theta
\end{equation}

Substitusikan kedalam persamaan awal, sehingga diperoleh
\begin{equation}
\frac{g}{l}=\omega^2
\end{equation}

Jika $\theta(0)=\theta_0$ dan $\dot{\theta}(0)=0$, maka
\begin{equation}
\dot{\theta}(0)=A\omega\cos(0)-B\omega\sin(0)=A\omega=0 \\
\theta(t)=B\cos\sqrt{\frac{g}{l}}t=0
\end{equation}
Sehingga didapatkan $A=0$ dan $B=\theta_0$ dan solusinya ialah
\begin{equation}
\theta(t)=\theta_0\cos\sqrt{\frac{g}{l}}t \\
T=\frac{2\pi}{\omega}=2\pi\sqrt{\frac{l}{g}}
\end{equation}

###c. Solusi numerik
    Diketahui hubungan euler
\begin{equation}
f^{n}(t+\Delta t)=f^{n}(t)+f^{n+1}(t)\Delta t
\end{equation}
$\theta$ dapat dinyatakan dalam hubungan tersebut dengan
\begin{equation}
\int_{t_0}^{t}\dot{\theta}(t)dt=\theta(t)-\theta(t_0) \\
\dot{\theta}(t)(t-t_0)=\theta(t)-\theta(t_0)
\end{equation}
Dapat kita susun menjadi
\begin{equation}
\theta(t)=\theta(t_0)+\dot{\theta}(t)(t-t_0)
\end{equation}

###d. Program C++
#include<iostream>
#include<math.h>
using namespace std;
int main()
{
int i,n;
float l[10],t1[10],t2[10],t[10],r[10],s=0,m,g;
cout<<"Masukkan banyak percobaan yang akan dilakukan : ";
cin>>n;
for(i=0;i<n;i++)
{
cout<<"\nNilai L:";
cin>>l[i];
cout<<"\nNilai T1:";
cin>>t1[i];
cout<<"\nNilai T2:";
cin>>t2[i];
t[i]=(t1[i]+t2[i])/(2*20);
r[i]=l[i]/(pow(t[i],2));
cout<<"\nHasil (L/T^2) ="<<r[i]<<"\n\n";
s=s+r[i];
}
m=s/n;
g=4*pow(3.14,2)*m;
cout<<"\n";
cout<<"\nLength\t\tPeriod\t\t(L/T^2)\n";
for(i=0;i<n;i++)
{
cout<<"\n\n"<<l[i]<<"\t\t"<<t[i]<<"\t\t"<<r[i];    
}
cout<<"\n\nMean value of (L/T^2) is: "<<m;
cout<<"\nAcceleration due to gravity,g: "<<g<<" m/s^2\n\n";
return 0;
}

## Soal 3. Arsitektur Jaringan Syarat Tiruan
###a. Notasi untuk data Tabel 1
Jika data pada tabel 1 dinyatakan dalam grafik sebagai scatter plot maka dapat dilihat hasilnya pada link berikut https://plotly.com/~adnan0997/2/. Agar dapat mengklasifikasikan data tersebut kedalam masing-masing kelasnya dapat digunakan arsitektur JST dengan topologi feedforward dengan dua input layer $N_{1,X_1, N_{1,X_2}$, satu hidden layer $N_{2,1}$, dan satu output layer $N_{3,1}$ Setelah menentukan arsitektur JST dipilih learning rate sebesar 0,01 dan fungsi aktivasi linear. Kedua hal tersebut dapat memengaruhi laju pembobotan fitur input. Kemudian, dilakukan pembelajaran dengan menggunakan sampel yang telah diketahui kelasnya dengan mengubah pembobotan berdasarkan hasil error yang didapatkan dari setiap iterasi dan iterasi dilakukan hingga didapatkan nilai yang konvergen. Dengan batas yang diharapkan berupa garis linear dengan gradien tertentu.
###b. Notasi untuk data Tabel 2
Jika data pada tabel 2 dinyatakan dalam grafik sebagai scatter plot maka dapat dilihat hasilnya pada link berikut https://plotly.com/~adnan0997/4/. Agar dapat mengklasifikasikan data tersebut kedalam masing-masing kelasnya dapat digunakan arsitektur JST dengan topologi feedforward dengan dua input layer $N_{1,X_1}, N_{1,X_2}$, dua hidden layer $N_{2,1}, N_{2,2}$, dan dua output layer $N_{3,1}, N_{3,2}$. Setelah menentukan arsitektur JST dipilih learning rate sebesar 0,01 dan fungsi aktivasi tanh.
###c. Notasi untuk data Tabel 3
Jika data pada tabel 3 dinyatakan dalam grafik sebagai scatter plot maka dapat dilihat hasilnya pada link berikut https://plotly.com/~adnan0997/5/. Agar dapat mengklasifikasikan data tersebut kedalam masing-masing kelasnya dapat digunakan arsitektur JST dengan topologi feedforward dengan tiga input layer $N_{1,X_1, N_{1,X_2},N_{1,X_2^2}$, dua hidden layer $N_{2,1}, N_{2,2}$ serta dua output layer  $N_{3,1}, N_{3,2}$. Setelah menentukan arsitektur JST dipilih learning rate sebesar 0,01 dan fungsi aktivasi sigmoid. Dengan batas yang diharapkan berupa parabola terbuka keatas.

###d. Arsitektur JST yang  sederhana berpengaruh terhadap keefektifan JST untuk mengklasifikasikan data. Dengan mengetahui karakteristik data yang tepat, kita dapat menentukan input layer yang sesuai dan dapat menentukan apakan diperlukan hidden layer atau tidak dan jika karakteristik data kurang dapat menghasilkan hasil yang cukup baik maka kita dapat menambahkan hidden layer sehingga bisa didapatkan karakteristik data tambahan sehingga hasil yang diperoleh lebih baik. Arsitektur JST yang sederhana mungkin dibutuhkan untuk dalam visualisasi sehingga bentuk yang sederhana, kemudian iterasi yang dilakukan tidak begitu lama.

##Soal 4. 
###a. Program yang dibuat adalah dengan menginput kromosom 0010110
main();
// Define main function
function main() {
    var p = "0010110";
    [xs, ys, cs] = getValues(p);
    console.log("p =",p);
    console.log("x =",xs);
    console.log("y =",ys);
    console.log("c =",cs);
}
function getValues() {
    var p = arguments[0];
    var xs = p.slice(0, 3);
    var ys = p.slice(3, 6);
    var cs = p.slice(6);
 
    return [xs, ys, cs];
}
Hasil yang didapat :

###b. program yang dibuat untuk nilai x0 = 111 dan y0 = 111
main();
// Define main function
function main() {
    var p = "1010110";
    [xs, ys, cs] = getValues(p);
    var hasil = 1/(1+fitness(xs,ys));                                              //fungsi utuh fitting
    console.log("p =",p);
    console.log("x =",xs);
    console.log("y =",ys);
    console.log("c =",cs);
    console.log("hasil = ",hasil);
}
 
function getValues() {
    var p = arguments[0];
    var xs = p.slice(0, 3);
    var ys = p.slice(3, 6);
    var cs = p.slice(6);
    return [xs, ys, cs];
}
 
function fitness(a, b) {                                    //fungsi untuk fitting (hanya bagian akar)
  return(Math.sqrt(Math.pow((a - 111), 2) + Math.pow((b - 111),2)));
}
###c. Program yang digunakan yaitu :
main();
 
// Define main function
function main() {
    var p = "1011001";    //menginput kromosom yang diuji
    [xs, ys, cs] = getValues(p);
    var hasil = 1/(1+fitness(xs,ys));
    console.log("p =",p);
    console.log("x =",xs);
    console.log("y =",ys);
    console.log("c =",cs);
    console.log("hasil = ",hasil);
 
}
 
function getValues() {
    var p = arguments[0];
 
    var xs = p.slice(0, 3);
    var ys = p.slice(3, 6);
    var cs = p.slice(6);
 
    return [xs, ys, cs];
}
 
function fitness(a, b) {
  return(Math.sqrt(Math.pow((a - 101), 2) + Math.pow((b - 100),2)));        //mengganti nilai dalam akar untuk kromosom referensi
}
###d. program yang di gunakan sama seperti program (b) dengan nilai x0 = 101 dan y0 = 100.
Kromosom yang akan di-check adalah
·         1111011 , x = 111 dan y = 101
·         1001111 , x = 100 dan y = 111
·         1001001, x = 100 dan y = 100
·         1111111, x = 111 dan y = 111
·         1011001, x = 101 dan y = 100
 
Hasil maksimal yang di dapat yaitu kromosom 1011001 karena sama dengan kromosom threshold dengan fitness 1 dan kromosom yang paling mendekati 1011001 adalah kromoson 1001001 dengan nilai fitness 0,5 dari 5 iterasi yang telah dicoba.

##Soal 5. Tujuan: Menghitung dosis distribusi pada treatment planning system (TPS) untuk Proton Beam Therapy (PBT) dengan cepat dan akurat menggunakan algoritma Monte Carlo.

Rumusan masalah: Terdapat banyak algoritma TPS untuk optimasi PBT, salah satunya adalah algoritma pencil beam. Algoritma pencil beam memiliki keuntungan perhitungan yang cepat yang sangat berguna untuk intensity modulated proton therapy (IMRT). Akan tetapi, akurasi algoritma ini pada dasarnya ditentukan oleh density scaling berkas proton satu dimensi pada water phantom (air) yang merupakan materi yang homogen. Ketidakhomogenan densitas pada tubuh manusia (yang tersusun dari otot, tulang, udara, lemak, dan lain-lain)  menyulitkan perhitungan dosis secara akurat karena multiple Coulomb scattering pada medium homogen (serta reaksi inti secara elastik dan inelastik) menggunakan algoritma pencil beam hanya berupa nilai pendekatan. Oleh karena itu, perlu diperkenalkan metode/algoritma lain yang dapat menghitung distribusi dosis yang jauh lebih akurat, yaitu algoritma Monte Carlo Calculation (MCC). MCC menjadi sangat akurat karena memperhitungkan setiap partikel (proton) yang berinteraksi dengan materi. 

Metode: Secara umum, algoritma Monte Carlo dari transport partikel bermuatan dapat dibagi menjadi 4 langkah:
Memperkirakan jarak (mean free path) partikel dari masing-masing interaksi yang terjadi (absorption and scatter).
Menghitung penampang lintang dan memindahkan partikel dari titik origin ke titik jarak.
Membuat suatu random jarak dan arah sehingga mendapat ????, ????,????.
Melakukan pengulangan hingga partikel berhenti atau seluruh energi partikel terabsorpsi.

Hasil dan diskusi: Untuk treatment planning radioterapi, sebaiknya target (sel kanker atau tumor ganas) mengenai dosis sebesar-besarnya sedangkan jaringan atau organ sekitar yang sehat (organ at risk, OARs) mengenai dosis sekecil-kecilnya untuk meminimalisasi risiko-risiko penyakit lain yang dapat muncul akibat kerusakan pada sel-sel sehat tersebut. Dengan metode MCC ini diharapkan dapat mengurangi risiko tersebut karena dapat mensimulasikan persebaran dosis proton beam dengan lebih akurat dan presisi dibanding dengan metode pencil beam.

Referensi: 
Fippel, Matthias, Martin Soukup. A Monte Carlo dose calculation algorithm for proton therapy. Med. Phys. Vol. 31, No.8 , August 2004. DOI: 10.1118/1.1769631

Robinson, Don. Inhomogeneity correction and the analytic anisotropic algorithm. Journal of Applied Clinical Medical Physics, Vol. 9, No. 2, Spring 2008

