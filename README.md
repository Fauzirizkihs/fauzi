import java.util.Scanner;

public class ArrayMahasiswa {

    public static void main(String[] args) {

        int jumlahMahasiswa;
        String[] namaMahasiswa;
        int[] umurMahasiswa;

        Scanner input = new Scanner(System.in);
        System.out.print("Masukan jumlah mahasiswa: ");
        jumlahMahasiswa = input.nextInt();

        namaMahasiswa = new String[jumlahMahasiswa];
        umurMahasiswa = new int[jumlahMahasiswa];

        for (int i = 0; i < jumlahMahasiswa; i++) {
            System.out.print("Nama mahasiswa ke-" + (i + 1) + ": ");
            namaMahasiswa[i] = input.next();

            System.out.print("Umur mahasiswa ke-" + (i + 1) + ": ");
            umurMahasiswa[i] = input.nextInt();
        }

        System.out.println("===Data Mahasiswa===");
        for (int i = 0; i < jumlahMahasiswa; i++) {
            System.out.println("Nama: " + namaMahasiswa[i] + ", Umur: " + umurMahasiswa[i]);
        }
    }
}
