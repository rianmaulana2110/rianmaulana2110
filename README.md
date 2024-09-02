import locale


# mendefenisikan kelas barang
class barang:
    # kosntuktor untuk inisialisasi objek barang
    def __inti__(self, nama, harga):
        self.nama = nama # menyimpan nama barang
        self.harga = harga # menyimpan harga barang

# metode untuk mendapatkan nama barang
def get_nama(self):
    return self.nama

# metode untuk mendapatkan nama harga
def get_harga(self):
    return self.harga

# mendefenisikan kelas transaksi
class  transaksi:
    # kontributor untuk inisialisasi objek tansaksi 
    def __inti__(self, barang, jumlah):
        self.barang = barang # menyimpan objek barang yang terlibat dalam transaksi
        self.jumlah = jumlah # penyimpanan jumlah barang yang dibeli
        self.total = self.hitung_total() # megnhitung total harga transaksi

# metode untuk menghitung total harga transaksi
def hitung_total(self):
    return self.barang.get_harga() * self.jumlah #total harga = harga barang * jumlah barang

# metode untuk mendapatkan informasi transaksi
def get_info(self):
    return f"barang: {self.barang.get_nama()}, harga:{self.barang.get_harga()}, jumalah: {self.jumlah}, total: {self.total}"

# mebuat objek barang
barang1 = barang("laptop dell", 1300000) #objek barang1 dengan nama "laptop" dan harga 1000
barang2 = barang("HP Asus", 500000) #objek barang2 dengan nama "HP" dan haga 500

# mekakukan transaksi pembelian
transaksi1 = transaksi(barang1, 2) # objek transasi1 dengan barang1 (laptop) dan jumlah 2
transaksi1 = transaksi(barang1, 3) # objek transasi2 dengan barang1 (HP) dan jumlah 1

# menampilkan informasi transaksi
print("transaksi 1:", transaksi1.get_info()) # menampilkan informasi transaksi1
print("transaksi 2:", transaksi2.get_info()) # menampilkan informasi transaksi12
