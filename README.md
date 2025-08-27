# LAB-47-FIREWALL-NAT
tanggal 27 agustus 2025

# Network Address Translation
Network address translation (nat) adalah proses mengubah alamat IP pada paket data saat paket tersebut melewati router atau firewall, agar bisa dikirim dengan benar antara jaringan privat (LAN) dan jaringan publik (seperti internet). serta bertujuan Menghubungkan jaringan lokal (IP privat) ke internet dan Menjaga keamanan jaringan internal. di firewall nat ini ada 2 chain utama yaitu :

**1. srcnat**     
yang berfungsi untuk mengubah alamat IP sumber (source address) dari paket data yang keluar dari jaringan privat ke jaringan publik (internet). 
**2. dstnat**     
(Destination Network Address Translation) adalah yang mengubah alamat IP tujuan (destination address) dari sebuah paket data. Fungsinya adalah untuk membuat server atau host dalam jaringan lokal dapat diakses dari luar jaringan (internet), misalnya melalui port forwarding.

**berikut beberapa action yang ada di firewal nat:** 

*1. masquerade*    
   digunakan untuk mengubah alamat IP privat di jaringan lokal menjadi satu alamat IP publik secara otomatis, cocok untuk ip yang dinamis/berubah ubah   
*2. same*    
   Mengubah IP sumber (source IP) seperti src-nat, tapi dengan upaya menjaga konsistensi pemetaan antara IP privat dan IP publik. Menjaga agar IP privat tertentu selalu diterjemahkan ke IP publik yang sama (jika ada lebih dari satu IP publik/ ip yang berubah ubah). serta Mencegah perubahan IP NAT (mapping) secara acak.      
*3. src-nat*    
   Mengganti alamat sumber/port paket ke nilai yang ditentukan (to-addresses, to-ports). Biasanya untuk menerjemahkan IP privat ke IP publik tertentu (static srcnat).    
*4. dst-nat*     
   
*5. accept*   

*6. redirect*    

*7. jump*     

*8. return*     

*9. passthrough*      

*10. add dst to address list*     

*11. add src to address list*    

*12. log*     

*13. netmap*      
