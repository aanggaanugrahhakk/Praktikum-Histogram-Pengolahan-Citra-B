
# Histogram

Histogram pengolahan citra adalah representasi grafik yang menyatakan distribusi intensitas piksel pada citra digital.

Library yang digunakan:

- matplotlib.pyplot: Library ini digunakan untuk membuat visualisasi seperti plot, histogram, dan gambar. Library ini biasanya digunakan dalam analisis data dan penelitian ilmiah.
- numpy: Library ini digunakan untuk komputasi numerik dalam Python. Library ini menyediakan dukungan untuk array dan matriks multi-dimensi yang besar, serta koleksi fungsi matematika yang besar untuk beroperasi pada array ini.
- cv2: Ini adalah library OpenCV, yang merupakan library visi komputer populer yang digunakan untuk pemrosesan gambar dan video. Library ini menyediakan berbagai fungsi untuk manipulasi gambar, deteksi fitur, pengenalan objek, dan banyak lagi.
- skimage: Ini adalah library skimage, yang merupakan kumpulan algoritme untuk pemrosesan gambar. Ini menyediakan fungsi untuk pemfilteran gambar, segmentasi, ekstraksi fitur, dan banyak lagi.

Penjelasan penyelesaian Histogram yang digunakan di skrip:

- Mengimpor library: Skrip dimulai dengan mengimpor library yang diperlukan untuk pemrosesan dan visualisasi gambar, termasuk matplotlib.pyplot, numpy, cv2, dan skimage.
- Membaca dan menampilkan gambar: Skrip membaca gambar bernama "citra_medis1.jpg" menggunakan fungsi imread dari skimage.io. Bentuk gambar dicetak menggunakan atribut shape dari array gambar. Gambar tersebut kemudian ditampilkan menggunakan fungsi imshow dari matplotlib.pyplot.
- Menerapkan filter: Kernel didefinisikan sebagai matriks 3x3, dan fungsi filter2D dari cv2 digunakan untuk menerapkan kernel ke gambar input. Gambar yang dihasilkan disimpan dalam imageOutput.
- Menampilkan gambar input dan output: Gambar input dan output ditampilkan berdampingan menggunakan fungsi subplot dan imshow dari matplotlib.pyplot.
- Perhitungan dan tampilan histogram: Histogram gambar input dihitung menggunakan fungsi calcHist dari cv2. Histogram kemudian ditampilkan menggunakan fungsi subplot dan plot dari matplotlib.pyplot.
- Mengonversi ruang warna dan menampilkan gambar: Gambar input dikonversi dari ruang warna BGR ke RGB menggunakan fungsi cvtColor dari cv2. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan dengan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.
- Menampilkan gambar dan histogram: Gambar input dan histogramnya ditampilkan pada baris pertama subplot 2x2, sedangkan gambar output dan histogramnya ditampilkan pada baris kedua.
- Pemerataan histogram: Gambar input dibaca lagi dengan menggunakan fungsi imread dari cv2, kali ini sebagai gambar skala abu-abu. Histogram gambar skala abu-abu dihitung menggunakan fungsi hist dari cv2, dan penyetaraan histogram diterapkan dengan menggunakan fungsi equalizeHist dari cv2. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan dengan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.
- Penyesuaian kecerahan: Array gambar baru citra_cerah dibuat sebagai salinan array gambar masukan. Penyesuaian kecerahan diterapkan pada setiap piksel array gambar baru dengan menambahkan nilai konstan beta ke nilai piksel. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.
- Penyesuaian kontras: Array gambar baru citra_kontras dibuat sebagai salinan array gambar input. Penyesuaian kontras diterapkan pada setiap piksel array gambar baru dengan mengalikan nilai piksel dengan nilai konstan alpa. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.

Berikut alur penjelasan skrip tersebut:

- Mengimpor library: Library yang diperlukan untuk pemrosesan gambar dan visualisasi diimpor, termasuk matplotlib.pyplot, numpy, cv2, dan skimage.
- Membaca dan menampilkan gambar: Skrip membaca gambar bernama "citra_medis1.jpg" menggunakan fungsi imread dari skimage.io. Bentuk gambar dicetak menggunakan atribut shape dari array gambar. Gambar tersebut kemudian ditampilkan menggunakan fungsi imshow dari matplotlib.pyplot.
- Menerapkan filter: Kernel didefinisikan sebagai matriks 3x3, dan fungsi filter2D dari cv2 digunakan untuk menerapkan kernel ke gambar input. Gambar yang dihasilkan disimpan dalam imageOutput.
- Menampilkan gambar input dan output: Gambar input dan output ditampilkan berdampingan menggunakan fungsi subplot dan imshow dari matplotlib.pyplot.
- Membaca dan menampilkan citra lain: Citra lain bernama "citra_medis.jpg" dibaca menggunakan fungsi imread dari cv2. Citra tersebut ditampilkan menggunakan fungsi imshow dari cv2.
- Perhitungan dan tampilan histogram: Histogram gambar input dihitung dengan menggunakan fungsi calcHist dari cv2. Histogram kemudian ditampilkan menggunakan fungsi subplot dan plot dari matplotlib.pyplot.
- Mengonversi ruang warna dan menampilkan gambar: Gambar input dikonversi dari ruang warna BGR ke RGB menggunakan fungsi cvtColor dari cv2. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.
- Menampilkan gambar dan histogram: Gambar input dan histogramnya ditampilkan pada baris pertama subplot 2x2, sedangkan gambar output dan histogramnya ditampilkan pada baris kedua.
- Penyetaraan histogram: Gambar input dibaca lagi dengan menggunakan fungsi imread dari cv2, kali ini sebagai gambar skala abu-abu. Histogram gambar skala abu-abu dihitung menggunakan fungsi hist dari cv2, dan penyetaraan histogram diterapkan dengan menggunakan fungsi equalizeHist dari cv2. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan dengan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.
- Penyesuaian kecerahan: Array gambar baru citra_cerah dibuat sebagai salinan array gambar masukan. Penyesuaian kecerahan diterapkan pada setiap piksel array gambar baru dengan menambahkan nilai konstan beta ke nilai piksel. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.
- Penyesuaian kontras: Array gambar baru citra_kontras dibuat sebagai salinan array gambar input. Penyesuaian kontras diterapkan pada setiap piksel array gambar baru dengan mengalikan nilai piksel dengan nilai konstan alpa. Gambar yang dihasilkan dan histogramnya ditampilkan secara berdampingan menggunakan fungsi subplot dan imshow/plot dari matplotlib.pyplot.

Sitasi:
- [1] https://www.semanticscholar.org/paper/6fa1d896eefee377adc9847c9211817dca478ae1 
- [2] https://www.semanticscholar.org/paper/6fa1d896eefee377adc9847c9211817dca478ae1
- [3] https://www.semanticscholar.org/paper/f06e0eba145bb5b8753030d16d74287f021081d5
- [4] https://www.semanticscholar.org/paper/6fa1d896eefee377adc9847c9211817dca478ae1
- [5] https://www.semanticscholar.org/paper/d52266a4101e369f37a8e253089c7b4b541ac6ba
- [6] https://www.semanticscholar.org/paper/b0077a4162c807fd9b83a276c784943fe0f3eee5
- [7] https://www.semanticscholar.org/paper/f7b95be8724cc5ede92af390961e76860c9cf1e4
- [8] https://www.semanticscholar.org/paper/7c6ad2b97c2e4d00b5d2697d5d16323b3fdc9c97
- [9] https://www.semanticscholar.org/paper/f06e0eba145bb5b8753030d16d74287f021081d5
- [10] https://www.semanticscholar.org/paper/6fa1d896eefee377adc9847c9211817dca478ae1
- [11] https://www.semanticscholar.org/paper/d52266a4101e369f37a8e253089c7b4b541ac6ba
- [12] https://www.semanticscholar.org/paper/b0077a4162c807fd9b83a276c784943fe0f3eee5
- [13] https://www.semanticscholar.org/paper/f7b95be8724cc5ede92af390961e76860c9cf1e4
- [14] https://www.semanticscholar.org/paper/7c6ad2b97c2e4d00b5d2697d5d16323b3fdc9c97
- [15] https://www.semanticscholar.org/paper/64f0198914f3c27be7ee7482a752620335aa5098
- [16] https://www.semanticscholar.org/paper/991b226c007379a6183d34fe5f7563b4c4be880d
- [17] https://www.semanticscholar.org/paper/7c6ad2b97c2e4d00b5d2697d5d16323b3fdc9c97
- [18] https://www.semanticscholar.org/paper/f44ecaa8f78088a3ab6925ad90f5a1790421c6d6
- [19] https://www.semanticscholar.org/paper/7a27865740dae1fd2f3bb4eaf2f175c0967f195d
- [20] https://www.semanticscholar.org/paper/6fa1d896eefee377adc9847c9211817dca478ae1
- [21] https://www.perplexity.ai/search/Histogram-Pengolahan-Citra-x63p9jglS4q0kjSq4JTKAw?s=c 
## 🔗 Link Data Diri
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anugrahak)

## Authors

- Anugrah AK. [@aanggaanugrahhakk](https://www.github.com/aanggaanugrahhakk)


## Identitas Authors

Nama: Anugrah AK.

NIM: 202131037

Kelas: B
