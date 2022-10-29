# CI Codemagic flutter-expert-project-main1 
https://api.codemagic.io/apps/6358ac1f123c0e33df4ea2fd/6358ac1f123c0e33df4ea2fc/status_badge.svg
    Preparing build machine             41s
    Fetching app sources                2s
    Installing dependencies             46s
    Building Android                    1m 20s
    Building iOS                        1m 34s
    Publishing                          8s
    Cleaning up                         < 1s

# Build overview
    ID          : 635a7ea66520fbea0bb45707
    Index       : 5
    Status      : finished
    Workflow    : Default Workflow
    Started     : a day ago Oct 27th, 2022 at 20:01 WIB
    Duration    : 4m 32s
    Machine     : Mac mini M1
    Branch      : master
    Commit      : 90ab88b

# Artifacts
    app-debug.aab [185.70 MB]
    Runner.app.zip [91.85 MB]

# Current configuration
    Flutter channel: default
    Mode: release
    Xcode version: 14.0.1
    Build for: Android & iOS
    
https://codemagic.io/app/635a702e6520fb0c6301515f/build/635a7ea66520fbea0bb45707
![image](https://user-images.githubusercontent.com/111186324/198293649-31daec62-3d57-4d43-9f7d-148dfd858012.png)

# a199-flutter-expert-project

Repository ini merupakan starter project submission kelas Flutter Expert Dicoding Indonesia.

---

## Tips Submission Awal

Pastikan untuk memeriksa kembali seluruh hasil testing pada submissionmu sebelum dikirimkan. Karena kriteria pada submission ini akan diperiksa setelah seluruh berkas testing berhasil dijalankan.


## Tips Submission Akhir

Jika kamu menerapkan modular pada project, Anda dapat memanfaatkan berkas `test.sh` pada repository ini. Berkas tersebut dapat mempermudah proses testing melalui *terminal* atau *command prompt*. Sebelumnya menjalankan berkas tersebut, ikuti beberapa langkah berikut:
1. Install terlebih dahulu aplikasi sesuai dengan Operating System (OS) yang Anda gunakan.
    - Bagi pengguna **Linux**, jalankan perintah berikut pada terminal.
        ```
        sudo apt-get update -qq -y
        sudo apt-get install lcov -y
        ```
    
    - Bagi pengguna **Mac**, jalankan perintah berikut pada terminal.
        ```
        brew install lcov
        ```
    - Bagi pengguna **Windows**, ikuti langkah berikut.
        - Install [Chocolatey](https://chocolatey.org/install) pada komputermu.
        - Setelah berhasil, install [lcov](https://community.chocolatey.org/packages/lcov) dengan menjalankan perintah berikut.
            ```
            choco install lcov
            ```
        - Kemudian cek **Environtment Variabel** pada kolom **System variabels** terdapat variabel GENTHTML dan LCOV_HOME. Jika tidak tersedia, Anda bisa menambahkan variabel baru dengan nilai seperti berikut.
            | Variable | Value|
            | ----------- | ----------- |
            | GENTHTML | C:\ProgramData\chocolatey\lib\lcov\tools\bin\genhtml |
            | LCOV_HOME | C:\ProgramData\chocolatey\lib\lcov\tools |
        
2. Untuk mempermudah proses verifikasi testing, jalankan perintah berikut.
    ```
    git init
    ```
3. Kemudian jalankan berkas `test.sh` dengan perintah berikut pada *terminal* atau *powershell*.
    ```
    test.sh
    ```
    atau
    ```
    ./test.sh
    ```
    Proses ini akan men-*generate* berkas `lcov.info` dan folder `coverage` terkait dengan laporan coverage.
4. Tunggu proses testing selesai hingga muncul web terkait laporan coverage.

