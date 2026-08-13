[index.html](https://github.com/user-attachments/files/31010943/index.html)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>SDN 001 Ukui | Sekolah Dasar Negeri</title>

    <meta name="description"
          content="Website resmi SDN 001 Ukui. Sekolah dasar unggul, berkarakter, berbudaya, berwawasan digital dan lingkungan.">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5f8fc;
            color: #1f2937;
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }.school-logo {
    width: 55px;
    height: 55px;
    object-fit: contain;
    margin-right: 12px;
}

.logo-text h2 {
    margin: 0;
}

.logo-text span {
    font-size: 12px;
}

        /* =========================
           NAVBAR
        ========================= */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 999;
            background: rgba(255,255,255,0.96);
            box-shadow: 0 2px 15px rgba(0,0,0,0.08);
        }

       .navbar {
    max-width: 1200px;
    margin: auto;
    height: 75px;
    display: flex;
    align-items: center;
    padding: 0 25px;
    position: relative;
}

 .logo {
    display: flex;
    align-items: center;
    gap: 10px;
    height: 75px;
    flex-shrink: 0;
}

.school-logo {
    width: 52px;
    height: 52px;
    object-fit: contain;
    display: block;
    margin: 0;
}

.logo-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    line-height: 1.2;
}

.logo-text h2 {
    margin: 0;
    padding: 0;
    color: #1f2937;
    font-size: 22px;
    font-weight: 700;
    white-space: nowrap;
}

.logo-text span {
    display: block;
    margin-top: 4px;
    color: #68c03f;
    font-size: 12px;
    white-space: nowrap;
}     
        .nav-menu a {
            font-size: 14px;
            font-weight: 600;
            color: #0beb1e;
            transition: 0.3s;
        }

        .nav-menu a:hover {
            color: #08c621;
        }

        .menu-btn {
            display: none;
            border: none;
            background: #2ab507;
            color: white;
            padding: 9px 12px;
            border-radius: 6px;
            font-size: 20px;
            cursor: pointer;
        }

        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 100vh;
            padding: 130px 25px 80px;
            background:
                linear-gradient(rgba(9, 10, 112, 0.82), rgba(12, 15, 199, 0.72)),
                url(GAMBAR/WhatsApp\ Image\ 2026-08-12\ at\ 20.29.33.jpeg)
                center/cover;
            display: flex;
            align-items: center;
        }

        .hero-content {
            max-width: 1200px;
            width: 100%;
            margin: auto;
            color: white;
        }

        .hero-content small {
            display: inline-block;
            background: rgba(255,255,255,0.15);
            border: 1px solid rgba(255,255,255,0.3);
            padding: 8px 16px;
            border-radius: 30px;
            margin-bottom: 20px;
        }

        .hero h1 {
            font-size: clamp(40px, 6vw, 75px);
            line-height: 1.05;
            max-width: 850px;
            margin-bottom: 25px;
        }

        .hero h1 span {
            color: #ffd43b;
        }

        .hero p {
            max-width: 650px;
            font-size: 18px;
            color: #eaf4ff;
            margin-bottom: 35px;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 13px 23px;
            border-radius: 8px;
            font-weight: bold;
            display: inline-block;
            transition: 0.3s;
        }

        .btn-primary {
            background: #ffd43b;
            color: #16a509;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
        }

        .btn-outline {
            border: 1px solid white;
            color: white;
        }

        .btn-outline:hover {
            background: white;
            color: #0db507;
        }

        /* =========================
           GENERAL
        ========================= */

        section {
            padding: 90px 25px;
        }

        .container {
            max-width: 1200px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title span {
            color: #08c611;
            font-size: 14px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .section-title h2 {
            font-size: 36px;
            margin-top: 8px;
            color: #13940f;
        }

        .section-title p {
            max-width: 650px;
            margin: 12px auto 0;
            color: #6b7280;
        }

        /* =========================
           TENTANG
        ========================= */

        .about {
            background: white;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-image img {
            width: 100%;
            height: 420px;
            object-fit: cover;
            border-radius: 18px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.12);
        }

        .about-text h3 {
            font-size: 30px;
            color: #07b410;
            margin-bottom: 18px;
        }

        .about-text p {
            color: #5b6470;
            margin-bottom: 15px;
        }

        .vision {
            margin-top: 25px;
            padding: 20px;
            background: #edf6ff;
            border-left: 5px solid hsl(115, 86%, 43%);
            border-radius: 8px;
        }

        .vision strong {
            color: #09ce3a;
        }

        /* =========================
           STATISTIK
        ========================= */

        .stats {
            background: linear-gradient(135deg, #24b507, #07da34);
            color: white;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .stat {
            text-align: center;
            padding: 30px 15px;
            border: 1px solid rgba(255,255,255,0.2);
            border-radius: 15px;
            background: rgba(255,255,255,0.08);
        }

        .stat h3 {
            font-size: 40px;
            color: #ffd43b;
        }

        .stat p {
            color: white;
        }

        /* =========================
           PROGRAM
        ========================= */

        .program-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .program-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 7px 25px rgba(0,0,0,0.07);
            transition: 0.3s;
        }

        .program-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.12);
        }

        .icon {
            width: 55px;
            height: 55px;
            background: #e6f3ff;
            color: #0bcf15;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 25px;
            margin-bottom: 20px;
        }

        .program-card h3 {
            color: #28a00a;
            margin-bottom: 10px;
        }

        .program-card p {
            color: #6b7280;
            font-size: 14px;
        }

        /* =========================
           BERITA
        ========================= */

        .news {
            background: white;
        }

        .news-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .news-card {
            background: #fff;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 7px 25px rgba(0,0,0,0.08);
        }

        .news-card img {
            width: 100%;
            height: 210px;
            object-fit: cover;
        }

        .news-body {
            padding: 22px;
        }

        .date {
            color: #19c50a;
            font-size: 13px;
            font-weight: bold;
        }

        .news-body h3 {
            margin: 8px 0;
            color: #57d60e;
        }

        .news-body p {
            font-size: 14px;
            color: #6b7280;
        }

        /* =========================
           GALERI
        ========================= */

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
        }

        .gallery-grid img {
            width: 100%;
            height: 220px;
            object-fit: cover;
            border-radius: 12px;
            transition: 0.3s;
        }

        .gallery-grid img:hover {
            transform: scale(1.03);
        }

        /* =========================
           KONTAK
        ========================= */

        .contact {
            background: #edf6ff;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 35px;
        }

        .contact-box {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.06);
        }

        .contact-item {
            display: flex;
            gap: 15px;
            margin-bottom: 22px;
        }

        .contact-icon {
            width: 45px;
            height: 45px;
            flex-shrink: 0;
            background: #e5f2ff;
            color: #08c641;
            border-radius: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .contact-item h4 {
            color: #3bcc10;
        }

        .contact-item p {
            font-size: 14px;
            color: #6b7280;
        }

        .map {
            width: 100%;
            height: 350px;
            border: none;
            border-radius: 15px;
        }

        /* =========================
           FOOTER
        ========================= */

        footer {
            background: #34bd0b;
            color: white;
            padding: 55px 25px 20px;
        }

        .footer-grid {
            max-width: 1200px;
            margin: auto;
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            gap: 40px;
        }

        footer h3 {
            margin-bottom: 15px;
        }

        footer p {
            color: #b8c7d8;
            font-size: 14px;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 8px;
            color: #c7d5e4;
            font-size: 14px;
        }

        .copyright {
            max-width: 1200px;
            margin: 40px auto 0;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.15);
            text-align: center;
            color: #9fb1c4;
            font-size: 13px;
        }

        /* =========================
           WHATSAPP
        ========================= */

        .whatsapp {
            position: fixed;
            right: 20px;
            bottom: 20px;
            width: 58px;
            height: 58px;
            background: #25d366;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 27px;
            z-index: 1000;
            box-shadow: 0 5px 20px rgba(0,0,0,0.25);
        }

        /* =========================
           RESPONSIVE
        ========================= */

        @media(max-width: 900px) {

            .nav-menu {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);

    display: flex;
    align-items: center;
    gap: 30px;

    list-style: none;
    margin: 0;
    padding: 0;
}

            .nav-menu.active {
                display: flex;
            }

            .nav-menu li {
                padding: 15px 25px;
                border-bottom: 1px solid #eee;
            }

            .menu-btn {
                display: block;
            }

            .about-grid,
            .contact-grid {
                grid-template-columns: 1fr;
            }

            .stats-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .program-grid,
            .news-grid {
                grid-template-columns: 1fr 1fr;
            }

            .gallery-grid {
                grid-template-columns: 1fr 1fr;
            }

            .footer-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        @media(max-width: 600px) {

            .navbar {
                padding: 0 15px;
            }

            .logo-text h2 {
                font-size: 15px;
            }

            .hero {
                min-height: 90vh;
            }

            .hero h1 {
                font-size: 43px;
            }

            .hero p {
                font-size: 16px;
            }

            section {
                padding: 65px 18px;
            }

            .section-title h2 {
                font-size: 28px;
            }

            .stats-grid,
            .program-grid,
            .news-grid,
            .gallery-grid,
            .footer-grid {
                grid-template-columns: 1fr;
            }

            .about-image img {
                height: 280px;
            }

            .gallery-grid img {
                height: 250px;
            }
        }/* =========================
   HERO DUA KOLOM
========================= */

.hero-grid {
    display: grid;
    grid-template-columns: 1.5fr 0.7fr;
    align-items: center;
    gap: 50px;
    width: 100%;
}

.hero-text {
    max-width: 700px;
}


/* =========================
   FOTO KEPALA SEKOLAH
========================= */

.kepsek-card {
    text-align: center;
    padding: 25px;
    background: rgba(255,255,255,0.12);
    backdrop-filter: blur(8px);
    -webkit-backdrop-filter: blur(8px);

    border: 1px solid rgba(255,255,255,0.35);
    border-radius: 25px;

    box-shadow: 0 15px 40px rgba(0,0,0,0.25);
}

.kepsek-card img {
    width: 220px;
    height: 220px;

    object-fit: cover;

    border-radius: 50%;

    border: 6px solid white;

    box-shadow:
        0 10px 30px rgba(0,0,0,0.35);

    display: block;

    margin: 0 auto 18px;
}

.kepsek-card h3 {
    color: white;
    font-size: 20px;
    margin-bottom: 5px;
}

.kepsek-card p {
    color: #ffd43b;
    font-size: 15px;
    font-weight: bold;
}


/* =========================
   TAMPILAN HP
========================= */

@media (max-width: 900px) {

    .hero-grid {
        grid-template-columns: 1fr;
        text-align: center;
    }

    .hero-text {
        max-width: 100%;
    }

    .hero-buttons {
        justify-content: center;
    }

    .kepsek-card {
        width: 100%;
        max-width: 350px;
        margin: 20px auto 0;
    }

    .kepsek-card img {
        width: 170px;
        height: 170px;
    }

} /* =========================
   PERBAIKAN MENU NAVBAR
========================= */

header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 9999;
    background: rgba(255, 255, 255, 0.97);
    box-shadow: 0 2px 15px rgba(0, 0, 0, 0.08);
}

.navbar {
    max-width: 1200px;
    height: 75px;
    margin: 0 auto;
    padding: 0 25px;

    display: flex !important;
    align-items: center;
    position: relative;
}

/* LOGO */
.logo {
    display: flex !important;
    align-items: center;
    gap: 10px;
    height: 75px;
    flex-shrink: 0;
}

.school-logo {
    width: 52px;
    height: 52px;
    object-fit: contain;
    display: block;
}

/* TULISAN SDN 001 UKUI */
.logo-text {
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.logo-text h2 {
    margin: 0;
    padding: 0;
    font-size: 22px;
    line-height: 1.2;
    color: #1f2937;
    white-space: nowrap;
}

.logo-text span {
    margin-top: 4px;
    font-size: 12px;
    line-height: 1;
    color: #68c03f;
    white-space: nowrap;
}

/* MENU */
.nav-menu {
    position: absolute !important;

    left: 50% !important;
    top: 50% !important;

    transform: translate(-50%, -50%) !important;

    display: flex !important;
    flex-direction: row !important;
    align-items: center !important;

    gap: 30px !important;

    margin: 0 !important;
    padding: 0 !important;

    list-style: none !important;
}

.nav-menu li {
    margin: 0 !important;
    padding: 0 !important;
    border: none !important;
    list-style: none !important;
}

.nav-menu a {
    display: block !important;

    color: #16b507 !important;

    font-size: 14px !important;
    font-weight: 600 !important;

    text-decoration: none !important;

    white-space: nowrap;

    padding: 8px 0 !important;

    transition: 0.3s;
}

.nav-menu a:hover {
    color: #078a00 !important;
}

/* TOMBOL HP */
.menu-btn {
    display: none;
}/* =========================
   VIDEO PROFIL
========================= */

.video-profile {
    background: #ffffff;
    padding: 80px 25px;
}

.video-box {
    max-width: 950px;
    margin: 0 auto;
    padding: 8px;
    background: #111;
    border-radius: 18px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.18);
    overflow: hidden;
}

.video-box video {
    width: 100%;
    display: block;
    border-radius: 12px;
}

@media (max-width: 600px) {

    .video-profile {
        padding: 60px 18px;
    }

    .video-box {
        padding: 5px;
        border-radius: 12px;
    }

}
    </style>
</head>

<body>

<!-- =========================
     NAVBAR
========================= -->

<header>
    <nav class="navbar">

        <a href="#home" class="logo">

            <img
                src="GAMBAR/LOGO SDN 001 UKUI.jpg"
                alt="Logo SDN 001 Ukui"
                class="school-logo"
            >

            <div class="logo-text">
                <h2>SDN 001 UKUI</h2>
                <span>Sekolah Dasar Negeri</span>
            </div>

        </a>

        <ul class="nav-menu" id="navMenu">
            <li><a href="#home">Beranda</a></li>
            <li><a href="#profil">Profil</a></li>
            <li><a href="#program">Program</a></li>
            <li><a href="#berita">Berita</a></li>
            <li><a href="#galeri">Galeri</a></li>
            <li><a href="#kontak">Kontak</a></li>
        </ul>

        <button class="menu-btn" onclick="toggleMenu()">
            ☰
        </button>

    </nav>
</header>


<!-- =========================
     HERO
========================= -->

<section class="hero" id="home">

    <div class="hero-content">

        <div class="hero-grid">

            <!-- BAGIAN KIRI -->
            <div class="hero-text">

                <small>🌟 WEBSITE RESMI SEKOLAH</small>

                <h1>
                    Selamat Datang di
                    <span>SDN 001 Ukui</span>
                </h1>

                <p>
                    Mewujudkan sekolah dasar yang unggul, berkarakter,
                    berbudaya, berwawasan digital serta peduli terhadap lingkungan.
                </p>

                <div class="hero-buttons">

                    <a href="#profil" class="btn btn-primary">
                        Jelajahi Sekolah
                    </a>

                    <a href="#kontak" class="btn btn-outline">
                        Hubungi Kami
                    </a>

                </div>

            </div>


            <!-- BAGIAN KANAN FOTO KEPALA SEKOLAH -->
            <div class="kepsek-card">

                <img
                    src="GAMBAR/KEPSEK"
                    alt="Kepala Sekolah SDN 001 Ukui">

                <h3>Nova Sepriyanti, S.Pd.</h3>

                <p>Kepala SDN 001 Ukui</p>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     PROFIL
========================= -->

<section class="about" id="profil">

    <div class="container">

        <div class="section-title">
            <span>Tentang Sekolah</span>
            <h2>Profil SDN 001 Ukui</h2>

            <p>
                Mengenal lebih dekat lingkungan, visi dan komitmen
                SDN 001 Ukui dalam memberikan pendidikan terbaik.
            </p>
        </div>


        <div class="about-grid">

           <div class="about-grid">

    <div class="about-image">
        <img
            src="VIDIO/PROFIL SDN 001 UKUI.MOV"
            alt="SDN 001 Ukui">
    </div>

            <div class="about-text">

                <h3>
                    Pendidikan untuk Masa Depan
                </h3>

                <p>
                    SDN 001 Ukui berkomitmen menciptakan lingkungan
                    pembelajaran yang aman, nyaman, aktif dan menyenangkan
                    bagi seluruh peserta didik.
                </p>

                <p>
                    Pembelajaran diarahkan untuk mengembangkan potensi
                    akademik, karakter, kreativitas, keterampilan dan
                    kepedulian terhadap lingkungan.
                </p>

                <div class="vision">
                    <strong>Visi Sekolah</strong>
                    <p>
                        Terwujudnya sekolah dasar yang unggul,
                        berkarakter, berbudaya, berwawasan digital
                        serta lingkungan.
                    </p>
                </div>

            </div>

        </div>

    </div>

</section>
<!-- =========================
     VIDEO PROFIL SEKOLAH
========================= -->

<section class="video-profile">

    <div class="container">

        <div class="section-title">
            <span>VIDEO PROFIL</span>
            <h2>Mengenal SDN 001 Ukui</h2>
            <p>
                Saksikan video profil SDN 001 Ukui
                untuk mengenal lebih dekat sekolah,
                guru, peserta didik, dan berbagai kegiatan sekolah.
            </p>
        </div>

        <div class="video-box">

            <video controls>
                <source src="VIDIO/PROFIL SDN 001 UKUI.MOV">
                Browser Anda tidak mendukung pemutar video.
            </video>

        </div>

    </div>

</section>

<!-- =========================
     STATISTIK
========================= -->

<section class="stats">

    <div class="container">

        <div class="stats-grid">

            <div class="stat">
                <h3>01</h3>
                <p>Sekolah Dasar</p>
            </div>

            <div class="stat">
                <h3>06</h3>
                <p>Tingkat Kelas</p>
            </div>

            <div class="stat">
                <h3>24/7</h3>
                <p>Semangat Belajar</p>
            </div>

            <div class="stat">
                <h3>100%</h3>
                <p>Untuk Pendidikan</p>
            </div>

        </div>

    </div>

</section>


<!-- =========================
     PROGRAM
========================= -->

<section id="program">

    <div class="container">

        <div class="section-title">
            <span>Program Sekolah</span>
            <h2>Program Unggulan</h2>

            <p>
                Berbagai kegiatan yang mendukung perkembangan
                akademik dan karakter peserta didik.
            </p>
        </div>


        <div class="program-grid">

            <div class="program-card">
                <div class="icon">📚</div>

                <h3>Pembelajaran Mendalam</h3>

                <p>
                    Pembelajaran yang mendorong peserta didik
                    memahami materi secara lebih bermakna.
                </p>
            </div>


            <div class="program-card">
                <div class="icon">💻</div>

                <h3>Pembelajaran Digital</h3>

                <p>
                    Pemanfaatan teknologi untuk mendukung
                    pembelajaran yang kreatif dan inovatif.
                </p>
            </div>


            <div class="program-card">
                <div class="icon">🏕️</div>

                <h3>Pramuka</h3>

                <p>
                    Membentuk peserta didik yang mandiri,
                    disiplin, bertanggung jawab dan berkarakter.
                </p>
            </div>


            <div class="program-card">
                <div class="icon">🥁</div>

                <h3>Drumband</h3>

                <p>
                    Mengembangkan bakat, kreativitas,
                    kekompakan dan kepercayaan diri siswa.
                </p>
            </div>


            <div class="program-card">
                <div class="icon">⚽</div>

                <h3>Olahraga</h3>

                <p>
                    Mendorong peserta didik untuk hidup sehat
                    dan mengembangkan potensi olahraga.
                </p>
            </div>


            <div class="program-card">
                <div class="icon">🌱</div>

                <h3>Peduli Lingkungan</h3>

                <p>
                    Membiasakan peserta didik menjaga kebersihan
                    dan kelestarian lingkungan sekolah.
                </p>
            </div>

        </div>

    </div>

</section>


<!-- =========================
     BERITA
========================= -->

<section class="news" id="berita">

    <div class="container">

        <div class="section-title">
            <span>Informasi Sekolah</span>
            <h2>Berita & Kegiatan</h2>

            <p>
                Informasi terbaru mengenai kegiatan
                SDN 001 Ukui.
            </p>
        </div>


        <div class="news-grid">

            <article class="news-card">

                <img
                    src="GAMBAR/KEGIATAN SEKOLAH.jpeg"
                    alt="Kegiatan sekolah">

                <div class="news-body">

                    <div class="date">
                        KEGIATAN SEKOLAH
                    </div>

                    <h3>
                        Kegiatan Pembelajaran Siswa
                    </h3>

                    <p>
                        Berbagai kegiatan pembelajaran dilaksanakan
                        untuk meningkatkan pengalaman belajar siswa.
                    </p>

                </div>

            </article>


            <article class="news-card">

                <img
                    src="GAMBAR/PRAMUKA"
                    alt="Pramuka">

                <div class="news-body">

                    <div class="date">
                        EKSTRAKURIKULER
                    </div>

                    <h3>
                        Kegiatan Pramuka
                    </h3>

                    <p>
                        Kegiatan kepramukaan sebagai sarana membentuk
                        karakter dan kemandirian peserta didik.
                    </p>

                </div>

            </article>


            <article class="news-card">

                <img
                    src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?auto=format&fit=crop&w=800&q=80"
                    alt="Pendidikan">

                <div class="news-body">

                    <div class="date">
                        PENDIDIKAN
                    </div>

                    <h3>
                        Semangat Belajar Siswa
                    </h3>

                    <p>
                        Sekolah terus mendorong peserta didik
                        untuk aktif, kreatif dan berprestasi.
                    </p>

                </div>

            </article>

        </div>

    </div>

</section>


<!-- =========================
     GALERI
========================= -->

<section id="galeri">

    <div class="container">

        <div class="section-title">
            <span>Dokumentasi</span>
            <h2>Galeri Sekolah</h2>

            <p>
                Dokumentasi kegiatan dan aktivitas
                peserta didik SDN 001 Ukui.
            </p>
        </div>


        <div class="gallery-grid">

            <img
                src="https://images.unsplash.com/photo-1509062522246-3755977927d7?auto=format&fit=crop&w=800&q=80"
                alt="Galeri sekolah">

            <img
                src="https://images.unsplash.com/photo-1580582932707-520aed937b7b?auto=format&fit=crop&w=800&q=80"
                alt="Gedung sekolah">

            <img
                src="https://images.unsplash.com/photo-1577896851231-70ef18881754?auto=format&fit=crop&w=800&q=80"
                alt="Kegiatan siswa">

            <img
                src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?auto=format&fit=crop&w=800&q=80"
                alt="Pembelajaran">

        </div>

    </div>

</section>


<!-- =========================
     KONTAK
========================= -->

<section class="contact" id="kontak">

    <div class="container">

        <div class="section-title">
            <span>Hubungi Kami</span>
            <h2>Kontak Sekolah</h2>

            <p>
                Silakan menghubungi SDN 001 Ukui
                untuk mendapatkan informasi lebih lanjut.
            </p>
        </div>


        <div class="contact-grid">

            <div class="contact-box">

                <div class="contact-item">

                    <div class="contact-icon">
                        📍
                    </div>

                    <div>
                        <h4>Alamat</h4>
                        <p>
                            SDN 001 Ukui, Kecamatan Ukui,
                            Kabupaten Pelalawan, Riau
                        </p>
                    </div>

                </div>


                <div class="contact-item">

                    <div class="contact-icon">
                        📞
                    </div>

                    <div>
                        <h4>Telepon</h4>
                        <p>
                            Silakan tambahkan nomor sekolah
                        </p>
                    </div>

                </div>


                <div class="contact-item">

                    <div class="contact-icon">
                        ✉️
                    </div>

                    <div>
                        <h4>Email</h4>
                        <p>
                            Silakan tambahkan email sekolah
                        </p>
                    </div>

                </div>


                <div class="contact-item">

                    <div class="contact-icon">
                        🕘
                    </div>

                    <div>
                        <h4>Jam Sekolah</h4>
                        <p>
                            Senin - Sabtu
                        </p>
                    </div>

                </div>

            </div>


            <div>

                <iframe
                    class="map"
                    src="https://www.google.com/maps?q=Ukui%20Pelalawan%20Riau&output=embed"
                    loading="lazy">
                </iframe>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     FOOTER
========================= -->

<footer>

    <div class="footer-grid">

        <div>

            <h3>SDN 001 Ukui</h3>

            <p>
                Terwujudnya sekolah dasar yang unggul,
                berkarakter, berbudaya, berwawasan digital
                serta lingkungan.
            </p>

        </div>


        <div>

            <h3>Menu</h3>

            <ul class="footer-links">
                <li><a href="#home">Beranda</a></li>
                <li><a href="#profil">Profil</a></li>
                <li><a href="#program">Program</a></li>
                <li><a href="#berita">Berita</a></li>
                <li><a href="#galeri">Galeri</a></li>
            </ul>

        </div>


        <div>

            <h3>Informasi</h3>

            <ul class="footer-links">
                <li>SDN 001 Ukui</li>
                <li>Kabupaten Pelalawan</li>
                <li>Provinsi Riau</li>
                <li>Indonesia</li>
            </ul>

        </div>

    </div>


    <div class="copyright">

        © 2026 SDN 001 Ukui. Semua Hak Dilindungi.

    </div>

</footer>


<!-- =========================
     WHATSAPP
========================= -->

<a
    class="whatsapp"
    href="https://wa.me/6280000000000"
    target="_blank"
    title="Hubungi WhatsApp">
    ☎
</a>


<script>

    function toggleMenu() {

        const menu = document.getElementById("navMenu");

        menu.classList.toggle("active");

    }


    document.querySelectorAll(".nav-menu a").forEach(link => {

        link.addEventListener("click", () => {

            document
                .getElementById("navMenu")
                .classList.remove("active");

        });

    });

</script>

</body>
</html>
