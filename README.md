<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Brilliant Sukma Mahardika | Portofolio</title>
    <meta name="description" content="Portofolio Brilliant Sukma Mahardika - Programmer, Designer & Tech Enthusiast">

    <!-- Bootstrap 5 -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet">

    <!-- Bootstrap Icons -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.13.1/font/bootstrap-icons.min.css" rel="stylesheet">

    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg: #080b12;
            --bg2: #0e131d;
            --card: rgba(255,255,255,.05);
            --border: rgba(255,255,255,.10);
            --text: #f5f7fb;
            --muted: #9ca3af;
            --primary: #7c5cff;
            --secondary: #00d4ff;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 80px;
        }

        body {
            font-family: "Inter", sans-serif;
            background: var(--bg);
            color: var(--text);
            line-height: 1.6;
        }

        .navbar {
            background: rgba(8, 11, 18, .82) !important;
            backdrop-filter: blur(15px);
            border-bottom: 1px solid var(--border);
        }

        .navbar-brand {
            font-weight: 800;
            font-size: 1.4rem;
        }

        .navbar-brand span {
            color: var(--primary);
        }

        .nav-link {
            color: var(--muted) !important;
            transition: .3s;
        }

        .nav-link:hover,
        .nav-link.active {
            color: #fff !important;
        }

        .hero {
            min-height: 100vh;
            padding-top: 120px;
            padding-bottom: 80px;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            background:
                radial-gradient(circle at 85% 25%, rgba(124,92,255,.18), transparent 28%),
                radial-gradient(circle at 70% 75%, rgba(0,212,255,.08), transparent 25%),
                var(--bg);
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 8px 15px;
            border: 1px solid var(--border);
            border-radius: 50px;
            color: #c8c1ff;
            background: rgba(124,92,255,.08);
            font-size: .85rem;
        }

        .hero h1 {
            font-size: clamp(3rem, 7vw, 5.4rem);
            line-height: 1.05;
            font-weight: 800;
            letter-spacing: -4px;
        }

        .gradient-text {
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .hero p,
        .text-muted-custom {
            color: var(--muted) !important;
        }

        .btn-gradient {
            color: #fff;
            background: linear-gradient(135deg, var(--primary), #5940db);
            border: none;
        }

        .btn-gradient:hover {
            color: #fff;
            transform: translateY(-3px);
        }

        .btn-outline-custom {
            color: #fff;
            border: 1px solid var(--border);
            background: var(--card);
        }

        .btn-outline-custom:hover {
            color: #fff;
            border-color: var(--primary);
            background: rgba(124,92,255,.10);
            transform: translateY(-3px);
        }

        .section-padding {
            padding: 100px 0;
        }

        .section-label {
            color: var(--primary);
            font-weight: 700;
            letter-spacing: .08em;
            font-size: .8rem;
        }

        .section-title {
            font-weight: 800;
        }

        .glass-card {
            background: var(--card);
            border: 1px solid var(--border);
            border-radius: 20px;
            transition: .3s;
        }

        .glass-card:hover {
            transform: translateY(-7px);
            border-color: rgba(124,92,255,.7);
        }

        .about-image {
            min-height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 100px;
            border-radius: 25px;
            border: 1px solid var(--border);
            background:
                radial-gradient(circle at 30% 30%, rgba(124,92,255,.35), transparent 35%),
                linear-gradient(135deg, #111827, #080b12);
        }

        .skill-icon {
            font-size: 2rem;
            color: #bdb3ff;
        }

        .project-image {
            height: 200px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            background: linear-gradient(135deg, #7c5cff, #00bcd4);
        }

        .tag {
            display: inline-block;
            font-size: .7rem;
            padding: 5px 9px;
            margin: 3px;
            border-radius: 5px;
            background: rgba(124,92,255,.15);
            color: #c9c0ff;
        }

        .contact-box {
            background: linear-gradient(135deg, rgba(124,92,255,.12), rgba(0,212,255,.05));
        }

        .social-link {
            color: #fff;
            text-decoration: none;
            border: 1px solid var(--border);
            border-radius: 8px;
            transition: .3s;
        }

        .social-link:hover {
            color: #fff;
            border-color: var(--primary);
            transform: translateY(-3px);
        }

        footer {
            border-top: 1px solid var(--border);
            color: var(--muted);
        }

        .reveal {
            opacity: 0;
            transform: translateY(25px);
            transition: .8s ease;
        }

        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }

        @media (max-width: 576px) {
            .hero h1 {
                letter-spacing: -2px;
            }

            .section-padding {
                padding: 75px 0;
            }

            .about-image {
                min-height: 280px;
                font-size: 70px;
            }
        }
    </style>
</head>

<body>

<!-- NAVBAR -->
<nav class="navbar navbar-expand-lg navbar-dark fixed-top">
    <div class="container">
        <a class="navbar-brand" href="#home">Brilliant<span>.</span></a>

        <button class="navbar-toggler" type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarNav"
                aria-controls="navbarNav"
                aria-expanded="false"
                aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto gap-lg-3">
                <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
                <li class="nav-item"><a class="nav-link" href="#skills">Skills</a></li>
                <li class="nav-item"><a class="nav-link" href="#journey">Journey</a></li>
                <li class="nav-item"><a class="nav-link" href="#projects">Projects</a></li>
                <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
            </ul>
        </div>
    </div>
</nav>

<!-- HERO -->
<section class="hero" id="home">
    <div class="container">
        <div class="row align-items-center">
            <div class="col-lg-9 reveal">
                <div class="hero-badge mb-4 shadow-sm">
                    <i class="bi bi-hand-wave"></i>
                    Welcome to my portofolio
                </div>

                <h1>
                    Hi, I'm <span class="gradient-text">Brilliant</span><br>
                    Web Developer.
                </h1>

                <img src="foto.jpg" width="150" height="200" alt="foto">

                <p class="lead mt-4 mb-0 col-lg-9">
                    Saya seorang programmer dan technology enthusiast
                    yang suka membangun website modern, aplikasi,
                    dan berbagai project digital.
                </p>

                <div class="d-flex flex-wrap gap-3 mt-4">
                    <a href="#projects" class="btn btn-gradient btn-lg px-4">
                        Lihat Project <i class="bi bi-arrow-right"></i>
                    </a>
                    <a href="#contact" class="btn btn-outline-custom btn-lg px-4">
                        Hubungi Saya
                    </a>
                </div>

                <div class="d-flex flex-wrap gap-4 mt-5 small text-muted-custom">
                    <span><i class="bi bi-geo-alt me-2"></i>Indonesia</span>
                    <span><i class="bi bi-code-slash me-2"></i>Web Development</span>
                    <span><i class="bi bi-controller me-2"></i>Gaming</span>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- QUICK STATS -->
<section class="py-4">
    <div class="container">
        <div class="row g-3">
            <div class="col-6 col-lg-3 reveal">
                <div class="glass-card text-center p-4 h-100">
                    <div class="display-6 fw-bold gradient-text">8+</div>
                    <div class="small text-muted-custom">Skills & Technologies</div>
                </div>
            </div>
            <div class="col-6 col-lg-3 reveal">
                <div class="glass-card text-center p-4 h-100">
                    <div class="display-6 fw-bold gradient-text">3+</div>
                    <div class="small text-muted-custom">portofolio Projects</div>
                </div>
            </div>
            <div class="col-6 col-lg-3 reveal">
                <div class="glass-card text-center p-4 h-100">
                    <div class="display-6 fw-bold gradient-text">S1</div>
                    <div class="small text-muted-custom">Teknik Informatika</div>
                </div>
            </div>
            <div class="col-6 col-lg-3 reveal">
                <div class="glass-card text-center p-4 h-100">
                    <div class="display-6 fw-bold gradient-text">2026</div>
                    <div class="small text-muted-custom">portofolio Edition</div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- ABOUT -->
<section id="about" class="section-padding">
    <div class="container">
        <div class="text-center mb-5 reveal">
            <div class="section-label">ABOUT ME</div>
            <h2 class="section-title display-6 mt-2">Tentang Saya</h2>
        </div>

        <div class="row align-items-center g-5">
            <div class="col-lg-6 reveal">
                <div class="about-image">💻</div>
            </div>

            <div class="col-lg-6 reveal">
                <h3 class="fw-bold mb-4">Building ideas into digital experiences.</h3>

                <p class="text-muted-custom">
                    Saya memiliki ketertarikan pada dunia programming,
                    web development, desain, dan teknologi.
                </p>

                <p class="text-muted-custom">
                    Saya senang mempelajari teknologi baru dan
                    mengubah ide menjadi website yang sederhana,
                    cepat, dan mudah digunakan.
                </p>

                <p class="text-muted-custom mb-0">
                    Saat ini saya fokus mengembangkan kemampuan
                    dalam web development dan software development.
                </p>
            </div>
        </div>
    </div>
</section>

<!-- SKILLS -->
<section id="skills" class="section-padding bg-black bg-opacity-25">
    <div class="container">
        <div class="text-center mb-5 reveal">
            <div class="section-label">MY SKILLS</div>
            <h2 class="section-title display-6 mt-2">Teknologi yang Saya Gunakan</h2>
            <p class="text-muted-custom mx-auto col-lg-7">
                Beberapa teknologi yang saya pelajari dan gunakan
                untuk membuat berbagai project.
            </p>
        </div>

        <div class="row g-4">
            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-code-slash"></i></div>
                    <h5 class="fw-bold">HTML</h5>
                    <p class="text-muted-custom small mb-0">Semantic structure dan modern web layout.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-palette"></i></div>
                    <h5 class="fw-bold">CSS</h5>
                    <p class="text-muted-custom small mb-0">Responsive design, animation dan UI styling.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-lightning-charge"></i></div>
                    <h5 class="fw-bold">JavaScript</h5>
                    <p class="text-muted-custom small mb-0">Interactive website dan dynamic functionality.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-filetype-py"></i></div>
                    <h5 class="fw-bold">Python</h5>
                    <p class="text-muted-custom small mb-0">Programming, automation dan backend basics.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-filetype-php"></i></div>
                    <h5 class="fw-bold">PHP</h5>
                    <p class="text-muted-custom small mb-0">Server-side programming dan web development.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-box"></i></div>
                    <h5 class="fw-bold">Java</h5>
                    <p class="text-muted-custom small mb-0">.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-database"></i></div>
                    <h5 class="fw-bold">Database</h5>
                    <p class="text-muted-custom small mb-0">Pengelolaan data menggunakan database relational.</p>
                </div>
            </div>

            <div class="col-sm-6 col-lg-3 reveal">
                <div class="glass-card h-100 p-4">
                    <div class="skill-icon mb-3"><i class="bi bi-controller"></i></div>
                    <h5 class="fw-bold">Gaming</h5>
                    <p class="text-muted-custom small mb-0">Tech enthusiast dan gaming enthusiast.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- JOURNEY -->
<section id="journey" class="section-padding bg-black bg-opacity-25">
    <div class="container">
        <div class="text-center mb-5 reveal">
            <div class="section-label">MY JOURNEY</div>
            <h2 class="section-title display-6 mt-2">Perjalanan & Fokus</h2>
            <p class="text-muted-custom mx-auto col-lg-7">
                Fokus saya adalah terus membangun skill dan project yang bisa
                menjadi bukti kemampuan secara nyata.
            </p>
        </div>

        <div class="row g-4 justify-content-center">
            <div class="col-lg-8">
                <div class="glass-card p-4 p-md-5 reveal">
                    <div class="d-flex gap-3">
                        <div class="skill-icon flex-shrink-0">
                            <i class="bi bi-mortarboard"></i>
                        </div>
                        <div>
                            <h5 class="fw-bold">Teknik Informatika</h5>
                            <p class="text-muted-custom mb-3">
                                Memiliki dasar pemrograman, algoritma, pengembangan
                                aplikasi dan teknologi komputer.
                            </p>
                            <span class="tag">Programming</span>
                            <span class="tag">Software</span>
                            <span class="tag">Technology</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col-lg-8">
                <div class="glass-card p-4 p-md-5 reveal">
                    <div class="d-flex gap-3">
                        <div class="skill-icon flex-shrink-0">
                            <i class="bi bi-window-stack"></i>
                        </div>
                        <div>
                            <h5 class="fw-bold">Web Development</h5>
                            <p class="text-muted-custom mb-3">
                                Fokus mengembangkan website modern menggunakan
                                HTML, CSS, JavaScript, PHP, Bootstrap dan Laravel.
                            </p>
                            <span class="tag">Bootstrap 5</span>
                            <span class="tag">Laravel</span>
                            <span class="tag">PHP</span>
                            <span class="tag">JavaScript</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col-lg-8">
                <div class="glass-card p-4 p-md-5 reveal">
                    <div class="d-flex gap-3">
                        <div class="skill-icon flex-shrink-0">
                            <i class="bi bi-rocket-takeoff"></i>
                        </div>
                        <div>
                            <h5 class="fw-bold">Current Goal</h5>
                            <p class="text-muted-custom mb-3">
                                Membuat portofolio dan project yang lebih profesional
                                untuk menunjukkan kemampuan kepada calon perusahaan
                                atau client.
                            </p>
                            <span class="tag">portofolio</span>
                            <span class="tag">Freelance</span>
                            <span class="tag">Career</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- PROJECTS -->
<section id="projects" class="section-padding">
    <div class="container">
        <div class="text-center mb-5 reveal">
            <div class="section-label">MY WORK</div>
            <h2 class="section-title display-6 mt-2">Project Saya</h2>
            <p class="text-muted-custom mx-auto col-lg-7">
                Beberapa project yang dapat ditampilkan di portofolio.
            </p>
        </div>

        <div class="row g-4">
            <div class="col-lg-4 reveal">
                <div class="glass-card overflow-hidden h-100">
                    <div class="project-image">🛒</div>
                    <div class="p-4">
                        <h4 class="fw-bold">Sistem Pendataan Stok Barang</h4>
                        <p class="text-muted-custom small">
                           Sistem untuk menambah, mengubah, menghapus data barang.
                        </p>
                        <div class="mb-3">
                            <span class="tag">HTML</span>
                            <span class="tag">CSS</span>
                            <span class="tag">JavaScript</span>
                            <span class="tag">PHP</span>
                        </div>
                        <a href="#contact" class="btn btn-sm btn-outline-custom">
                            Detail Project <i class="bi bi-arrow-right"></i>
                        </a>
                    </div>
                </div>
            </div>

            <div class="col-lg-4 reveal">
                <div class="glass-card overflow-hidden h-100">
                    <div class="project-image">📊</div>
                    <div class="p-4">
                        <h4 class="fw-bold">Dashboard Admin</h4>
                        <p class="text-muted-custom small">
                            Dashboard administrator untuk mengelola
                            data dan informasi aplikasi.
                        </p>
                        <div class="mb-3">
                            <span class="tag">Laravel</span>
                            <span class="tag">PHP</span>
                            <span class="tag">SQLite</span>
                        </div>
                        <a href="#contact" class="btn btn-sm btn-outline-custom">
                            Detail Project <i class="bi bi-arrow-right"></i>
                        </a>
                    </div>
                </div>
            </div>

            <div class="col-lg-4 reveal">
                <div class="glass-card overflow-hidden h-100">
                    <div class="project-image">📝</div>
                    <div class="p-4">
                        <h4 class="fw-bold">Task Management</h4>
                        <p class="text-muted-custom small">
                            Aplikasi sederhana untuk membuat,
                            mengedit dan menyelesaikan task.
                        </p>
                        <div class="mb-3">
                            <span class="tag">JavaScript</span>
                            <span class="tag">HTML</span>
                            <span class="tag">CSS</span>
                        </div>
                        <a href="#contact" class="btn btn-sm btn-outline-custom">
                            Detail Project <i class="bi bi-arrow-right"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- CTA -->
<section class="section-padding pt-0">
    <div class="container">
        <div class="glass-card p-4 p-md-5 reveal">
            <div class="row align-items-center g-4">
                <div class="col-lg-8">
                    <div class="section-label mb-2">READY TO CONNECT?</div>
                    <h3 class="fw-bold mb-2">Mari buat sesuatu yang keren bersama.</h3>
                    <p class="text-muted-custom mb-0">
                        Terbuka untuk diskusi project, web development,
                        teknologi dan peluang kerja.
                    </p>
                </div>
                <div class="col-lg-4 text-lg-end">
                    <a href="#contact" class="btn btn-gradient px-4 py-3">
                        Let's Talk <i class="bi bi-arrow-up-right"></i>
                    </a>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- CONTACT -->
<section id="contact" class="section-padding">
    <div class="container">
        <div class="contact-box glass-card text-center p-4 p-md-5 reveal">
            <h2 class="display-6 fw-bold">Let's work together.</h2>
            <p class="text-muted-custom mx-auto col-lg-7 my-3">
                Punya project atau ingin berdiskusi mengenai
                teknologi? Silakan hubungi saya.
            </p>

            <div class="d-flex flex-wrap justify-content-center gap-3 mt-4">
                <a href="mailto:brylee.wu@gmail.com" class="social-link px-4 py-2">
                    <i class="bi bi-envelope"></i> Email
                </a>

                <a href="https://id.linkedin.com/in/brilliant-sukma-mahardika-5004911ab"
                   target="_blank" class="social-link px-4 py-2">
                    <i class="bi bi-linkedin"></i> LinkedIn
                </a>

                <a href="#" class="social-link px-4 py-2">
                    <i class="bi bi-github"></i> GitHub
                </a>

                <a href="https://www.instagram.com/brilliantsm_/"
                   target="_blank" class="social-link px-4 py-2">
                    <i class="bi bi-instagram"></i> Instagram
                </a>
            </div>
        </div>
    </div>
</section>

<!-- FOOTER -->
<footer class="py-4 text-center">
    <div class="container">
        <small>© 2026 Brilliant Sukma Mahardika. All rights reserved.</small>
    </div>
</footer>

<!-- Bootstrap 5 JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js"></script>

<script>
    // Scroll reveal animation
    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add("active");
            }
        });
    }, { threshold: 0.15 });

    document.querySelectorAll(".reveal").forEach(element => {
        observer.observe(element);
    });

    // Active navbar link
    const sections = document.querySelectorAll("section[id]");
    const navLinks = document.querySelectorAll(".nav-link");

    window.addEventListener("scroll", () => {
        let current = "";

        sections.forEach(section => {
            const sectionTop = section.offsetTop - 120;
            if (window.scrollY >= sectionTop) {
                current = section.getAttribute("id");
            }
        });

        navLinks.forEach(link => {
            link.classList.remove("active");
            if (link.getAttribute("href") === "#" + current) {
                link.classList.add("active");
            }
        });
    });

    // Close Bootstrap mobile navbar after clicking a link
    document.querySelectorAll(".navbar-nav .nav-link").forEach(link => {
        link.addEventListener("click", () => {
            const navbar = document.querySelector(".navbar-collapse");
            if (navbar.classList.contains("show")) {
                bootstrap.Collapse.getOrCreateInstance(navbar).hide();
            }
        });
    });
</script>

</body>
</html>
