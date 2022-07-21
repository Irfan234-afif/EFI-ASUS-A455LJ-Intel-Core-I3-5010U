# HACKINTOSH ASUS A455LJ Intel Core I3-5010U

## ORIENTASI                                                                                                           
Saya berhasil membuat efi ini dengan bantuan mas abbas atau yang sering di kenal repo github nya "JAEMAN PRATAMA" dan para senior yang lain seperti mas reno mas rara mas bagas, di bimbing dengan baik untuk membuat efi ini terima kasih sebelum nya untuk semua senior hackintosh.                                                                                                                           

Sharing dikit menggunakan hackintosh ini, saya puas menggunakan hackintosh karna fitur yang ditawarkan banyak sekali dan membuat workflow menjadi sangat mudah, namun harus sabar menggunakan hackintosh untuk di awal, karna mengulik-ulik efi tidak mudah, banyak sekali informasi yang harus kita ketahui, dan banyak sekali nanti masalah yang akan di hadapi.                                        

Jika sudah berhasil boot hackintosh jangan sia-sia kan fitur yang di tawarkan, karna itu yang membuat hackintosh sangat berguna, jika fitur fitur saja tidak anda gunakan maka apa bedanya dengan windows.                                                                   

Saya menggunakan metode manual untuk membuat ssdt-plug karna metode ini menurut saya yang pas, CPU dingin kana opini saya menggunakan metode manual itu POWER MANAGEMENT akan di sama kan dengan default pengaturan CPU nya seperti di windows(hanya opini) dan saya sudah mencoba banyak metode pembuatan ssdt-plug namun ini yang menurut saya terbaik jika anda ingin mengganti silahkan

  
<p align="center">
   <img src="https://github.com/Irfan234-afif/EFI-ASUS-A455LJ-Intel-Core-I3-5010U/blob/main/SCREENSHOT/Jepretan%20Layar%202022-07-15%20pukul%2016.57.49.png"
</p>


| **Category**   | **Component**                 		
|----------------|--------------------------------------|
|**CPU**		       |Intel Core I3-5010U 2.10 GHz  |										      
|**GPU**		       |Intel HD 5500		     		 										       |
|**DGPU**		       |Nvidia GT 920M(disable)			     		 										       |
|**RAM**         |RAM   : 1x 2GB DDR3L   1x 8GB DDR3L              |
|**SDD**         |SSD MidasForce 256 GB SATA III  		                |
|**Layar**       |14 Inch HD LED	1366x768 (biasanya pake 1600x900 biar lega)	 		               |										      
|**Wi-Fi/BT**    |Qualcom atheros AR956x 	   			     		                         | 	  
|**Ethernet**    |Realtek RTL8168/8111 			 		                    |										      
|**Audio** 		   |Conexant CX20751/2					 		                 |
|**Input**       |PS2 Keyboard & Asus PS2 Touchpad |



## WORK

- CPU POWER MANAGEMENT
- SHUTDOWN, RESTART, SLEEP
- QE/CI of HD 5500
- ETHERNET
- WIFI
- BLUETOOTH
- AUDIO AND PORT JACK
- HDMI
- ALL USB PORT  

SUPPORT MAC OS  High Sierra - BIG SUR. (MONTEREY Hapus Kext Wifi dan Bluetooth)


**DI REKOMENDASIKAN MOJAVE**



**KENAPA MOJAVE?**

mojave sangat stabil di versi laptop ini, menurut saya. karna segala featur masih di support dan performa sangat pas disini dari mulai GPU dan CPU. 
Namun saya tetap menggunakan bigsur

**KENAPA TIDAK CATALINA?**

karna banyak rumor yang menyatakan catalina banyak bug dan segala macem, maka dari itu saya tidak pernah mencobanya dan beberapa senior di @HACKINTOSH_LOVERS menyarankan untuk mojave


-------------------------------------------------------------------------------------------------------------------------------------------------

## BIOS Configurator

saya mencoba beberapa pengaturan, dan saya menemukan hal aneh. Berada di pengaturan BIOS-ADVANCED, INTEL VIRTUALIZATION dan INTEL VT-D sebaiknya di non-aktifkan, ini akan mempengaruhi di bagian performa, entah mengapa bisa begitu saya juga tidak tahu, tapi saya telah tes BenchMark untuk itu. Dan ada lagi hal aneh yang terjadi, jika Intel AES-NI ikut ikut di nonaktifkan maka performa ikut menurun lagi saya tidak tahu lagi mengapa, Padahal Intel AES-NI berfungsi untuk Encrypt. saya mencoba mengak-tifkan satu persatu fitur itu, tapi yang terjadi sama saja dengan yang saya katakan tadi, maka saran saya begitu saja, tidak banyak namun berpengaruh di performa sekitar 10-20%


Secure Boot         --|--   Disabel   
Intel Virtulization --|--   Disable   
Intel VT-D          --|--   Disable   
DVMT Pre-Allocation --|--   64M / default 32M  
XHCI Pre-Boot Mode  --|--   Enabled / Smart Auto jika menggunakan perangkat EHCI   
SATA Mode           --|--   AHCI   
Launch CSM          --|--   Disable  


________________________________________________________________________________________________________________________________________________

## Pasca-Instalation

- Ganti SMBIOS, saran saya gunakan MacBook Air 7,2
- Hapus yang perlu. koreksi lagi EFI ini karna tidak ada efi publik yang langsung pakai
- Jika devices sama persis, mungkin bisa langsung pakai
- dGPU di non-aktifkan melalui SSDT


## Post-Instalation

**-USB MAPPING**                                                                                                                                 
   jika sudah berhasil boot maka yang harus anda lakukan adalah **USB MAPPING** karna saya sering mendengar, hasil usb mapping gampang hilang maka usb mapping lah yang pertama kali anda lakukan

**-Tes POWER MANAGEMENT**                                                                                                                         
  tes paling dasar adalah tes sleep,restart, shutdown. dan coba lah buka Intel Power Management dan biarkan laptop jangan digunakan apa apa dan lihat frekuensi nya, apakah naik naik atau stabil di 800 MHz. lakukan lebih mendalam lagi, lihat di dortania jika lebih lengkap nya

**-Selalu Update OpenCore dan kext**                                                                                                            
  karna kext juga penting untuk perbaikan mendasar
                                                                                                                                                
                                                                        


## Thanks

- Allah SWT.
- Dortania
- Olarila
- Achidantera
- Hackintosh Lovers
- Hackintosh Indonesia
- Jaemann Pratama
- Achidantera
