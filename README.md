
# 🧬 CYTB Gene Sequence & Structure Analysis using Biopython

## 📌 Project Overview

Proyek ini berfokus pada analisis komparatif sekuens DNA dan struktur dari gen **Cytochrome b (CYTB)** pada 4 spesies dari famili Proboscidea (gajah dan mamut purba) menggunakan ekosistem Python/Biopython. Proyek ini mencakup otomatisasi pengunduhan data FASTA langsung dari NCBI Entrez, analisis frekuensi basa/nukleotida, visualisasi data, hingga penentuan jarak genetik (Levenshtein distance) dan *pairwise alignment*.

---

## 🔬 Spesies yang Dianalisis

Data sekuens DNA diperoleh dari **NCBI Nucleotide Database**:

1. **Gajah Asia** (*Elephas maximus*) - `NC_005129.2`
2. **Gajah Sabana Afrika** (*Loxodonta africana*) - `NC_000934.1`
3. **Gajah Hutan Afrika** (*Loxodonta cyclotis*) - `AY195701.1`
4. **Mammoth Purba** (*Mammuthus primigenius*) - `EU153444.1`

---

## 🛠️ Fitur & Metodologi Utama

* **Otomatisasi Data Pipeline (Biopython Entrez)**
Mengunduh file `.fasta` sekuens gen lengkap dari database NCBI secara langsung dengan pustaka `Bio.Entrez`.
* **Analisis Sekuens & Komposisi Basa**
Menganalisis panjang sekuens, *subsequence* (20 bp pertama & terakhir), serta menghitung frekuensi distribusi basa nitrogen (A, T, G, C).
* **Visualisasi Data**
Membuat bar chart interaktif dengan `matplotlib` untuk membandingkan frekuensi basa antar spesies.
* **Analisis Penjajaran & Jarak Genetik (*Alignment & Distance*)**
Melakukan *pairwise sequence alignment* (`Bio.pairwise2`) dan perhitungan jarak Levenshtein (`python-Levenshtein`) untuk mengukur tingkat kemiripan genetik antar spesies.
* **Visualisasi Molekuler 3D**
Dukungan integrasi visualisasi struktur 3D protein/DNA menggunakan `py3Dmol` dan `Bio.PDB`.

---

## 🧰 Pustaka & Teknologi (Tech Stack)

* **Language:** Python 3.12
* **Bioinformatics:** `Biopython` (`Bio.Entrez`, `Bio.SeqIO`, `Bio.pairwise2`, `Bio.PDB`)
* **Data Processing & Analytics:** `NumPy`, `collections.Counter`, `python-Levenshtein`
* **Visualization:** `Matplotlib`, `py3Dmol`
