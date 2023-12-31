# SIDEKAL : Sistem deteksi kandungan logam & non logam pada proses pengemasan makanan

## Project Description
 Sistem Deteksi Kandungan Logam dan Non-logam (SIDEKAL) dalam proses pengemasan makanan adalah teknologi vital yang digunakan dalam industri makanan untuk memastikan keamanan produk sebelum didistribusikan ke konsumen. SIDEKAL menjadi krusial karena potensi terjadinya kontaminasi logam pada produk makanan selama proses produksi itu sangat besar. SIDEKAL diintegrasikan dengan memanfaatkan Programmable Logic Controller(PLC) dimana sistem dirancang menggunakan konveyor otomatis yang dilengkapi dengan sensor canggih untuk mengidentifikasi keberadaan logam atau non-logam dalam produk makanan pada tahap pengemasan. Hal ini bertujuan untuk memastikan produk yang diproduksi bebas dari kontaminasi sebelum mencapai tangan konsumen.
 
## Contributor
| Full Name | Affiliation | Email | Role |
| --- | --- | --- | --- |
| Edy Fitriyanto | Ahmad Dahlan University | edy2100022030@webmail.uad.ac.id | Team Lead |
| Chalda Bhakti Jelika | Ahmad Dahlan University| chalda2115022030@webmailuad.ac.id | Team Member|
| Haris Imam Karim Fathurrahman, S.Pd., M.Sc.| lecturer Ahmad Dahlan University | haris.fathurrahman@te.uad.ac.id | lecturer |

## Setup
### Prerequisite Packages (Dependencies)
- CX-Programmer Omron
- CX-Designer 

example Display HMI :
The Team
![Tampilan Awal](https://github.com/Edyfitriyanto12/Sidekal/blob/main/the%20team.jpeg)
Manual Mode
![Tampilan Awal](https://github.com/Edyfitriyanto12/Sidekal/blob/main/Manual%20Mode.jpeg)
Otomatis Mode
![Tampilan Awal](https://github.com/Edyfitriyanto12/Sidekal/blob/main/Otomatis%20mode.jpeg)

## Cara keja
### Mode manual
terdapat tampilan 3 konveyor, 2 sensor (sensor logam dan non logam) dan 2 buah robot pemindah barang. 
- tekan push button start yang mana sistem akan standby untuk mengghidupkan ke 3 konveyor tsb. 
- jika switch M1 sekali tekan maka konveyor 1 akan hidup, switch M2 sekali tekan maka konveyor 2 akan hidup, dan switch 3 sekali tekan maka konveyor 3 akan hidup. 
- selanjutnya kedua robot akan bekerja dengan memenfaatkan deteksi dari kedua sensor masing masing. dimana jika sensor logam mendeteksi barang logam, maka robot 1 akan bekerja memindahkan barang ke konveyor 2 dan jika sensor logam tidak mendeteksi dan barang terdeteksi sensor non logam maka robot 2 akan bekerja untuk memindahkan ke konveyor 3
  
### Mode Otomatis
- Tekan tombol start dan sistem akan standby untuk bekerja.
- jika sensor masuk mendeteksi barang maka konveyor 1 secara otomatis on sampai menuju sensor logam dan non logam. 
- jika sensor logam mendeteksi maka robot akan bekerja selama 10 detik untuk memindahkan barang, setelah robot bekerja dilanjutkan dengan konveyor 2 ON untuk membawa sampai sensor output mendeteksi barang logam tersebut.
- kemudian pada sistem sensor non logam mendeteksi maka robot akan bekerja selama 10 detik untuk memindahkan barang, 
- setelah robot bekerja dilanjutkan dengan konveyor 3 on untuk membawa sampai sensor output mendeteksi barang non logam tersebut. 

## References
Provide all links that support this final project, i.e., papers, GitHub repositories, websites, etc.
- 
## How to Cite
If you find this project useful, we'd grateful if you cite this repository:
```
@article{
...
}
```

## License
For academic and non-commercial use only.

## Acknowledgement
This project entitled <b>"YOUR PROJECT TITLE HERE"</b> is supported and funded by Startup Campus Indonesia and Indonesian Ministry of Education and Culture through the "**Kampus Merdeka: Magang dan Studi Independen Bersertifikasi (MSIB)**" program.
