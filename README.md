# AplikasiPertambahanDuaAngka
### 1. Deskripsi Program:
   
   • Pengguna memasukkan dua angka

   • Saat tombol Tambah diklik akan menampilkan hasil pertambahan

   • Saat tombol Hapus diklik akan menghapus nilai di TextField dan
   mengarahkan fokus ke TextField angka pertama

### 2. Komponen GUI: JFrame, JPanel, JLabel, JTextField, JButton

### 3. Logika Program: Penambahan dua angka, validasi input numerik

### 4. Events: ActionListener untuk tombol Tambah, Hapus, dan Keluar
   
#### A.Tambah
```bash
   private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                          
        try {
        double a1 = double.parseInt(angka1.getText());
        double a2 = double.parseInt(angka2.getText());
        double hasil = a1 + a2;
        txtHasil.setText(String.valueOf(hasil));
```

#### B.Hapus
  ```bash
  private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         

        angka1.setText("");
        angka2.setText("");
        phasil.setText("");
        angka1.requestFocus();
    }  
```

#### C.Keluar
  ```bash
  private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {                                          
        System.exit(0);
    }                                         
  ```
### 5. Variasi: 
#### A.Gunakan JOptionPane untuk menampilkan error input
```bash
} catch (NumberFormatException e) {
        JOptionPane.showMessageDialog(this, "Input harus berupa angka!", "Error", JOptionPane.ERROR_MESSAGE);
    }
```
#### B.Implementasikan FocusListener untuk membersihkan JTextField
saat mendapatkan fokus.
```bash
    private void txtAngka1FocusGained(java.awt.event.FocusEvent evt) {                                      
        // TODO add your handling code here:
        angka1.setText("");
    }
```
## Foto Aplikasi Setelah di Run

 ![](https://github.com/M-Irfansyah/AplikasiPertambahanDuaAngka/blob/main/Screenshot%202024-11-04%20102122.png)

## Indikator Penilaian:

| No  | Komponen         |  Persentase  |
| :-: | --------------   |   :-----:    |
|  1  | Komponen GUI     |    20    |
|  2  | Logika Program   |    20    |
|  3  | Kesesuaian UI    |    15    |
|  4  | Constructor      |    15    |
|  5  | Memenuhi Variasi |    30    |
|     | TOTAL        | 100 |

## Pembuat

Nama:M.Irfansyah

NPM :2210010176
