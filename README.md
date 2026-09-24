
// NIM : 1124160036
// NAMA : FELISSA VIVIAN MARGARETHA

```dart
import 'package:flutter/material.dart';

void main() {
  print("Hello world");
  print('Hello world');
  String makanan = ('TAHOOOO BULAT');
  print (makanan) ;
   //nilai ini sudah ditetapkan dengan String
  
  int nilai = (90);
  print (nilai);
  //nilai ini sudah ditetapkan dengan int
  
  double nilai2 = (90.5);
  print (nilai2);
  //nilai ini sudah ditetapkan dengan double
  
  String? namaawal ;
  namaawal = "Felissa";
  print (namaawal);
  //nilai ini belum ditetapkan dan di null kan
  
  namaawal = null ;
  
  String gantinama = namaawal ?? "Vivian";
  print (gantinama);
  
    //////////////////// TIPE DATA //////////////////////
  
   // Tipe String Kumpulan karakter seperti huruf, kata, kalimat, atau angka yang dianggap sebagai teks.
  String name = 'joko';
  String id = '192877743';
  
  print (name.toUpperCase ());
  print(id);
  
    Map<String, dynamic> user = {
    'name': 'joko',
    'id': '192877743',
  };

  // Mengambil ISI dari key 'name' dan 'id' di dalam Map
  print("ini ${user['name']} dengan id ${user['id']}"); 
  // Output: ini joko dengan id 192877743

  // Dipakai juga kalau mau pakai method seperti .toUpperCase()
  print("ini ${name.toUpperCase()}"); 
  // Output: ini JOKO
  
  // Tipe int ini bisa nampung nilai yang tipe datanya int yang bisa di operasi matematika, dan hanya bisa menampung bilangan bulat
  int sisi = 20 ;
  int square = sisi * 4;

  print (square);
  Text('luas square: $square');
  
  double berat = 2.5;
  print (berat);
  
  double beratBadan = 2.5;
  Text('Berat: $beratBadan kg');
  
  
// Tipe Num ini bisa nampung nilai yang tipe datanya int maupun double
    num angka = 10;
    num angkaKoma = 10.5;

    print('ini bilangan bulat : $angka dan ini bilangan desimal :         $angkaKoma');
  
// Tipe data Bool
  
  bool sudahLogin = true;
  bool notifikasiAktif = false;
  
  bool isLoading = true ;
  
// @override
// Widget build(BuildContext context) {
//   return isLoading
//       ? const CircularProgressIndicator() // Jika loading (true)
//       : const Text('Data berhasil dimuat'); // Jika tidak loading (false)

  
  /////////////////////// LIST DATA ///////////////////
  
  List<String> namaTemanku = [
  "Asha",
  "Febry ",
  "Gavin"
];
  
  print (namaTemanku [0]);
  print (namaTemanku [1]);
  namaTemanku.add('Dewi');
  print (namaTemanku [3]);


 Set<String> menu = {
    'Tempe Orek',
    'Sayur Asem',
    'Tahu Bacem'
  };
  //
  print (menu);
  namaTemanku.add('Usus');
  namaTemanku.add('Tehu Bacem');
  print (menu);
  
  //Nilai Tahu Bacem hanya akan tersimpan sekali.
  
  Map<String, dynamic> hewan = {
    'name' : 'bombom', 
    'skin' : 'Orange',
    'age' : '4 tahun',
    'ras' : 'kampung'
  };
  
  print(hewan['name']); // bombom
  print(hewan['age']); // 4 tahun
  
   Map<String, dynamic> produkJson = {
  'id': 10,
  'nama': 'Tahu Bacem',
  'harga': '${5000} per/pcs',
  'tersedia': true,
  };
  
  print(produkJson['id']); 
  print(produkJson['nama']); 
  
  // Contoh menampilkan data produk ke widget UI
  Card(
    child: ListTile(
      title: Text(produkJson['nama']), // Menampilkan "Tahu Bacem"
      subtitle: Text('Rp ${produkJson['harga']}'), // Menampilkan "Rp 5000"
      trailing: Icon(
        produkJson['tersedia'] ? Icons.check_circle : Icons.cancel,
        color: produkJson['tersedia'] ? Colors.green : Colors.red,
      ),
    ),
  );
  
  //object ini bisa di timpe berkali2 nilainya. Gunakan Object ketika sebuah nilai dapat memiliki beberapa tipe,
  Object data ='Felissa';
  data = 20;
  data = true;
  
  if (data is String)
  {
    print(data.toUpperCase ());
  }
  
  dynamic keterangan = 'Budi';
  keterangan = 20;
  keterangan = true;
  

  print(keterangan.toUpperCase());
  
  

  
}


,,,
