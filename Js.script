document.addEventListener('DOMContentLoaded', () => {
    const emotionCards = document.querySelectorAll('.emotion-card');
    const backButtons = document.querySelectorAll('.back-button');
    const allPages = document.querySelectorAll('.page');

    // Fungsi untuk pindah halaman
    const showPage = (targetId) => {
        // Sembunyikan semua halaman
        allPages.forEach(page => {
            page.classList.remove('active');
        });
        
        // Tampilkan halaman target
        const targetPage = document.getElementById(targetId);
        if (targetPage) {
            targetPage.classList.add('active');
            window.scrollTo(0, 0); // Gulir ke atas halaman baru
        }
    };

    // Event Listener untuk Kartu Emosi (pindah ke halaman surat)
    emotionCards.forEach(card => {
        card.addEventListener('click', () => {
            const targetId = card.getAttribute('data-target');
            showPage(targetId);
        });
    });

    // Event Listener untuk Tombol Kembali (pindah ke homepage)
    backButtons.forEach(button => {
        button.addEventListener('click', () => {
            showPage('home-page');
        });
    });
});
