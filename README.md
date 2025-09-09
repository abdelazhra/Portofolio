# Portofolio
about me
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Abdel Azhra - UX Researcher & Data Analyst</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            /* Modern gradient background */
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: #1e293b;
        }
        
        /* Alternative backgrounds - uncomment one to use */
        
        /* Option 1: Dark mode with purple gradient
        body {
            background: linear-gradient(135deg, #1e1b4b 0%, #312e81 50%, #1e3a8a 100%);
            color: #f8fafc;
        }
        */
        
        /* Option 2: Warm sunset gradient
        body {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: #1e293b;
        }
        */
        
        /* Option 3: Ocean blue gradient
        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #1e293b;
        }
        */
        
        /* Option 4: Forest green gradient
        body {
            background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);
            color: #1e293b;
        }
        */
        
        .gradient-text {
            background: linear-gradient(to right, #4f46e5, #14b8a6);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .section-title {
            border-bottom: 3px solid #4f46e5;
            padding-bottom: 8px;
            display: inline-block;
        }
        .card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.15), 0 10px 10px -5px rgba(0, 0, 0, 0.1);
            background: rgba(255, 255, 255, 1);
        }
        .link-button {
             display: inline-block;
             background-color: rgba(238, 242, 255, 0.9);
             color: #4338ca;
             font-weight: 600;
             padding: 8px 16px;
             border-radius: 9999px;
             transition: all 0.3s ease;
             text-decoration: none;
             border: 1px solid rgba(255, 255, 255, 0.3);
        }
        .link-button:hover {
            background-color: #e0e7ff;
            transform: translateY(-2px);
        }
        
        /* Glass morphism effect for sections */
        .glass-section {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 20px;
        }
        
        /* Enhanced header with glass effect */
        .glass-header {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(15px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        /* Color scheme selector */
        .color-selector {
            position: fixed;
            top: 50%;
            right: 20px;
            transform: translateY(-50%);
            z-index: 1000;
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 15px;
            box-shadow: 0 8px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .color-option {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            margin: 5px 0;
            cursor: pointer;
            border: 3px solid white;
            transition: transform 0.2s ease;
        }
        
        .color-option:hover {
            transform: scale(1.1);
        }
    </style>
</head>
<body class="antialiased">

    <!-- Color Selector -->
    <div class="color-selector">
        <div class="text-xs font-semibold text-gray-600 mb-2 text-center">Themes</div>
        <div class="color-option" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);" onclick="changeTheme('ocean')"></div>
        <div class="color-option" style="background: linear-gradient(135deg, #1e1b4b 0%, #312e81 50%, #1e3a8a 100%);" onclick="changeTheme('dark')"></div>
        <div class="color-option" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);" onclick="changeTheme('sunset')"></div>
        <div class="color-option" style="background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);" onclick="changeTheme('forest')"></div>
        <div class="color-option" style="background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%);" onclick="changeTheme('pink')"></div>
    </div>

    <!-- Header & Navigasi -->
    <header class="glass-header shadow-lg sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <div class="text-2xl font-bold text-white">
                <a href="#" class="drop-shadow-sm">Abdel Azhra</a>
            </div>
            <ul class="hidden md:flex space-x-8 text-white font-semibold">
                <li><a href="#about" class="hover:text-yellow-300 transition drop-shadow-sm">Tentang Saya</a></li>
                <li><a href="#skills" class="hover:text-yellow-300 transition drop-shadow-sm">Kompetensi</a></li>
                <li><a href="#project" class="hover:text-yellow-300 transition drop-shadow-sm">Proyek Unggulan</a></li>
                <li><a href="#certs" class="hover:text-yellow-300 transition drop-shadow-sm">Sertifikasi</a></li>
                <li><a href="#contact" class="hover:text-yellow-300 transition drop-shadow-sm">Kontak</a></li>
            </ul>
            <button id="mobile-menu-button" class="md:hidden text-white">
                <i class="fas fa-bars fa-lg drop-shadow-sm"></i>
            </button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden px-6 pt-2 pb-4">
             <ul class="flex flex-col space-y-4 text-white font-semibold">
                <li><a href="#about" class="block hover:text-yellow-300 transition">Tentang Saya</a></li>
                <li><a href="#skills" class="block hover:text-yellow-300 transition">Kompetensi</a></li>
                <li><a href="#project" class="block hover:text-yellow-300 transition">Proyek Unggulan</a></li>
                <li><a href="#certs" class="block hover:text-yellow-300 transition">Sertifikasi</a></li>
                <li><a href="#contact" class="block hover:text-yellow-300 transition">Kontak</a></li>
            </ul>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section id="hero" class="py-24 md:py-32">
            <div class="container mx-auto px-6 text-center">
                <h1 class="text-4xl md:text-6xl font-bold text-white leading-tight drop-shadow-lg">
                    <span class="block">Abdel Azhra</span>
                    <span class="gradient-text block mt-2">UX Researcher & Data Analyst</span>
                </h1>
                <p class="mt-6 max-w-2xl mx-auto text-lg text-white/90 drop-shadow-sm">
                    Mahasiswa Computer Science di Binus University dengan fokus pada riset pengalaman pengguna (UX) dan analisis data untuk menciptakan produk digital yang intuitif dan berdampak positif.
                </p>
                <a href="#project" class="mt-8 inline-block bg-white/20 backdrop-blur-sm text-white font-bold py-3 px-8 rounded-full hover:bg-white/30 transition transform hover:scale-105 border border-white/30">Lihat Proyek Saya</a>
            </div>
        </section>

        <!-- Tentang Saya -->
        <section id="about" class="py-20">
            <div class="container mx-auto px-6">
                <div class="glass-section p-8 md:p-12 mx-4">
                    <h2 class="section-title text-3xl font-bold mb-12 text-center text-white">Tentang Saya</h2>
                    <div class="max-w-3xl mx-auto text-center text-white/90 leading-relaxed">
                        <p>
                            Sebagai mahasiswa Computer Science, saya memiliki ketertarikan mendalam pada titik temu antara teknologi dan perilaku manusia. Melalui program Enrichment *Self Study Independence*, saya berkesempatan untuk terjun langsung ke dalam siklus hidup pengembangan produk—mulai dari identifikasi masalah, perancangan metodologi riset, analisis data, hingga validasi konsep.
                        </p>
                        <p class="mt-4">
                            Proyek BeeFit menjadi kanvas saya untuk mengaplikasikan ilmu dalam sebuah tim kolaboratif, di mana saya belajar bahwa data yang diolah dengan baik dapat menjadi fondasi untuk menciptakan solusi teknologi yang tidak hanya fungsional, tetapi juga berempati pada penggunanya.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Kompetensi -->
        <section id="skills" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title text-3xl font-bold mb-12 text-center text-white">Kompetensi Inti</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                    <div class="card p-8 rounded-xl text-center">
                        <i class="fas fa-users text-4xl text-indigo-500 mb-4"></i>
                        <h3 class="text-xl font-bold mb-2 text-slate-800">UX Research & Analysis</h3>
                        <p class="text-slate-600">Merancang dan melaksanakan studi *usability* menggunakan metode standar seperti System Usability Scale (SUS).</p>
                    </div>
                    <div class="card p-8 rounded-xl text-center">
                        <i class="fas fa-chart-pie text-4xl text-teal-500 mb-4"></i>
                        <h3 class="text-xl font-bold mb-2 text-slate-800">Data Visualization</h3>
                        <p class="text-slate-600">Mengolah data mentah menjadi wawasan bermakna dan memvisualisasikannya dalam dasbor interaktif.</p>
                    </div>
                    <div class="card p-8 rounded-xl text-center">
                        <i class="fas fa-code text-4xl text-sky-500 mb-4"></i>
                        <h3 class="text-xl font-bold mb-2 text-slate-800">Front-End Development</h3>
                        <p class="text-slate-600">Dasar kuat dalam HTML, CSS (Tailwind), dan JavaScript untuk membangun prototipe dan visualisasi data.</p>
                    </div>
                     <div class="card p-8 rounded-xl text-center">
                        <i class="fas fa-hands-helping text-4xl text-violet-500 mb-4"></i>
                        <h3 class="text-xl font-bold mb-2 text-slate-800">Kolaborasi Tim</h3>
                        <p class="text-slate-600">Berkontribusi dalam tim multidisiplin, menjembatani riset dengan pengembangan teknis untuk mencapai tujuan bersama.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Proyek Unggulan: BeeFit -->
        <section id="project" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title text-3xl font-bold mb-4 text-center text-white">Proyek Unggulan</h2>
                <h3 class="text-center text-4xl font-bold gradient-text mb-12">Evaluasi Usability Website Kebugaran BeeFit</h3>
                
                <div class="card rounded-2xl shadow-2xl p-8 md:p-12">
                    <div class="grid grid-cols-1 lg:grid-cols-5 gap-12 items-start">
                        <div class="lg:col-span-3">
                            <h4 class="text-2xl font-bold text-slate-800 mb-4">Problem & Solution</h4>
                            <p class="text-slate-600 mb-2"><b>Problem:</b> Banyak individu kesulitan melacak kebugaran karena kurangnya alat praktis dan panduan yang efektif, sehingga motivasi menurun dan tujuan tidak tercapai.</p>
                            <p class="text-slate-600 mb-6"><b>Solution:</b> BeeFit hadir sebagai aplikasi web yang menyediakan pelacakan intuitif, panduan latihan personal, dan program terstruktur untuk membantu pengguna memulai dan mempertahankan rutinitas dengan percaya diri.</p>
                            
                            <h4 class="text-2xl font-bold text-slate-800 mb-4">Peran Saya dalam Tim</h4>
                            <p class="text-slate-600 mb-4">Dalam tim bersama Wafi Dian Akbar dan Rafael Sinaga, peran saya adalah sebagai **Peneliti Utama dan Analis Data**. Tanggung jawab saya meliputi:</p>
                            <ul class="list-disc list-inside text-slate-600 space-y-2">
                                <li>Merancang metodologi riset *usability* dari awal hingga akhir.</li>
                                <li>Mengumpulkan dan mengolah data dari 29 responden menggunakan metode SUS.</li>
                                <li>Menerjemahkan hasil analisis data menjadi rekomendasi desain yang dapat ditindaklanjuti oleh tim pengembang.</li>
                            </ul>
                        </div>
                        <div class="lg:col-span-2 card bg-gradient-to-br from-indigo-50 to-purple-50 rounded-xl p-6 text-center">
                            <h4 class="text-xl font-bold text-slate-700">Hasil Kunci: Skor Usability</h4>
                            <div class="my-4 h-48">
                                <canvas id="susScoreChart"></canvas>
                            </div>
                            <p class="text-slate-600">Skor rata-rata **72.24** mengonfirmasi bahwa konsep BeeFit memiliki tingkat *usability* **"Baik" (Grade B)**, membuktikan ide ini diterima positif oleh calon pengguna.</p>
                        </div>
                    </div>

                    <div class="mt-12 pt-8 border-t border-slate-200">
                         <h4 class="text-2xl font-bold text-slate-800 mb-6 text-center">Fitur & Keunggulan BeeFit</h4>
                         <div class="grid grid-cols-1 md:grid-cols-3 gap-6 text-left">
                             <div class="bg-gradient-to-br from-blue-50 to-indigo-50 p-6 rounded-xl">
                                 <i class="fas fa-bullseye text-2xl text-indigo-500 mb-3"></i>
                                 <h5 class="font-bold text-slate-700">Workout Planner</h5>
                                 <p class="text-sm text-slate-600">Perencanaan latihan yang terstruktur dan dapat dipersonalisasi sesuai kebutuhan pengguna.</p>
                             </div>
                             <div class="bg-gradient-to-br from-teal-50 to-green-50 p-6 rounded-xl">
                                 <i class="fas fa-utensils text-2xl text-teal-500 mb-3"></i>
                                 <h5 class="font-bold text-slate-700">Diet Plan & Calorie Tracker</h5>
                                 <p class="text-sm text-slate-600">Panduan diet dan pelacak kalori untuk membantu menjaga pola makan yang sehat.</p>
                             </div>
                              <div class="bg-gradient-to-br from-sky-50 to-blue-50 p-6 rounded-xl">
                                 <i class="fas fa-question-circle text-2xl text-sky-500 mb-3"></i>
                                 <h5 class="font-bold text-slate-700">Kuisioner Kesehatan</h5>
                                 <p class="text-sm text-slate-600">Membantu pengguna memahami kebutuhan kesehatan mereka secara personal.</p>
                             </div>
                         </div>
                    </div>
                    
                    <div class="mt-12 pt-8 border-t border-slate-200 text-center">
                         <h4 class="text-2xl font-bold text-slate-800 mb-6">Dokumen Proyek</h4>
                         <div class="flex flex-wrap justify-center gap-4">
                            <a href="./Paper BeeFit (part 3 ).pdf" target="_blank" class="link-button"><i class="fas fa-file-pdf mr-2"></i>Lihat Paper Penelitian</a>
                            <a href="./Infografis BeeFit-1.pdf" target="_blank" class="link-button"><i class="fas fa-image mr-2"></i>Lihat Infografis</a>
                         </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sertifikasi -->
        <section id="certs" class="py-20">
            <div class="container mx-auto px-6">
                <div class="glass-section p-8 md:p-12 mx-4">
                    <h2 class="section-title text-3xl font-bold mb-12 text-center text-white">Sertifikasi & Pembelajaran</h2>
                    <div class="max-w-5xl mx-auto">
                        <p class="text-center text-white/90 mb-8">Selama program Enrichment, saya aktif meningkatkan kompetensi melalui sertifikasi dari freeCodeCamp yang relevan dengan proyek.</p>
                        <div class="grid grid-cols-2 md:grid-cols-3 gap-4 text-center">
                            <div class="card p-4 rounded-xl flex items-center justify-center hover:scale-105 transition-transform">
                               <p class="font-semibold text-indigo-700">Responsive Web Design</p>
                            </div>
                            <div class="card p-4 rounded-xl flex items-center justify-center hover:scale-105 transition-transform">
                               <p class="font-semibold text-indigo-700">Legacy JavaScript Algorithms and Data Structures</p>
                            </div>
                            <div class="card p-4 rounded-xl flex items-center justify-center hover:scale-105 transition-transform">
                               <p class="font-semibold text-indigo-700">Data Visualization</p>
                            </div>
                            <div class="card p-4 rounded-xl flex items-center justify-center hover:scale-105 transition-transform">
                               <p class="font-semibold text-indigo-700">Front End Development Libraries</p>
                            </div>
                             <div class="card p-4 rounded-xl flex items-center justify-center hover:scale-105 transition-transform">
                               <p class="font-semibold text-indigo-700">Machine Learning with Python</p>
                            </div>
                             <div class="card p-4 rounded-xl flex items-center justify-center hover:scale-105 transition-transform">
                               <p class="font-semibold text-indigo-700">Scientific Computing with Python</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Kontak -->
    <footer id="contact" class="py-16">
        <div class="container mx-auto px-6">
            <div class="glass-section p-8 md:p-12 mx-4 text-center">
                <h2 class="text-3xl font-bold text-white mb-4">Mari Terhubung</h2>
                <p class="mb-8 max-w-xl mx-auto text-white/90">Saya terbuka untuk diskusi, kolaborasi, atau peluang di bidang riset UX dan analisis data.</p>
                
                <!-- Contact Information -->
                <div class="mb-8 space-y-4">
                    <div class="flex flex-col md:flex-row justify-center items-center gap-6 text-white/90">
                        <div class="flex items-center gap-2">
                            <i class="fas fa-envelope text-yellow-300"></i>
                            <span class="font-semibold">Email:</span>
                        </div>
                        <div class="flex flex-col md:flex-row gap-4 text-center md:text-left">
                            <a href="mailto:abdel.azhra@binus.ac.id" class="hover:text-yellow-300 transition underline">abdel.azhra@binus.ac.id</a>
                            <span class="hidden md:inline text-white/60">|</span>
                            <a href="mailto:abdelazhra09@gmail.com" class="hover:text-yellow-300 transition underline">abdelazhra09@gmail.com</a>
                        </div>
                    </div>
                    
                    <div class="flex justify-center items-center gap-2 text-white/90">
                        <i class="fas fa-phone text-yellow-300"></i>
                        <span class="font-semibold">WhatsApp:</span>
                        <a href="https://wa.me/628111531906" target="_blank" class="hover:text-yellow-300 transition underline">08111531906</a>
                    </div>
                </div>
                
                <!-- Social Media Icons -->
                <div class="flex justify-center space-x-6 text-3xl mb-8">
                    <a href="mailto:abdel.azhra@binus.ac.id" class="text-white hover:text-yellow-300 transition transform hover:scale-110" aria-label="Email Binus"><i class="fas fa-envelope drop-shadow-sm"></i></a>
                    <a href="mailto:abdelazhra09@gmail.com" class="text-white hover:text-yellow-300 transition transform hover:scale-110" aria-label="Email Gmail"><i class="fas fa-envelope-open drop-shadow-sm"></i></a>
                    <a href="https://wa.me/628111531906" target="_blank" class="text-white hover:text-yellow-300 transition transform hover:scale-110" aria-label="WhatsApp"><i class="fab fa-whatsapp drop-shadow-sm"></i></a>
                    <a href="#" class="text-white hover:text-yellow-300 transition transform hover:scale-110" aria-label="LinkedIn"><i class="fab fa-linkedin drop-shadow-sm"></i></a>
                    <a href="#" class="text-white hover:text-yellow-300 transition transform hover:scale-110" aria-label="GitHub"><i class="fab fa-github drop-shadow-sm"></i></a>
                </div>
                
                <p class="text-sm text-white/70">&copy; 2025 Abdel Azhra. Dirancang dan dibangun sebagai bagian dari Enrichment Program.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Theme changer
        function changeTheme(theme) {
            const body = document.body;
            
            switch(theme) {
                case 'ocean':
                    body.style.background = 'linear-gradient(135deg, #667eea 0%, #764ba2 100%)';
                    break;
                case 'dark':
                    body.style.background = 'linear-gradient(135deg, #1e1b4b 0%, #312e81 50%, #1e3a8a 100%)';
                    break;
                case 'sunset':
                    body.style.background = 'linear-gradient(135deg, #f093fb 0%, #f5576c 100%)';
                    break;
                case 'forest':
                    body.style.background = 'linear-gradient(135deg, #11998e 0%, #38ef7d 100%)';
                    break;
                case 'pink':
                    body.style.background = 'linear-gradient(135deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%)';
                    break;
            }
        }

        // Chart.js SUS Score Chart
        const ctx = document.getElementById('susScoreChart').getContext('2d');
        const susScoreChart = new Chart(ctx, {
            type: 'doughnut',
            data: {
                labels: ['Skor Tercapai', 'Sisa'],
                datasets: [{
                    data: [72.24, 100 - 72.24],
                    backgroundColor: [
                        '#4f46e5', // indigo-600
                        '#e5e7eb'  // gray-200
                    ],
                    borderColor: '#ffffff',
                    borderWidth: 4,
                    hoverOffset: 4
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                cutout: '70%',
                plugins: {
                    legend: {
                        display: false
                    },
                    tooltip: {
                        callbacks: {
                            label: function(context) {
                                return null;
                            }
                        }
                    },
                    title: {
                        display: true,
                        text: '72.24 / 100',
                        position: 'bottom',
                        align: 'center',
                        font: {
                            size: 16,
                            weight: 'bold'
                        },
                        color: '#334155',
                        padding: {
                            top: 10
                        }
                    }
                }
            }
        });
    </script>
</body>
</html>
