public class Persegi {
        private double sisi;

        public double getSisi() {
            return sisi;
        }

        public void setSisi(double sisi) {
            this.sisi = sisi;
        }

        public double hitungKeliling() {
            return 4 * sisi;
        }

        public double hitungLuas() {
            return sisi * sisi;
        }
    }

    class PersegiPanjang {
        private double panjang;
        private double lebar;

        public double getPanjang() {
            return panjang;
        }

        public void setPanjang(double panjang) {
            this.panjang = panjang;
        }

        public double getLebar() {
            return lebar;
        }

        public void setLebar(double lebar) {
            this.lebar = lebar;
        }

        public double hitungKeliling() {
            return 2 * (panjang + lebar);
        }

        public double hitungLuas() {
            return panjang * lebar;
        }
    }

    class Tester {
        public static void main(String[] args) {
            Persegi persegi = new Persegi();
            PersegiPanjang persegiPanjang = new PersegiPanjang();

            // Mengatur nilai sisi pada objek Persegi
            persegi.setSisi(5.0);

            // Mengatur nilai panjang dan lebar pada objek PersegiPanjang
            persegiPanjang.setPanjang(7.0);
            persegiPanjang.setLebar(4.0);

            // Menghitung keliling dan luas dari Persegi
            double kelilingPersegi = persegi.hitungKeliling();
            double luasPersegi = persegi.hitungLuas();

            // Menghitung keliling dan luas dari PersegiPanjang
            double kelilingPersegiPanjang = persegiPanjang.hitungKeliling();
            double luasPersegiPanjang = persegiPanjang.hitungLuas();

            // Menampilkan hasil perhitungan ke layar
            System.out.println("Persegi:");
            System.out.println("Sisi: " + persegi.getSisi());
            System.out.println("Keliling: " + kelilingPersegi);
            System.out.println("Luas: " + luasPersegi);

            System.out.println("\nPersegi Panjang:");
            System.out.println("Panjang: " + persegiPanjang.getPanjang());
            System.out.println("Lebar: " + persegiPanjang.getLebar());
            System.out.println("Keliling: " + kelilingPersegiPanjang);
            System.out.println("Luas: " + luasPersegiPanjang);
        }
}
