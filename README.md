# GUI
# Aplikasi Konversi RGB to layer RED GREEN BLUE
~~~
Nama   = Endrik
NIM    = 311910088
Mata Kuliah : Pengolah Citra TI.19.C1
Program Studi : Teknik Informatika
Dosen Pengampu : Muhammad Najamuddin Dwi Miharja, M.Kom
Kelas  = TI.19.C.1
Universitas Pelita Bangsa
~~~
# Buat program GUI untuk konversi citra rgb ke layer red, green, blue
Ini langkah- langkahnya :
## 1. Buka aplkasi matlab
## 2. New Script
## 3. Ketik guide > enter >create New > Blank Gui > Simpan difolder yang kalian inginkan.

![x2](https://user-images.githubusercontent.com/81820421/117172209-c7772880-adf5-11eb-8da8-6be49063b0dd.JPG)
## 4. Nanti muncul tampilan GUI
![x3](https://user-images.githubusercontent.com/81820421/117172216-c940ec00-adf5-11eb-9170-84ddb1a1054e.JPG)

## 5. Buatlah layout GUI interface sesuka kalian, saya buat seperti ini.
 ![1](https://user-images.githubusercontent.com/81820421/117172703-40768000-adf6-11eb-8d63-8f573ae2b0bf.JPG)

## Setelah itu masukan sourcode nya . 
~~~
[filename, pathname] = uigetfile({'*.jpg','*.png'});
gambar1 = imread([pathname,filename]);

%menampilkan di axes1
axes(handles.axes1);
imshow(gambar1);

%menampilkan di axes2
red = gambar1(:,:,1);
a = zeros(size(gambar1, 1), size(gambar1, 2));
redOnly = cat(3, red, a, a);
axes(handles.axes2);
imshow(redOnly)
%menampilkan di axes4
green = gambar1(:,:,2);
a = zeros(size(gambar1, 1), size(gambar1, 2));
greenOnly = cat(3, a, green, a);
axes(handles.axes4);
imshow(greenOnly)

%menampilkan di axes5
blue = gambar1(:,:,3);
a = zeros(size(gambar1, 1), size(gambar1, 2));
blueOnly = cat(3, a, a, blue);
axes(handles.axes5);
imshow(blueOnly)
~~~
![22](https://user-images.githubusercontent.com/81820421/117173231-c5619980-adf6-11eb-93c0-e1538f53a74f.JPG)
## Setelah diinput sourcode nya , Aplikasi GUI kita bisa di operasikan dengan klik run .
Nanti akan muncul seperti ini .
![1](https://user-images.githubusercontent.com/81820421/117173424-f5a93800-adf6-11eb-9833-47a10380c37f.JPG)
##  Selanjutnya Pilih gambar yang ada dikomputer foto apa saja yang kalian suka .
Setelah itu aplikasi bekerja akan mengubah foto menjadi konversi yang diubah.

![23](https://user-images.githubusercontent.com/81820421/117173818-589acf00-adf7-11eb-8346-74f430f6e9fb.JPG)


