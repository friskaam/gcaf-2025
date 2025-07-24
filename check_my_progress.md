# 📊 Check My Progress Bookmarklet

Gunakan bookmarklet berikut untuk menyembunyikan leaderboard dan menampilkan skor pada halaman lab tertentu.

## 🔧 Cara Pakai

1. Salin kode di bawah ini.
2. Buat **bookmark baru** di browser kamu.
3. Edit bookmark
4. Tempelkan kode ini ke kolom **URL** bookmark.
5. Beri nama seperti `Check My Progress`.
6. Saat berada di halaman lab, klik bookmark tersebut untuk menjalankannya.

## 📜 Bookmarklet Kode

```
javascript:(function () {
    const removeLeaderboard = document.querySelector('.js-lab-leaderboard');
    const showScore = document.querySelector('.games-labs');

    removeLeaderboard.remove();
    showScore.className = "lab-show l-full no-nav application-new lab-show l-full no-nav";
})();

```
