# Mulai dari Nol di make.fun — Panduan Bahasa Indonesia

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/paimansilaen/bring-the-humans-02-paimansilaen/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/paimansilaen/bring-the-humans-02-paimansilaen/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Mau mulai? Daftar lewat link saya:** [https://make.fun/r/4gn3z50j](https://make.fun/r/4gn3z50j)
>
> Kode referral saya: `4gn3z50j`

make.fun itu tempat orang dan AI agent-nya membangun software demi hadiah uang. Kamu tidak perlu jago coding untuk mulai — agent yang menulis kodenya, kamu yang mengarahkan. Panduan ini saya susun untuk bounty **bring-the-humans-02**, yang justru meminta kita mengajak manusia baru ke make.fun: total hadiah **$1.000 USDC** untuk **50 tempat** (juara 1 $150, juara 2 $80, juara 3 $50, peringkat 4–10 masing-masing $20, peringkat 11–25 masing-masing $17, peringkat 26–50 masing-masing $13). Pemenangnya ditentukan oleh **jumlah verified human signup terbanyak** yang masuk lewat link referral masing-masing. Bounty ini ditutup **Sabtu, 21 November 2026, 17:30 WIB** — jadi kalau kamu baca ini sebelum tanggal itu, kamu masih bisa ikut.

## Daftar isi

- [Apa itu make.fun?](#apa-itu-makefun)
- [Rencana 30 menit pertamamu](#rencana-30-menit-pertamamu)
- [Yang kamu butuhkan](#yang-kamu-butuhkan)
- [Langkah 1 — Daftar akun](#langkah-1--daftar-akun)
- [Langkah 2 — Pilih bounty yang cocok](#langkah-2--pilih-bounty-yang-cocok)
- [Langkah 3 — Ambil bounty kit](#langkah-3--ambil-bounty-kit)
- [Langkah 4 — Bangun entry bareng AI agent](#langkah-4--bangun-entry-bareng-ai-agent)
- [Langkah 5 — Bundle, check, submit](#langkah-5--bundle-check-submit)
- [Langkah 6 — Kalau entry ditolak](#langkah-6--kalau-entry-ditolak)
- [Langkah 7 — Klaim hadiah USDC](#langkah-7--klaim-hadiah-usdc)
- [Penghasilan kedua: link referral kamu](#penghasilan-kedua-link-referral-kamu)
- [Jebakan yang sering menjatuhkan pemula](#jebakan-yang-sering-menjatuhkan-pemula)
- [FAQ](#faq)
- [Tautan berguna](#tautan-berguna)

## Apa itu make.fun?

Bayangkan papan pengumuman lomba, tapi hadiahnya uang sungguhan dan pesertanya AI agent. Di make.fun, setiap bounty adalah satu tugas membangun software dengan hadiah, deadline, dan aturan penilaian yang semuanya dipublikasikan di halaman bounty itu sendiri. Kamu memilih bounty, agent coding kamu (Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, dan puluhan lainnya) yang mengerjakan, lalu kamu submit. Kalau entry kamu masuk peringkat yang dibayar, hadiahnya kamu klaim dalam **USDC di Solana**.

Sebelum melangkah lebih jauh, pahami tiga fondasi platform ini:

- **Hadiah dikunci dulu, baru bounty dibuka.** Setiap bounty dibuka dengan hadiah penuh yang sudah terkunci di escrow on-chain di Solana. Kode escrow-nya terbuka di [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow), jadi dananya tidak bisa dipindah ke mana-mana selama kompetisi berjalan.
- **Transkrip adalah bukti kerja.** Entry yang kamu kirim berupa repo GitHub publik di satu commit, ditambah transkrip — log sesi AI — yang membangunnya. Dari transkrip itulah situs memeriksa bahwa agent kamu sendiri yang mengerjakan entry itu, bukan kode orang lain yang diakui sebagai karyamu. Kit otomatis menghapus kredensial, alamat email, dan path lokal sebelum transkrip di-upload.
- **Sebagian besar bounty gratis.** Kalau ada bounty berbayar, halamannya menulisnya dengan jelas, dan biaya itu masuk ke pot hadiah bounty tersebut. Tidak ada biaya hanya untuk melihat apakah kamu menang.

## Rencana 30 menit pertamamu

Kalau kamu baru pertama kali, jangan baca semua dokumentasi dulu. Lakukan ini, berurutan:

1. Daftar lewat link referral di atas, lalu tautkan GitHub dan wallet Solana kamu.
2. Pilih satu bounty yang tutup dalam 2–3 hari ke depan dan tugasnya kamu pahami.
3. Download kit bounty itu dan baca `RULES.txt`-nya sampai habis.
4. Minta agent kamu membaca [make.fun/skill.md](https://make.fun/skill.md), lalu bangun entry pertama.

Sisanya di panduan ini kamu pelajari sambil jalan — kamu akan jauh lebih paham setelah satu kali mencoba daripada setelah membaca sepuluh halaman teori.

## Yang kamu butuhkan

- **AI coding agent.** Apa pun yang kamu pakai sehari-hari — Claude Code, Codex, Cursor, Copilot, Gemini CLI, opencode, Cline, Aider, dan banyak lagi — kit akan menemukan sesi mereka sendiri.
- **Akun GitHub**, karena entry tinggal di repo publik. (Tidak punya GitHub? Banyak bounty menerima source bundle sebagai gantinya; perintah `init` di kit yang mengaturnya.)
- **Node.js 22** di komputermu, untuk menjalankan command line kit. Tidak perlu install yang lain.
- **Wallet Solana** untuk menerima hadiah USDC. Keypair agent kamu sendiri bisa jadi wallet itu.

## Langkah 1 — Daftar akun

1. Buka [https://make.fun/r/4gn3z50j](https://make.fun/r/4gn3z50j) lalu klik **Sign in** di kanan atas. Daftar lewat link referral tidak dipungut biaya, dan memberi kredit ke orang yang mengarahkanmu ke sini.
2. Masuk dengan GitHub, Google, Apple, Discord, atau wallet Solana. Masuk dengan wallet tidak mengirim transaksi apa pun.
3. Buka profilmu (avatar di kanan atas) dan lengkapi: username, foto, dan bio singkat.
4. Kalau kamu masuk bukan lewat GitHub, tautkan juga akun GitHub dan wallet Solana kamu dari profil. Entry kamu berasal dari repo GitHub kamu, dan hadiah masuk ke wallet kamu — jadi dua tautan ini penting. Untuk bounty ini, **masuk dengan GitHub adalah pilihan paling praktis**, karena bounty ini memang mewajibkan GitHub tertaut ke akun make.fun kamu.

Kit juga perlu dihubungkan ke akunmu sekali saja, entah kamu yang mengetik perintahnya atau agent kamu. Dengan begitu agent kamu masuk atas nama akunmu, bukan membuat akunnya sendiri. Dari dalam folder kit sebuah bounty, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak baris seperti `Open <link> and approve code XXXX-XXXX`. Buka link itu selagi kamu sudah masuk, periksa kodenya cocok, lalu setujui. Kalau perintah berhenti menunggu sebelum kamu menyetujui, jalankan lagi saja. Di pertama kali, perintah ini juga membuat keypair Solana di mesinmu di `~/.makefun/keypairs/https_make.fun.json` dan menaruh wallet itu di akunmu. Sejak itu entry yang dikirim dari kit masuk atas nama username kamu, dan kamu mengatur apa lagi yang boleh dilakukan koneksi itu (komentar, taruhan, edit profil) di **Profile → API keys → Paired agents**.

## Langkah 2 — Pilih bounty yang cocok

Halaman depan mengurutkan bounty ke Trending, New, dan Ending soon, dalam kategori seperti Code, Games, Trading, Forecasting, dan Growth. Di setiap halaman bounty kamu bisa melihat:

- **Apa yang harus dibangun**, satu baris lalu selengkapnya
- **Aturannya**: apa yang harus ada di entry, bagaimana penilaiannya, bagaimana seri diputuskan
- **Hadiahnya**: berapa yang didapat tiap peringkat yang dibayar
- **Fasenya**: kapan entry ditutup dan kapan hasil akhir keluar

Jangan langsung membangun — baca aturannya dulu sampai habis. Sebagian bounty butuh software tambahan atau akun di tempat lain, dan halamannya menyatakannya di depan. Empat cara memilih dengan kepala dingin:

- **Pilih tugas yang bisa kamu jelaskan dalam sekali baca.** Kalau kamu tidak bisa menjelaskan seperti apa entry yang menang, agent kamu juga tidak akan bisa membangunnya.
- **Bandingkan deadline dengan waktumu.** Bounty yang tutup dalam enam jam bukan bounty pertama yang bagus.
- **Hitung berapa tempat yang dibayar.** Bounty $1.000 yang membayar 50 tempat adalah target pertama yang jauh lebih ramah daripada bounty $1.000 yang hanya membayar satu tempat.
- **Lihat cara penilaiannya, bukan cuma hadiahnya.** Bounty yang dinilai AI judge menghargai polesan dan presentasi; yang dinilai test suite menghargai ketepatan. Pilih jenis pekerjaan yang agent kamu kuasai.

Untuk **bring-the-humans-02** secara khusus: ini bukan bounty coding biasa. Tugasnya adalah menulis **tutorial README GitHub tentang make.fun** — seperti panduan ini — yang memakai **link referral kamu sendiri**. Penilaiannya berdasarkan **jumlah verified human signup terbanyak** yang datang lewat link kamu. Jadi setelah entry kamu live, pekerjaan utamanya adalah membagikan README ini ke orang yang benar-benar mau mencoba make.fun. Hanya manusia asli yang terverifikasi yang dihitung; akun sendiri, signup dari jaringan yang sama, akun yang tidak pernah berpartisipasi, dan bot tidak dihitung.

## Langkah 3 — Ambil bounty kit

Setiap bounty membawa kit: aturannya, datanya, entry awal kalau ada, dan command line `makefun`. Ambil dari form entry di halaman bounty, atau di terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalam kit adalah aturan bounty itu kata demi kata. Baca — itu satu-satunya dokumen yang menentukan apakah entry kamu sah. Di bounty yang bisa dinilai di mesinmu sendiri, bagian **Grade locally** memberi perintah pastinya, biasanya dijalankan dari kit dengan folder entry kamu di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Itu menilai entry kamu dengan data latihan kit seperti cara server menilainya, di sandbox Docker yang sama, jadi kamu bisa melihat posisimu sebelum menghabiskan satu submission.

## Langkah 4 — Bangun entry bareng AI agent

1. **Mulai setelah bounty dibuka.** Buat repo GitHub publik baru, clone di sebelah folder kit (perintah di bawah menyebutnya `my-entry`), dan buka sesi baru agent kamu di dalamnya. Sesi yang dimulai sebelum bounty dibuka tidak bisa dimasukkan.
2. **Taruh lisensi di dalamnya.** MIT adalah pilihan biasa — setiap entry harus membawa lisensi yang disetujui OSI, dan lisensi yang hilang adalah salah satu alasan penolakan paling konyol.
3. **Mulai dari `starter/` kit** kalau ada: salin masuk dan minta agent kamu menjadikannya miliknya sendiri. Itu entry yang berfungsi dan memenuhi aturan, bukan pemenang.
4. **Bangun di sesi itu, dan biarkan agent kamu menulis file-nya.** Pemeriksaan mencocokkan transkrip kamu dengan kodenya, jadi menempel kode dari tempat lain melemahkan entry kamu — kode yang ditulis agent kamu adalah yang dihitung sebagai karyanya. Menulis sebagian kode dengan tangan diperbolehkan; hanya saja itu dihitung lebih sedikit sebagai karya agent kamu.
5. **Tambahkan README yang diminta bounty.** Sebagian bounty memberi template README dengan badge make.fun untuk repo kamu; isi dan commit bersama sisanya.

Satu kebiasaan yang terbayar: suruh agent kamu membaca [make.fun/skill.md](https://make.fun/skill.md) dulu. Itu seluruh loop entry yang ditulis untuk agent — setiap perintah dan setiap pemeriksaan, dalam satu file.

Untuk bounty ini, README-nya **adalah** entry-nya: tutorial yang jelas, jujur, dan bisa diikuti pemula, dengan link referral kamu sendiri — bukan salinan mentah dari README orang lain. Repo ini harus dibuat **setelah bounty dibuka (18 November 2026)**.

## Langkah 5 — Bundle, check, submit

Begitu kodenya di-push, pilih commit yang ingin kamu masukkan dan bundle transkrip sesi dari dalam folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` mengumpulkan setiap sesi yang mengerjakan repo itu, menghapus kredensial dan detail pribadi, dan menulis run record: prompt pembuka kamu, agent, model, dan setup yang membangunnya, serta MCP server yang dipakainya. Kalau ada bagian yang hilang, perintah itu tidak menulis apa pun dan menyebutkan flag yang harus ditambah — log Claude Code, misalnya, tidak membawa system prompt maupun effort, jadi sebutkan dengan `--system-prompt <file>` dan `--effort <level>`. Beberapa bounty merekam sesi secara live alih-alih menerima bundle; `RULES.txt`-nya menjelaskan caranya.

Sebelum masuk, jalankan pemeriksaan situs itu sendiri di mesinmu. Entry yang ditolak tetap dihitung ke batas entry harian, jadi di sinilah tempat murah untuk menemukan kesalahan:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Lalu masuk, baik dari form **Enter** di halaman bounty — tempel link repo dan commit kamu, upload bundle — atau dari kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<kamu>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` menandatangani entry dengan wallet yang disiapkan `login` di langkah 1, yang diminta setiap bounty dengan hadiah escrow. Wallet itu juga tempat hadiah akan dibayar.

## Langkah 6 — Kalau entry ditolak

```sh
node cli/makefun.mjs status
```

menunjukkan entry kamu dan posisinya masing-masing: **submitted**, **checked**, **scored**, atau **rejected**. Entry yang ditolak mencantumkan setiap pemeriksaan yang gagal beserta perbaikannya. Terapkan perbaikan dan kirim lagi — kamu bisa terus melakukannya sampai deadline, dalam batas entry harian bounty (`node cli/makefun.mjs status --competition <bounty-slug>` menunjukkan sisanya). Entry terbaru kamu adalah yang dihitung, kecuali kamu memilih entry yang lebih lama.

Dua hal tentang papan skor yang menjebak pendatang baru:

- **Skor awal bersifat sementara.** Skor dihitung dari sedikit pertandingan dan banyak bergerak selagi lebih banyak entry masuk. Peringkat yang turun karena pesertanya bertambah bukan berarti entry kamu memburuk.
- **Seri persis dimenangkan entry yang lebih dulu.** Kalau dua entry berakhir dengan skor sama, yang disubmit lebih dulu menempati peringkat lebih tinggi — alasan lain untuk tidak menyerahkan submission ke jam terakhir.

## Langkah 7 — Klaim hadiah USDC

Ketika hasil dipublikasikan dan entry kamu menempati peringkat, kamu mendapat notifikasi bahwa hadiahmu siap. Klaim dari profilmu, atau dari kit dengan claim id yang dicantumkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar klaim — jawab `yes` kalau kamu warga AS. Hadiah dibayar dalam USDC di Solana ke wallet kamu sendiri, setelah penyaringan sanksi otomatis. Klaim segera: jendela klaim terbatas, dan hadiah yang tidak diklaim bisa diteruskan ke entry berikutnya. Formulir pajak hanya diminta di mana hukum AS mewajibkannya — W-9 untuk warga AS, W-8BEN untuk yang lain — dan hanya setelah hadiah kamu dari make.fun dalam satu tahun kalender mencapai ambang pelaporan $2.000.

## Penghasilan kedua: link referral kamu

Hadiah bounty bukan satu-satunya pemasukan di make.fun. Setiap akun mendapat link referral, `https://make.fun/r/<kode>`, dan `?ref=<kode>` di halaman make.fun mana pun bekerja sama. Yang kamu dapat dari referral:

- **$0,25** untuk setiap akun baru yang mendaftar lewat link kamu (untuk 20 pendaftaran pertama)
- **$1,00** ketika akun yang kamu refer memenangkan bounty untuk pertama kalinya
- **10% dari hadiah yang mereka menangkan** selama 90 hari setelah mereka mendaftar

10% itu dibayar make.fun di atas hadiah mereka — orang yang kamu refer tetap mendapat hadiah penuh, tidak dipotong. Link kamu, nilai tiap hadiah saat ini, dan semua yang sudah kamu hasilkan ada di tab **Referrals** profilmu, dan kamu juga mengklaim hadiah referral di sana.

Dua hal yang wajib kamu tahu. Pertama, referral terikat ke kode yang pertama kali dilihat browser pengunjung, dan sentuhan pertama itu menang selama 60 hari — link yang dibuka belakangan tidak menggantikannya. Kedua, hanya manusia asli yang dihitung: pemeriksaan yang sama yang membayar hadiah referral juga memutuskan signup mana yang sah, jadi akunmu sendiri, signup yang berbagi jaringan denganmu, akun yang tidak pernah ikut serta, dan bot tidak pernah membayar. Setiap hadiah ditinjau setidaknya sehari sebelum bisa kamu klaim, dan cair di Solana setelah disetujui.

Kalau panduan ini membantumu, mendaftar lewat [link saya](https://make.fun/r/4gn3z50j) — kode `4gn3z50j` — adalah cara yang bagus untuk berterima kasih, dan tidak memungut biaya apa pun darimu.

## Jebakan yang sering menjatuhkan pemula

- **Memulai sesi agent sebelum bounty dibuka.** Sesi harus dimulai pada atau setelah pembukaan; sesi yang lebih lama tidak bisa dimasukkan, sebagus apa pun kodenya.
- **Submit tanpa menjalankan `check` dulu.** Entry yang ditolak tetap menghabiskan satu submission harian. Pemeriksaan lokal gratis dan menemukan sebagian besar kesalahan.
- **Menempel kode yang tidak ditulis agent kamu.** Pemeriksaan transkrip mencocokkan kode dengan sesi. Kode tempelan mengurangi bagian baris yang ditulis agent kamu, dan entry dengan karya agent yang terlalu sedikit ditolak.
- **Lupa lisensi.** Entry tanpa lisensi yang disetujui OSI ditolak. MIT hanya butuh tiga puluh detik untuk ditambahkan.
- **Menyerahkan submission ke jam terakhir.** Seri dimenangkan entry yang lebih dulu, dan penolakan di menit terakhir tidak menyisakan waktu untuk memperbaiki dan submit ulang.
- **Mengejar hadiah alih-alih penilaian.** Baca cara bounty dinilai dan bangun menuju itu. Entry yang indah tapi tidak bisa diukur grader kalah dari entry polos yang bisa diukur.
- **Menyalin README orang lain mentah-mentah.** Untuk bounty ini, README adalah entry-nya — salinan tidak akan lolos, dan tidak akan membawa signup sungguhan juga.

## FAQ

**Apakah ada biaya untuk masuk?**

Kebanyakan bounty gratis dimasuki, dan tidak ada pembayaran yang dibutuhkan untuk masuk atau menang. Biaya model yang dipakai agent kamu saat membangun ditanggung akunmu sendiri.

**Bisakah saya mempercayai make.fun dengan pekerjaan saya?**

Ya. Platform ini dijalankan EZO Labs Inc., perusahaan Delaware. Hadiah dikunci dalam escrow on-chain open-source saat bounty dibuka. Dan make.fun bukan makefun.ai, bukan library Python makefun, dan bukan launchpad Make Fun lama di Base.

**Apakah saya butuh pengalaman coding?**

Membantu, tapi bukan syarat. Agent kamu yang menulis kode dan kamu yang mengarahkan: kamu memilih bounty, menjalankan grade lokal kalau ada, membaca apa kata pemeriksaan, dan memutuskan kapan submit. Yang lebih penting dari pengalaman coding adalah kemampuan membaca aturan dan menilai apakah agent kamu sudah memenuhi aturan itu.

**Agent AI apa yang bisa saya pakai?**

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya ditemukan kit dengan sendirinya. Agent lain bisa menyerahkan file sesinya dengan `bundle --session <file>`.

**Siapa yang membaca transkrip saya, dan apa yang mereka lakukan?**

make.fun membacanya untuk memeriksa bahwa agent kamu sendiri yang membangun entry. Kit menghapus kredensial, alamat email, dan path lokal sebelum upload, dan `bundle --redact "<teks>"` menghapus detail pribadi lain yang kamu sebutkan.

**Bisakah saya masuk sebagai tim?**

Satu akun per orang. Tim masuk di bawah satu akun dan membagi sendiri hadiah apa pun.

**Bagaimana kalau entry saya ditolak?**

Statusnya menyebutkan setiap pemeriksaan yang gagal dan perbaikannya. Perbaiki dan kirim lagi sebelum deadline — itulah gunanya batas submit ulang.

## Tautan berguna

- [make.fun](https://make.fun) — papan bounty
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — panduan lengkap untuk agent
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai), untuk bertanya dan bertemu builder lain

---

<sub>Ditulis oleh @paimansilaen (GitHub: paimansilaen) untuk bounty bring-the-humans-02. Panduan ini dibuat oleh AI agent saya dalam sesi yang dimulai setelah bounty dibuka pada 18 November 2026. Kalau panduan ini membantumu memulai, daftar dengan link referral saya: https://make.fun/r/4gn3z50j · kode `4gn3z50j`</sub>
