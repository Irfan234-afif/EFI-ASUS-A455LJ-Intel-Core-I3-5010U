# EFI ASUS A455LJ Intel Core I3-5010U




| **Category**   | **Component**                 		
|----------------|--------------------------------------|
|**CPU**		       |Intel Core I3-5010U 2.10 GHz  |										      
|**GPU**		       |Intel HD 5500		     		 										       |
|**DGPU**		       |Nvidia GT 920M			     		 										       |
|**RAM**         |RAM   : 1x 2GB DDR3L   1x 8GB DDR3L              |
|**SDD**         |SSD MidasForce 256 GB SATA III  		                |
|**Layar**       |14 Inch HD LED	1366x768 (biasanya pake 1600x900 biar lega)	 		               |										      
|**Wi-Fi/BT**    |Qualcom atheros AR956x 	   			     		                         | 	  
|**Ethernet**    |Realtek RTL8168/8111 			 		                    |										      
|**Audio** 		   |Conexant CX20751/2					 		                 |
|**Input**       |PS2 Keyboard & Asus PS2 Touchpad |


SUPPORT HIGH SIERRA - BIG SUR. (MONTEREY ADA PERSYARATAN)


**DI REKOMENDASIKAN MOJAVE**

karna MAC OS versi semakin tinggi,semakin di pangkas lagi featurnya


**KENAPA MOJAVE?**

mojave sangat stabil di versi laptop ini, menurut saya. karna segala featur masih di support dan performa sangat pas disini dari mulai GPU dan CPU. 


**KENAPA TIDAK CATALINA?**

sederhana saja, karna banyak rumor yang menyatakan catalina banyak bug dan segala macem, maka dari itu saya tidak pernah mencobanya


-------------------------------------------------------------------------------------------------------------------------------------------------

BIOS Configurator

saya mencoba beberapa pengaturan, dan saya menemukan hal aneh. Berada di pengaturan BIOS-ADVANCED, INTEL VIRTUALIZATION dan INTEL VT-D sebaiknya di non-aktifkan, ini akan mempengaruhi di bagian performa, entah mengapa bisa begitu saya juga tidak tahu, tapi saya telah tes BenchMark untuk itu. Dan ada lagi hal aneh yang terjadi, jika Intel AES-NI ikut ikut di nonaktifkan maka performa ikut menurun lagi saya tidak tahu lagi mengapa, Padahal Intel AES-NI berfungsi untuk Encrypt. saya mencoba mengak-tifkan satu persatu fitur itu, tapi yang terjadi sama saja dengan yang saya katakan tadi, maka saran saya begitu saja, tidak banyak namun berpengaruh di performa sekitar 10-20%


Secure Boot         --|   Disabel   
Intel Virtulization --|   Disable   
Intel VT-D          --|   Disable   
DVMT Pre-Allocation --|   64M / default 32M  
XHCI Pre-Boot Mode  --|   Enabled / Smart Auto jika menggunakan perangkat EHCI   
SATA Mode           --|   AHCI   
Launch CSM          --|   Disable  


________________________________________________________________________________________________________________________________________________

## Pasca-Instalation

- Ganti SMBIOS saran saya gunakan MacBook Air 7,2
- Hapus yang perlu koreksi lagi EFI ini karna tidak ada efi publik yang langsung pakai
- Jika devices sama persis, mungkin bisa langsung pakai


## Post-Instalation

-USB MAPPING
   jika sudah berhasil boot maka yang harus anda lakukan adalah **USB MAPPING** karna saya sering mendengar, hasil usb mapping gampang hilang maka usb mapping lah yang pertama kali anda lakukan

-Tes POWER MANAGEMENT
  tes paling dasar adalah tes sleep,restart, shutdown. dan coba lah buka Intel Power Management dan biarkan laptop jangan digunakan apa apa dan lihat frekuensi nya, apakah naik naik atau stabil di 800 MHz. lakukan lebih mendalam lagi, lihat di dortania jika lebih lengkap nya

-Selalu Update OpenCore dan kext
  karna kext juga penting untuk perbaikan mendasar
