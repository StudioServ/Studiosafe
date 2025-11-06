<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <base target="_self">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StudioSERV - Edição Profissional de Vídeos e Transformação de Marcas</title>
    <meta name="description" content="Transforme seu conteúdo amador em presença profissional. Edição de vídeos que fazem sua marca ser levada a sério. Entre em contato via Instagram.">
    <meta name="keywords" content="edição de vídeos, branding, conteúdo profissional, transformação digital, autoridade online">
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: "#000000",
                        secondary: "#1a1a1a",
                        accent: "#ff0000",
                        "accent-blue": "#00ffff",
                        "dark-gray": "#2d2d2d",
                        "light-gray": "#4a4a4a"
                    },
                    fontFamily: {
                        'sans': ['Inter', 'system-ui', 'sans-serif'],
                    },
                    animation: {
                        'fade-in': 'fadeIn 0.8s ease-in-out',
                        'slide-up': 'slideUp 0.6s ease-out',
                        'pulse-glow': 'pulseGlow 2s infinite'
                    }
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { 
                opacity: 0;
                transform: translateY(30px);
            }
            to { 
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes pulseGlow {
            0%, 100% { box-shadow: 0 0 5px rgba(255, 0, 0, 0.3); }
            50% { box-shadow: 0 0 20px rgba(255, 0, 0, 0.6); }
        }
        
        body {
            font-family: 'Inter', sans-serif;
        }
        
        .gradient-text {
            background: linear-gradient(45deg, #ff0000, #00ffff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .instagram-gradient {
            background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="min-h-screen bg-primary text-white">
    <!-- Header -->
    <header class="bg-primary border-b border-light-gray sticky top-0 z-50">
        <nav class="container mx-auto px-4 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center space-x-2">
                    <div class="w-8 h-8 bg-accent rounded-full"></div>
                    <span class="text-xl font-bold">Studio<span class="text-accent">SERV</span></span>
                </div>
                
                <div class="hidden md:flex space-x-8">
                    <a href="#sobre" class="hover:text-accent transition-colors duration-300">Sobre</a>
                    <a href="#beneficios" class="hover:text-accent transition-colors duration-300">Benefícios</a>
                    <a href="#portfolio" class="hover:text-accent transition-colors duration-300">Portfólio</a>
                    <a href="#contato" class="hover:text-accent transition-colors duration-300">Contato</a>
                </div>
                
                <button onclick="openInstagram()" class="bg-accent hover:bg-red-600 text-white px-6 py-2 rounded-lg font-medium transition-all duration-300 transform hover:scale-105">
                    Orçamento
                </button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="min-h-screen flex items-center justify-center bg-gradient-to-br from-primary to-secondary relative overflow-hidden">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-4xl md:text-6xl lg:text-7xl font-bold mb-6 animate-fade-in">
                Quer que te levem a sério?
                <br>
                <span class="gradient-text">Começa pela sua edição.</span>
            </h1>
            <p class="text-xl md:text-2xl text-light-gray mb-12 max-w-3xl mx-auto animate-slide-up">
                Transformamos conteúdo amador em presença profissional com edições que geram autoridade e respeito.
            </p>
            <button onclick="openInstagram()" class="bg-accent hover:bg-red-600 text-white px-8 py-4 rounded-lg font-bold text-lg md:text-xl transition-all duration-300 transform hover:scale-110 animate-pulse-glow">
                Solicitar Orçamento
            </button>
            <p class="text-light-gray mt-4 text-sm">
                Entre em contato via Instagram: <span class="instagram-gradient font-semibold">@studioserv</span>
            </p>
        </div>
        
        <!-- Background Elements -->
        <div class="absolute top-1/4 left-1/4 w-2 h-2 bg-accent-blue rounded-full opacity-70 animate-pulse"></div>
        <div class="absolute bottom-1/3 right-1/4 w-1 h-1 bg-accent rounded-full opacity-50 animate-pulse" style="animation-delay: 0.5s;"></div>
    </section>

    <!-- Sobre Section -->
    <section id="sobre" class="py-20 bg-secondary">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Sobre a <span class="text-accent">StudioSERV</span></h2>
                <p class="text-xl text-light-gray max-w-3xl mx-auto">
                    Somos especialistas em transformar conteúdo amador em presença profissional, 
                    focando em impacto, respeito e resultados reais para sua marca.
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Velocidade -->
                <div class="text-center p-8 bg-dark-gray rounded-xl hover:transform hover:scale-105 transition-all duration-300">
                    <div class="w-16 h-16 bg-accent rounded-full flex items-center justify-center mx-auto mb-6">
                        <i class="fas fa-bolt text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Velocidade</h3>
                    <p class="text-light-gray">
                        Entregas rápidas sem comprometer a qualidade. Seu conteúdo no ar quando você precisa.
                    </p>
                </div>
                
                <!-- Qualidade -->
                <div class="text-center p-8 bg-dark-gray rounded-xl hover:transform hover:scale-105 transition-all duration-300">
                    <div class="w-16 h-16 bg-accent-blue rounded-full flex items-center justify-center mx-auto mb-6">
                        <i class="fas fa-gem text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Qualidade</h3>
                    <p class="text-light-gray">
                        Padrão profissional em cada frame. Edições que impressionam e geram credibilidade.
                    </p>
                </div>
                
                <!-- Autoridade Digital -->
                <div class="text-center p-8 bg-dark-gray rounded-xl hover:transform hover:scale-105 transition-all duration-300">
                    <div class="w-16 h-16 bg-accent rounded-full flex items-center justify-center mx-auto mb-6">
                        <i class="fas fa-crown text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-4">Autoridade Digital</h3>
                    <p class="text-light-gray">
                        Conteúdo que posiciona você como referência no seu nicho e constrói confiança.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Benefícios Section -->
    <section id="beneficios" class="py-20 bg-primary">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Por que Escolher a <span class="text-accent">StudioSERV</span>?</h2>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
                <div class="flex items-start space-x-4 p-6 bg-dark-gray rounded-lg hover:bg-light-gray transition-colors duration-300">
                    <div class="w-8 h-8 bg-accent rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                        <i class="fas fa-check text-sm"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-semibold mb-2">Edições que fazem sua marca ser levada a sério</h3>
                        <p class="text-light-gray">Conteúdo profissional que transmite credibilidade e autoridade.</p>
                    </div>
                </div>
                
                <div class="flex items-start space-x-4 p-6 bg-dark-gray rounded-lg hover:bg-light-gray transition-colors duration-300">
                    <div class="w-8 h-8 bg-accent rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                        <i class="fas fa-check text-sm"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-semibold mb-2">Profissionalize seu conteúdo</h3>
                        <p class="text-light-gray">Transforme gravações caseiras em produções de alto nível.</p>
                    </div>
                </div>
                
                <div class="flex items-start space-x-4 p-6 bg-dark-gray rounded-lg hover:bg-light-gray transition-colors duration-300">
                    <div class="w-8 h-8 bg-accent rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                        <i class="fas fa-check text-sm"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-semibold mb-2">Impressione quem te assiste</h3>
                        <p class="text-light-gray">Conteúdo visualmente impactante que cativa e converte.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-secondary">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Nosso <span class="text-accent">Portfólio</span></h2>
                <p class="text-xl text-light-gray max-w-3xl mx-auto">
                    Veja exemplos de transformações que elevam a percepção de valor das marcas.
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="group relative overflow-hidden rounded-xl bg-dark-gray hover:transform hover:scale-105 transition-all duration-500">
                    <img 
                        src="https://picsum.photos/400/300?random=1" 
                        alt="Transformação de conteúdo corporativo - antes e depois" 
                        class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500"
                        loading="lazy"
                    />
                    <div class="absolute inset-0 bg-black bg-opacity-70 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                        <div class="text-center p-4">
                            <h3 class="text-xl font-bold mb-2">Conteúdo Corporativo</h3>
                            <p class="text-light-gray">Transformação completa de apresentações empresariais</p>
                        </div>
                    </div>
                </div>
                
                <div class="group relative overflow-hidden rounded-xl bg-dark-gray hover:transform hover:scale-105 transition-all duration-500">
                    <img 
                        src="https://picsum.photos/400/300?random=2" 
                        alt="Edição para criadores de conteúdo digital" 
                        class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500"
                        loading="lazy"
                    />
                    <div class="absolute inset-0 bg-black bg-opacity-70 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                        <div class="text-center p-4">
                            <h3 class="text-xl font-bold mb-2">Criadores Digitais</h3>
                            <p class="text-light-gray">Edição profissional para YouTube e redes sociais</p>
                        </div>
                    </div>
                </div>
                
                <div class="group relative overflow-hidden rounded-xl bg-dark-gray hover:transform hover:scale-105 transition-all duration-500">
                    <img 
                        src="https://picsum.photos/400/300?random=3" 
                        alt="Branding visual para marcas pessoais" 
                        class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500"
                        loading="lazy"
                    />
                    <div class="absolute inset-0 bg-black bg-opacity-70 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
                        <div class="text-center p-4">
                            <h3 class="text-xl font-bold mb-2">Branding Pessoal</h3>
                            <p class="text-light-gray">Identidade visual consistente para marcas pessoais</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Final Section -->
    <section id="contato" class="py-20 bg-gradient-to-br from-primary to-dark-gray">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-5xl font-bold mb-6">
                Agora é com <span class="text-accent">você</span>.
            </h2>
            <p class="text-xl md:text-2xl text-light-gray mb-8 max-w-2xl mx-auto">
                Solicite seu orçamento e transforme seu conteúdo hoje mesmo.
            </p>
            <p class="text-lg text-light-gray mb-12 max-w-3xl mx-auto">
                Não deixe que edições amadoras comprometam sua autoridade. 
                Conte com profissionais que entendem o poder do conteúdo bem produzido.
            </p>
            <button onclick="openInstagram()" class="bg-accent hover:bg-red-600 text-white px-12 py-6 rounded-lg font-bold text-xl md:text-2xl transition-all duration-300 transform hover:scale-110 shadow-2xl">
                Falar com a StudioSERV
            </button>
            <div class="mt-6">
                <p class="text-light-gray text-lg">
                    Entre em contato via Instagram: 
                    <span class="instagram-gradient font-bold text-xl">@studioserv</span>
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black py-12 border-t border-light-gray">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <div class="flex items-center space-x-2 mb-4">
                        <div class="w-6 h-6 bg-accent rounded-full"></div>
                        <span class="text-xl font-bold">Studio<span class="text-accent">SERV</span></span>
                    </div>
                    <p class="text-light-gray text-sm">
                        Transformando conteúdo em autoridade digital
                    </p>
                </div>
                
                <div class="flex space-x-6">
                    <a href="https://instagram.com/studioserv" target="_blank" class="text-light-gray hover:text-accent transition-colors duration-300">
                        <i class="fab fa-instagram text-xl"></i>
                    </a>
                    <a href="#" class="text-light-gray hover:text-accent transition-colors duration-300">
                        <i class="fab fa-youtube text-xl"></i>
                    </a>
                    <a href="#" class="text-light-gray hover:text-accent transition-colors duration-300">
                        <i class="fab fa-linkedin text-xl"></i>
                    </a>
                </div>
            </div>
            
            <div class="border-t border-light-gray mt-8 pt-8 text-center">
                <p class="text-light-gray text-sm">
                    &copy; 2024 StudioSERV. Todos os direitos reservados.
                </p>
                <p class="text-light-gray text-xs mt-2">
                    Entre em contato: <span class="instagram-gradient">@studioserv</span>
                </p>
            </div>
        </div>
    </footer>

    <script>
        // Instagram integration
        function openInstagram() {
            const instagramUrl = "https://instagram.com/studioserv";
            window.open(instagramUrl, '_blank');
        }
        
        // Smooth scrolling
        function scrollToContact() {
            document.getElementById('contato').scrollIntoView({ 
                behavior: 'smooth' 
            });
        }
        
        // Navigation smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
        
        // Add scroll animation
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'slideUp 0.6s ease-out forwards';
                }
            });
        }, observerOptions);
        
        // Observe elements for animation
        document.addEventListener('DOMContentLoaded', () => {
            const animatedElements = document.querySelectorAll('.grid > div');
            animatedElements.forEach(el => {
                el.style.opacity = '0';
                observer.observe(el);
            });
        });
    </script>
</body>
</html>
