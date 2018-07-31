# SlayTheSpire-Translasi-Indo
File .json buat translasi Indonesianya Slay The Spire. Aturan mainnya:

1. Tipe file di sini adalah .json. Di dalamnya ada bagian yang bernama "fields." Jangan ditranslate!
    <br>Field adalah nama yang digunakan oleh gamenya untuk mengidentifikasi teks translasi. Kalau ditranslate, gamenya bisa bingung.
    
    Contoh (Teks yang diawali sama "<<<" adalah keterangan tambahan, bukan kode asli):
> ```
> "Ironclad": {
>     "NAMES": [          <<< Ini contoh salah satu "Field"
>         "The Ironclad"  <<< Ini teks yang bisa ditranslasi. Diapit oleh dua kurung siku []
>     ], 
> "TEXT": [
>         "The remaining soldier of the Ironclads. NL Sold his soul to harness demonic energies."   <<< Ini juga bisa ditranslasi; diapit dua kurung siku []
>     ]
> },
> ```
2. Formatting tag dkk:
    - Teks biasanya berwarna putih. Tetapi kalau ada kata kunci penting atau hal penting lainnya, kamu bisa mewarnai teks dengan
    menggunakan tag: #y, #r, #g, #b, #p. Sesuai urutan: Yellow-Kuning, Red-Merah, Green-Hijau, Blue-Biru, dan Purple-Ungu (Warna ungu jangan dipakai buat teks kartu, yo. Khusus buat event)
    Contoh: "#yOi, #yKuning! Satu tag cuma bisa #rmewarnai #rsatu #kata. #pAwas #pspasi."

    - Khusus di event dan dialog, kamu bisa menjepit kata dengan ~ untuk efek gelombang (naik turun), atau @ untuk efek getar-getar.
    EXAMPLE: "@Jangan@ @lupa@ @tiap@ @kata.@ Bisa juga tiap huruf. ~W~ ~u~ ~u~."

    - Kombinasi tag warna dan tag efek bisa digabung. Tag warna harus diketik lebih dulu (di kiri).
    EXAMPLE: "#y@DUAR@ #y@DUAR@"

    - Ingat, banyak teks kartu yang harus menampilkan jumlah damage, blok, dsb. Tagnya: !D! untuk damage, !B! untuk blok, dan !M! untuk lain-lain (miscellaneous).
    EXAMPLE: "Timbulkan !D! damage."
    EXAMPLE: "Peroleh !B! blok."
    EXAMPLE2: "Ambil !M! kartu."

    - Kata Kunci yang ada di file keywords.json wajib dikapitalisasi, terutama di dalam deskripsi kartu, bakat (power), atau pusaka (relic).
    EXAMPLE: "Timbulkan 2 Letih (Vulnerable)." (Lemah letih lesu - Weak VUln Frail)

    - Tag NL artinya baris baru. Ibarat tombol "Enter" kalau mengetik biasa. Gunakan baris baru supaya
    teks Indonesia yang panjang-panjang enak dibaca, atau untuk memisahkan
    "quote quote"
    penting. Tag NL harus dispasi di kedua sisi.
    EXAMPLE: "Halo. NL Saya Bejo."

    - Terkadang, kode untuk deskripsi di filenya kelihatan terpotong-potong. 
    Tenang saja, itu memang disengaja. Developernya perlu memasukkan nilai tertentu di antara potongan teksnya.
    Contoh:
    "Balonku ada #b",
    ", rupa-rupa warnanya."
    Akan kelihatan jadi: "Balonku ada #b5, rupa-rupa warnanya" di dalam gamenya.
