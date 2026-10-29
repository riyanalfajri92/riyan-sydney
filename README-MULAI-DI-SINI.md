# Cerita Sydney Riyan — paket Vercel

Semua cerita dan caption ID/EN dipertahankan. Foto sumber sebelum kompresi disimpan tanpa perubahan di public/assets/originals. Album memakai WebP terpisah; ketika diketuk, foto membuka sumber resolusi tinggi. Foto sumber yang memang kecil tidak di-upscale. Peta memakai resolusi sebelum kompresi.

## Pasang melalui GitHub Desktop → Vercel
1. Ekstrak ZIP ini. Jangan unggah ZIP besar ini ke Vercel Drop atau GitHub sebagai satu berkas.
2. Buka GitHub Desktop, pilih File → New Repository. Nama: riyan-sydney. Pilih tempat penyimpanannya.
3. Salin ISI folder riyan-sydney-vercel (public, vercel.json dan panduan ini) ke dalam folder repository yang baru dibuat. public dan vercel.json harus berada di tingkat teratas repository.
4. Di GitHub Desktop, tulis ringkasan “Website cerita Sydney”, lalu Commit to main. Klik Publish repository. Repository boleh private. Foto dalam website tetap dapat diakses pengunjung setelah deployment.
5. Di Vercel: Add New → Project → Import repository riyan-sydney. Izinkan akses GitHub bila diminta.
6. Framework Preset: Other. Root Directory: ./ . Build Command: kosong/tidak perlu. Output Directory: public. Tidak perlu environment variable, instalasi paket, atau Vercel Blob.
7. Klik Deploy. Setelah selesai, buka alamat yang diberikan Vercel.

Paket ini memakai integrasi Git, bukan CLI/Drop yang batas unggahnya berbeda. Seluruh aset harus ikut masuk repository; jangan hanya mengunggah index.html. Vercel akan menyajikan aset sebagai berkas statis terpisah. Tidak semua foto diunduh ketika halaman dibuka. Jangan jalankan optimasi kompresi ulang pada originals.

## Memperbarui cerita
Ganti berkas dalam repository, Commit lalu Push lewat GitHub Desktop. Vercel membuat deployment baru otomatis jika integrasi Git aktif.

## Membuka di laptop
Buka public/index.html sambil menjaga folder assets di sebelahnya. Foto/peta lokal tersedia tanpa internet; YouTube dan tautan eksternal membutuhkan internet.

## Catatan
ZIP total boleh lebih dari 100 MB; batas unggahan CLI Hobby 100 MB tidak menjadi alasan mengompres semua foto menjadi satu HTML lagi. Jangan mengunggah paket ini sebagai satu ZIP ke antarmuka yang membatasi 100 MB. Penyajian publik tetap memakai kuota transfer paket Vercel. Belum ada deployment ke akun Vercel Anda yang dilakukan dari paket ini.
