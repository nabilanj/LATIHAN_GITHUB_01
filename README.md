**TUTORIAL PEMBUATAN REPOSITORY LOCAL DAN PEMBUATAN FILE README.md MENGGUNAKAN GIT**

**LANGKAH - LANGKAH**

**1. Install Git versi WINDOWS**
   - Melalui website resmi Git di *https://git-scm.com*, dengan ketentuan arsitektur komputer kita. Jika 32 Bit pilih dan unduh 32 bit        Git for Windows setup, begitupula sebaliknya jika 64 Bit pilih dan unduh 64 bit Git for Windows setup (Pastikan komputer Anda            terkoneksi jaringan internet).
     ![Screenshot (62)](https://user-images.githubusercontent.com/57028453/67616591-fd9d1a80-f804-11e9-8c83-e16b56988466.png)
     
   - Buka Setup git yang sudah di unduh tadi, ikuti saja intruksi (Klik Next terus) dan pastikan folder git terpasang sesuai lokasi          yang Anda inginkan, setelah itu tinggal next saja sampai proses download selesai. (Cara ini untuk yang tak berbayar atau Free)
     ![Screenshot (7)](https://user-images.githubusercontent.com/57028453/67617006-04c62780-f809-11e9-979e-cfac7b014a27.png)
     
     (Proses Instalasi telah selesai)
     
     ![Screenshot (42)](https://user-images.githubusercontent.com/57028453/67624828-2f8f9a80-f860-11e9-80d5-0bd73dd6af46.png)

   - Jika proses install telah selesai, untuk memastikan telah terinstal di komputer Anda, cobalah dengan cara buka CMD/ PowerShell          melalui **W + R** atau pun search *"CMD"* di Windows Explore. Setelah itu ketik perintah *"git --version"* lalu enter, jika versi        telah muncul maka git sudah terpasang dan dapat digunakan.
   
      ![Screenshot (43)](https://user-images.githubusercontent.com/57028453/67617588-bae04000-f80e-11e9-8f37-1bd1f5acb320.png)

**2. SIGN UP** 
   - Sebelum pembuatan Repository sebaiknya sign up terlebih dahulu di *https://github.com/* , lalu isi username, email Anda dan isi          password (Pastikan password terdapat huruf dan angka)
![Screenshot (12)](https://user-images.githubusercontent.com/57028453/67616801-47870000-f807-11e9-80e1-94187f9046f4.png)

   - Jangan lupa untuk verifikasi email yang sudah dikirim ke email Anda. Lalu Anda akan dialihkan ke laman *GitHub* untuk membuat            Repository Baru.
![Screenshot (63)](https://user-images.githubusercontent.com/57028453/67617553-591fd600-f80e-11e9-879d-2a63c958d7db.png)

**3. PEMBUATAN REPOSITORY LOKAL**
   - Sebelum membuat repository pada laman *github*. Buka direktory aktif dengan search git pada *Windows Explore* atau klik kanan            sembarang di tampilan dekstop ataupun di Folder yang sudah kalian tentukan.
![Screenshot (44)](https://user-images.githubusercontent.com/57028453/67617438-625c7300-f80d-11e9-850b-8b1315c28753.png)

   - Lalu pilih menu **"Git Bash Here"**, sehingga muncul *Git Bash Commad*. 
![Screenshot (47)](https://user-images.githubusercontent.com/57028453/67617487-cd0dae80-f80d-11e9-95a5-023804aaaef7.png)
(Jangan lupa untuk Klik Enter setelah melakukan perintah agar mengetahui hasilnya error atau tidaknya).

   - Saat pertama kali menggunakan git, perlu dilakukan *"Global Config"* atau konfigurasi *"user.name"* dan *"user.email"*. Apabila          belum melakukan konfigurasi bisa terjadi kegagalan saat menjalankan perintan "git commit". Dengan perintah sebagai berikut ;
   
     ***$ git config --global user.name "username"***
     
     ***$ git config --global user.email "email"***
     
        ![Screenshot (48)](https://user-images.githubusercontent.com/57028453/67617782-f845cd00-f810-11e9-923f-ca1738987516.png)
        
   - Setelah melakukan global config, lanjutkan dengan membuat direktory project yang akan kalian buat, misal: **GitHub01**
     dengan perintah ***$ mkdir GitHub01*** dan ***$ cd GitHub01*** . (Nama tidak boleh sama dengan project yang pernah dibuat).
     
      ![mkdir2](https://user-images.githubusercontent.com/57028453/67624171-8ba1f100-f857-11e9-9280-5f4ee619b212.png)
   
   - Setelah itu, jalankan perintah **"git init"**, yaitu untuk membuat repository baru.
      ![init2](https://user-images.githubusercontent.com/57028453/67624232-12ef6480-f858-11e9-9042-2a2ea4506533.png)
      
        (Jika Repository baru berhasil di inisialisasi, maka terbentuklah satu direktori hidden dengan nama ***".git"***).
 
   - Lalu jalankan perintah berikutnya untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif          (Repository). Dan disini kita akan buat satu file bernama README.md (text file). Dengan perintah :
   
     ***$ echo "#Nama_Project" >> README.md*** dan untuk melihat file ketik perintah ***$ ls -l*** .  
     ![echo](https://user-images.githubusercontent.com/57028453/67624242-534ee280-f858-11e9-90b8-3198beb31a27.png)
     
        (File README.md berhasil dibuat).
   
   - Lalu untuk menambahkan file yang baru saja dibuat bisa menggunakan printah **"git add"** dengan format :
   
       ***$ git add README.md***
     
     ![add2](https://user-images.githubusercontent.com/57028453/67624309-36ff7580-f859-11e9-8231-819fb3229ee6.png)
     
     (File README.md berhasil ditambahkan dan jika salah memasukkan perintah dan terjadi eror, bisa dilakukan kembali).
     
   - Setelah itu, untuk menyimpan perubahan yang ada kedalaman database reposit lokal, bisa menggunakan perintah  ;
   
     ***$ git commit -m "komentar commit"*** (misal nama komentar "File Pertama Saya")
   
       ![comit](https://user-images.githubusercontent.com/57028453/67624322-5c8c7f00-f859-11e9-8cb6-93c9f2dd957c.png)

        (Perubahan berhasil disimpan).
        
   - Kemudian, menambahkan remote repository untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses banyak user.
     berikut perintahnya : ***$ git remote add origin [URL]***
     
     (URL bisa didapatkan saat melakukan Repository Server).
       
      *Berikut cara untuk mengetahui URL Anda :*    
      **PEMBUATAN REPOSITORY SERVER**
        - Buat Repository Server, dengan menggunakan laman github ***https://github.com***
   
          Jika belum membuat akun buatlah Akun terlebih dahulu. Caranya ada diatas number ***"2. SIGN UP"***. Jika sudah mempunyai akun           Anda bisa Sign in. Sehabis itu Anda bisa klik ***Start a Project*** atau dari menu icon **( + )** di pojok kanan atas, lalu             pilih ***New Repository***.
          ![Screenshot (49)](https://user-images.githubusercontent.com/57028453/67618897-5d082400-f81f-11e9-9403-041316ff767b.png)
     
        - Setelah itu, isi **Nama Repository** dan **Description** sesuai keinginan Anda , misal : **LATIHAN_GITHUB_01** . Lalu klik               ***"Create Repository"***.
          ![Screenshot (65)](https://user-images.githubusercontent.com/57028453/67618966-3d253000-f820-11e9-8186-3078c7d8a52f.png)
   
        - Selanjutnya, akan muncul repository baru atau laman seperti gambar dibawah. Lalu copy URL tersebut untuk melanjutkan                   perintah repository lokal di ***Git Bash Commad***.
          ![http](https://user-images.githubusercontent.com/57028453/67624457-002a5f00-f85b-11e9-9957-7c7e3217fd47.png)
         
        - URL tersebut digunakan untuk perintah **Remote Repository**. Berikut perintahnya : ***$ git remote add origin [URL]***
          contoh hasil :
          
          ![remote](https://user-images.githubusercontent.com/57028453/67624331-80e85b80-f859-11e9-8251-53424920cb58.png)
        
   
   **KEMBALI KE REPOSITORY LOCAL** atau **GIT BASH COMMAD**
   - Setelah menambahkan remote repository, selanjutnya lakukan **PUSH** (mengirim perubahan ke server). Untuk mengirim perubahan dari        repository local ke reposiroty server bisa menggunakan perintah ***"git push"***.
   
     ***$ git push -u origin master***
     
      ![pus](https://user-images.githubusercontent.com/57028453/67624695-230a4280-f85e-11e9-99db-1deced617ed0.png)
    
   - Kemudian perintah itu akan meninta memasukkan **Username** dan **Password** pada ada akun ***github.com***. 
   ![login](https://user-images.githubusercontent.com/57028453/67624701-37e6d600-f85e-11e9-9a09-9c7d7103e4f5.png)
   
   - Selanjutnya, melakukan **Clone Repository** digunakan untuk chekout repository atau pada dasarnya yaitu meng-copy repository server      dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya ***(Working Directory)***.
     Untuk melakukan cloning bisa menggunakan perintah ***git Clone [URL]***. Untuk mengetahui URL bisa menggunakan URL pada perintah        **Remote Repository** karna sama saja atau URL bisa dicopy dari ***clone or download*** klik, lalu akan muncul URL dari file            tersebut.
     ![cloneee](https://user-images.githubusercontent.com/57028453/67625292-6ff21700-f866-11e9-842d-91b9a6f8aefa.png)
   
   - Setelah log in, untuk melihat hasilnya pada server repository buka kembali laman baru ****https://github.com*** .
     Arahkan pada repositorinya misal : **nabilanj/LATIHAN_GITHUB_01**
     
     ![pojok](https://user-images.githubusercontent.com/57028453/67625386-dcb9e100-f867-11e9-8a0c-cb7f3084c607.png)
   
   - Repository Anda sudah bisa digunakan. Klik pada menu pada lingkaran merah dan Anda bisa membuat project di file README.md tersebut. 
     ![bbb](https://user-images.githubusercontent.com/57028453/67625400-10950680-f868-11e9-8a8f-76cca54b5258.png)
     
     (File README.md sudah bisa di edit)
     ![read](https://user-images.githubusercontent.com/57028453/67625471-d710cb00-f868-11e9-830b-62588585aed3.png)
     


***THANKS FOR READING***



<< ***TUGAS BAHASA PEMOGRAMAN\\Dosen Agung Nugroho,S.Kom.*** >>
