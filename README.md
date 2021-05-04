# Kasir
PROJECT UTS APLIKASI KASIR BERBASIS GUI
import java.util.Scanner;
public class Kasir {
    
    public static void main(String[]args) {
    Scanner input = new Scanner(System.in);
    String nama_barang;
    int jumlah_barang, harga, totalharga;
            double diskon = 0.075 ;
            double totalbayar ;
            System.out.println("Program Kasir Sederhana");
            System.out.println("=======================");
            System.out.println("Masukan Data Berikut");
            System.out.println("Nama Barang");
            nama_barang = input.nextLine();
            
            System.out.println("Jumlah Barang = ");
            jumlah_barang = input.nextInt();
            if (jumlah_barang <= 0){
                
            System.out.println("mohon masukan jumlah yang benar dan ulangi program");
            System.exit(0);
            }
            System.out.println("Harga Barang = Rp");
            harga = input.nextInt();
            if (harga <100)
            {
                System.out.println("mohon masukan harga yang valid dan ulangi");
                System.exit(0);
            }
            System.out.println("Anda Mendapatkan Diskon 7,5%");
            totalharga = jumlah_barang * harga;
            System.out.println("Total harga = Rp" +totalharga);
            diskon = totalharga * diskon;
            totalbayar = totalharga - diskon;
            System.out.println("Total bayar = Rp +totalbayar");
            System.out.println("============================");
            System.out.println("Nota Belanja");
            System.out.println("Nama Barang =" +nama_barang);
            System.out.println("Jumlah Barang =" +jumlah_barang);
            System.out.println("Harga Barang Rp=" +harga);
            System.out.println("Total Harga Rp=" +totalharga);
            System.out.println("Total Bayar Rp=" +totalbayar);
            System.out.println("===========================");
            
            
            
                
 }
}
