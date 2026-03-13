<!DOCTYPE html>
<html lang="ar" dir="rtl" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رائد الرفيد | مطور ويب محترف</title>
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com">
    <link href="https://unpkg.com" rel="stylesheet">
    
    <style>
        @import url('https://fonts.googleapis.com');
        
        body {
            font-family: 'Cairo', sans-serif;
            background-color: #020617;
            color: #f8fafc;
            overflow-x: hidden;
        }

        .glass-nav {
            background: rgba(2, 6, 23, 0.7);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(16, 185, 129, 0.1);
        }

        .hero-glow {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 600px;
            height: 600px;
            background: radial-gradient(circle, rgba(16, 185, 129, 0.15) 0%, transparent 70%);
            z-index: -1;
            filter: blur(80px);
        }

        .profile-frame {
            position: relative;
            width: 160px;
            height: 160px;
            border-radius: 50%;
            border: 3px solid rgba(16, 185, 129, 0.5);
            padding: 5px;
            transition: all 0.5s ease;
        }

        .profile-frame:hover {
            transform: rotate(5deg) scale(1.05);
            border-color: #10b981;
            box-shadow: 0 0 30px rgba(16, 185, 129, 0.4);
        }

        .profile-img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover; /* تم التصحيح */
        }

        .project-card {
            background: rgba(15, 23, 42, 0.6);
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .project-card:hover {
            border-color: #10b981;
            transform: translateY(-10px);
            background: rgba(16, 185, 129, 0.05);
        }

        .custom-gradient-text {
            background: linear-gradient(to right, #10b981, #34d399, #6ee7b7);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* تحسين السكرول بار */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #020617; }
        ::-webkit-scrollbar-thumb { background: #10b981; border-radius: 10px; }
    </style>
</head>
<body>

    <!-- Navbar -->
    <nav class="fixed w-full z-50 glass-nav py-4 transition-all duration-500" id="navbar">
        <div class="container mx-auto px-6 flex justify-between items-center">
            <div class="text-2xl font-black text-emerald-500 tracking-tighter">RAED.<span class="text-white">DEV</span></div>
            <div class="hidden md:flex space-x-reverse space-x-8 font-medium">
                <a href="#home" class="hover:text-emerald-400 transition">الرئيسية</a>
                <a href="#services" class="hover:text-emerald-400 transition">الخدمات</a>
                <a href="#portfolio" class="hover:text-emerald-400 transition">أعمالي</a>
            </div>
            <a href="https://wa.me" target="_blank" class="bg-emerald-600 px-6 py-2 rounded-full hover:bg-emerald-500 transition shadow-lg shadow-emerald-900/20 font-bold">تواصل معي</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="relative min-h-screen flex items-center justify-center pt-20 overflow-hidden">
        <div class="hero-glow"></div>
        <div class="container mx-auto px-6 text-center z-10" data-aos="fade-up">
            <div class="profile-frame mb-8 mx-auto">
                <img src="https://raw.githubusercontent.com" alt="Raed's Photo" class="profile-img">
            </div>
            
            <div class="inline-flex items-center gap-2 px-4 py-1 border border-emerald-500/30 rounded-full text-emerald-400 text-sm mb-6 bg-emerald-500/10">
                <span class="relative flex h-2 w-2">
                    <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
                    <span class="relative inline-flex rounded-full h-2 w-2 bg-emerald-500"></span>
                </span>
                متاح حالياً للمشاريع الجديدة
            </div>

            <h1 class="text-5xl md:text-7xl font-black mb-6 leading-tight">
                أنا رائد الرفيد <br>
                <span class="custom-gradient-text" id="typed-text"></span>
            </h1>
            
            <p class="text-gray-400 text-lg md:text-xl max-w-2xl mx-auto mb-10">
                أقوم بتحويل الأفكار المعقدة إلى واجهات مستخدم بسيطة وجذابة. متخصص في تطوير المواقع المتكاملة (Full-Stack).
            </p>

            <div class="flex flex-wrap justify-center gap-4">
                <a href="#portfolio" class="px-8 py-4 bg-emerald-600 rounded-xl font-bold hover:scale-105 transition-all shadow-xl shadow-emerald-900/40">استعرض أعمالي</a>
                <a href="https://wa.me" target="_blank" class="px-8 py-4 border border-emerald-500/30 rounded-xl font-bold hover:bg-white/5 transition-all flex items-center gap-2">
                    <i class="fab fa-whatsapp text-emerald-500"></i> واتساب
                </a>
            </div>
        </div>
    </section>

    <!-- Services -->
    <section id="services" class="py-24 relative">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold mb-4">خدماتي <span class="text-emerald-500">الاحترافية</span></h2>
                <div class="h-1 w-20 bg-emerald-500 mx-auto rounded-full"></div>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="p-8 rounded-3xl project-card group" data-aos="fade-up">
                    <div class="w-14 h-14 bg-emerald-500/10 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-layer-group text-2xl text-emerald-500"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">تطوير المواقع</h3>
                    <p class="text-gray-400 leading-relaxed">بناء مواقع سريعة، متجاوبة، ومتوافقة مع جميع الشاشات باستخدام أحدث التقنيات.</p>
                </div>

                <div class="p-8 rounded-3xl project-card bg-emerald-600/5 border-emerald-500/20" data-aos="fade-up" data-aos-delay="100">
                    <div class="w-14 h-14 bg-emerald-500 rounded-lg flex items-center justify-center mb-6 shadow-lg shadow-emerald-500/20">
                        <i class="fas fa-rocket text-2xl text-white"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">تحسين الأداء</h3>
                    <p class="text-gray-400 leading-relaxed">تسريع سرعة تحميل الصفحات وضمان أفضل تجربة للمستخدم النهائي.</p>
                </div>

                <div class="p-8 rounded-3xl project-card group" data-aos="fade-up" data-aos-delay="200">
                    <div class="w-14 h-14 bg-emerald-500/10 rounded-lg flex items-center justify-center mb-6">
                        <i class="fas fa-search-dollar text-2xl text-emerald-500"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">تهيئة الـ SEO</h3>
                    <p class="text-gray-400 leading-relaxed">جعل موقعك يظهر في النتائج الأولى لمحركات البحث لزيادة عدد الزيارات.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio -->
    <section id="portfolio" class="py-24 bg-slate-900/30">
        <div class="container mx-auto px-6">
            <div class="flex justify-between items-end mb-16">
                <div>
                    <h2 class="text-4xl font-bold mb-2">معرض <span class="text-emerald-500">الأعمال</span></h2>
                    <p class="text-gray-400">بعض المشاريع التي قمت بتنفيذها مؤخراً</p>
                </div>
            </div>

            <div class="grid md:grid-cols-2 gap-10">
                <div class="project-card rounded-2xl overflow-hidden shadow-2xl group" data-aos="zoom-in-right">
                    <div class="relative overflow-hidden">
                        <img src="https://images.unsplash.com" class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110">
                        <div class="absolute inset-0 bg-emerald-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="bg-white text-black px-6 py-2 rounded-full font-bold">مشاهدة التفاصيل</span>
                        </div>
                    </div>
                    <div class="p-8">
                        <div class="flex gap-2 mb-4">
                            <span class="text-[10px] bg-emerald-500/20 text-emerald-400 px-2 py-1 rounded">React</span>
                            <span class="text-[10px] bg-blue-500/20 text-blue-400 px-2 py-1 rounded">Firebase</span>
                        </div>
                        <h3 class="text-2xl font-bold text-white mb-2">منصة إحصائيات متطورة</h3>
                        <p class="text-gray-400 mb-6">لوحة تحكم ذكية لعرض البيانات بشكل تفاعلي ولحظي.</p>
                        <a href="#" class="text-emerald-400 font-bold flex items-center gap-2 group-hover:gap-4 transition-all">
                            زيارة المشروع <i class="fas fa-arrow-left"></i>
                        </a>
                    </div>
                </div>

                <div class="project-card rounded-2xl overflow-hidden shadow-2xl group" data-aos="zoom-in-left">
                    <div class="relative overflow-hidden">
                        <img src="https://images.unsplash.com" class="w-full h-64 object-cover transition-transform duration-500 group-hover:scale-110">
                        <div class="absolute inset-0 bg-emerald-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center">
                            <span class="bg-white text-black px-6 py-2 rounded-full font-bold">مشاهدة التفاصيل</span>
                        </div>
                    </div>
                    <div class="p-8">
                        <div class="flex gap-2 mb-4">
                            <span class="text-[10px] bg-emerald-500/20 text-emerald-400 px-2 py-1 rounded">Next.js</span>
                            <span class="text-[10px] bg-purple-500/20 text-purple-400 px-2 py-1 rounded">Stripe</span>
                        </div>
                        <h3 class="text-2xl font-bold text-white mb-2">متجر إلكتروني حديث</h3>
                        <p class="text-gray-400 mb-6">تصميم متجر متكامل مع نظام دفع ذكي وتجربة شراء سلسة.</p>
                        <a href="#" class="text-emerald-400 font-bold flex items-center gap-2 group-hover:gap-4 transition-all">
                            زيارة المشروع <i class="fas fa-arrow-left"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 border-t border-white/5 text-center text-gray-500">
        <p>© 2024 رائد الرفيد. جميع الحقوق محفوظة.</p>
    </footer>

    <!-- Scripts -->
    <script src="https://unpkg.com"></script>
    <script src="https://cdn.jsdelivr.net"></script>
    
    <script>
        // تهيئة الأنيميشن
        AOS.init({ duration: 1000, once: true });

        // تشغيل تأثير الكتابة
        new Typed('#typed-text', {
            strings: ['مطور مواقع Full-Stack', 'مصمم واجهات UI/UX', 'مبرمج تطبيقات ذكية'],
            typeSpeed: 60,
            backSpeed: 40,
            loop: true
        });

        // تغيير مظهر الـ Navbar عند السكرول
        window.onscroll = function() {
            const nav = document.getElementById('navbar');
            if (window.scrollY > 50) {
                nav.classList.add('py-2', 'bg-slate-950/90');
                nav.classList.remove('py-4', 'bg-transparent');
            } else {
                nav.classList.add('py-4', 'bg-transparent');
                nav.classList.remove('py-2', 'bg-slate-950/90');
            }
        };
    </script>
</body>
</html>
