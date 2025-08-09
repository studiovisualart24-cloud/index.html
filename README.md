<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Altere o texto abaixo para o título que você preferir -->
    <title>Studio Visual Art</title>
    
    <!-- Inclui o Tailwind CSS via CDN para estilização -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Adiciona a fonte Inter do Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous"/>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;800&display=swap" rel="stylesheet"/>
    <style>
      body {
        font-family: 'Inter', sans-serif;
      }
      /* Custom styles for the testimonial carousel */
      .carousel-dot {
          transition: background-color 0.3s ease;
      }
      .carousel-dot.active {
          background-color: #f97316; /* Cor laranja do Tailwind */
      }
    </style>
</head>
<body class="bg-gray-900 text-white">

    <!-- Topo Fixo (Menu) -->
    <header class="bg-gray-800 shadow-md sticky top-0 z-50">
        <div class="max-w-6xl mx-auto flex items-center justify-between py-4 px-6 md:px-8">
            <a href="#" class="text-2xl font-bold text-orange-500 hover:text-orange-400 transition-colors duration-200">
                MeuNegócio
            </a>
            <nav class="hidden md:block">
                <ul class="flex space-x-6 text-sm md:text-base">
                    <li><a href="#inicio" class="text-white hover:text-orange-500 transition-colors duration-200">Início</a></li>
                    <li><a href="#servicos" class="text-white hover:text-orange-500 transition-colors duration-200">Serviços</a></li>
                    <li><a href="#portfolio" class="text-white hover:text-orange-500 transition-colors duration-200">Portfólio</a></li>
                    <li><a href="#depoimentos" class="text-white hover:text-orange-500 transition-colors duration-200">Depoimentos</a></li>
                </ul>
            </nav>
            <a href="#contato" class="hidden md:inline-block bg-orange-500 text-white font-bold py-2 px-4 rounded-lg hover:bg-orange-600 transition-colors duration-200">
                Contato
            </a>
            <!-- Botão do menu para dispositivos móveis -->
            <button id="mobile-menu-button" class="md:hidden text-white focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
                </svg>
            </button>
        </div>
    </header>

    <!-- Menu Mobile (oculto por padrão) -->
    <nav id="mobile-menu" class="md:hidden bg-gray-800 absolute w-full left-0 transition-transform duration-300 transform -translate-y-full z-40">
        <ul class="flex flex-col items-center py-4 space-y-4">
            <li><a href="#inicio" class="block text-white hover:text-orange-500 transition-colors duration-200">Início</a></li>
            <li><a href="#servicos" class="block text-white hover:text-orange-500 transition-colors duration-200">Serviços</a></li>
            <li><a href="#portfolio" class="block text-white hover:text-orange-500 transition-colors duration-200">Portfólio</a></li>
            <li><a href="#depoimentos" class="block text-white hover:text-orange-500 transition-colors duration-200">Depoimentos</a></li>
            <li><a href="#contato" class="block bg-orange-500 text-white font-bold py-2 px-4 rounded-lg hover:bg-orange-600 transition-colors duration-200">Contato</a></li>
        </ul>
    </nav>

    <!-- Conteúdo Principal -->
    <main>
        <!-- Seção Banner Hero -->
        <section id="inicio" class="relative h-screen flex items-center justify-center text-center bg-gray-900 overflow-hidden">
            <div class="absolute inset-0 bg-cover bg-center opacity-30" style="background-image: url('https://placehold.co/1920x1080/1f2937/d1d5db?text=Background+Hero');"></div>
            <div class="relative z-10 p-6 max-w-2xl mx-auto">
                <h1 class="text-4xl md:text-6xl font-extrabold text-orange-500 tracking-tight leading-tight mb-4">
                    Transforme Sua Marca Digitalmente
                </h1>
                <p class="text-xl md:text-2xl text-gray-300 mb-8">
                    Estratégias de marketing digital inovadoras para o seu negócio crescer e se destacar na web.
                </p>
                <a href="#servicos" class="bg-orange-500 text-white font-bold py-3 px-8 rounded-lg text-lg hover:bg-orange-600 transition-colors duration-200">
                    Descubra Nossos Serviços
                </a>
            </div>
        </section>

        <!-- Seção Serviços -->
        <section id="servicos" class="py-16 md:py-24 bg-gray-900">
            <div class="max-w-6xl mx-auto px-6 md:px-8 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-orange-500 mb-4">Nossos Serviços</h2>
                <p class="text-lg text-gray-400 mb-12 max-w-3xl mx-auto">
                    Oferecemos uma gama completa de soluções para impulsionar a sua presença online e alcançar seus objetivos de negócio.
                </p>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                    <!-- Bloco de Serviço 1: SEO -->
                    <div class="bg-gray-800 rounded-xl shadow-lg p-6 hover:shadow-2xl transition-all duration-300">
                        <svg class="w-12 h-12 mx-auto text-orange-500 mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
                        </svg>
                        <h3 class="text-xl font-bold mb-2">SEO</h3>
                        <p class="text-gray-400">Otimize seu site para os motores de busca e aumente sua visibilidade organicamente.</p>
                    </div>
                    <!-- Bloco de Serviço 2: Redes Sociais -->
                    <div class="bg-gray-800 rounded-xl shadow-lg p-6 hover:shadow-2xl transition-all duration-300">
                        <svg class="w-12 h-12 mx-auto text-orange-500 mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 10h16M4 14h16M4 18h16"></path>
                        </svg>
                        <h3 class="text-xl font-bold mb-2">Redes Sociais</h3>
                        <p class="text-gray-400">Gerencie e crie conteúdo para suas redes, construindo uma comunidade engajada.</p>
                    </div>
                    <!-- Bloco de Serviço 3: Anúncios Pagos -->
                    <div class="bg-gray-800 rounded-xl shadow-lg p-6 hover:shadow-2xl transition-all duration-300">
                        <svg class="w-12 h-12 mx-auto text-orange-500 mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                        </svg>
                        <h3 class="text-xl font-bold mb-2">Anúncios Pagos</h3>
                        <p class="text-gray-400">Crie campanhas de anúncios eficazes no Google e nas redes sociais para resultados rápidos.</p>
                    </div>
                    <!-- Bloco de Serviço 4: Design Gráfico -->
                    <div class="bg-gray-800 rounded-xl shadow-lg p-6 hover:shadow-2xl transition-all duration-300">
                        <svg class="w-12 h-12 mx-auto text-orange-500 mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m-6 4H4m7 4v2m0-2a2 2 0 100-4m0 4a2 2 0 110-4m0-4h2m-6 4h4m4-4V6m0 4h4m-4 4v2m0-2a2 2 0 100-4m0 4a2 2 0 110-4m-4-4V6m0 4h4m4-4V6"></path>
                        </svg>
                        <h3 class="text-xl font-bold mb-2">Design Gráfico</h3>
                        <p class="text-gray-400">Logotipos, posts para redes sociais e outros materiais visuais que fortalecem sua marca.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção Portfólio -->
        <section id="portfolio" class="py-16 md:py-24 bg-gray-900">
            <div class="max-w-6xl mx-auto px-6 md:px-8 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-orange-500 mb-4">Nosso Portfólio</h2>
                <p class="text-lg text-gray-400 mb-12 max-w-3xl mx-auto">
                    Confira alguns dos nossos projetos recentes e o impacto que causamos para nossos clientes.
                </p>
                <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                    <img class="w-full h-auto rounded-lg shadow-lg hover:scale-105 transition-transform duration-300" src="https://placehold.co/600x400/1f2937/d1d5db?text=Projeto+1" alt="Imagem do projeto 1" />
                    <img class="w-full h-auto rounded-lg shadow-lg hover:scale-105 transition-transform duration-300" src="https://placehold.co/600x400/1f2937/d1d5db?text=Projeto+2" alt="Imagem do projeto 2" />
                    <img class="w-full h-auto rounded-lg shadow-lg hover:scale-105 transition-transform duration-300" src="https://placehold.co/600x400/1f2937/d1d5db?text=Projeto+3" alt="Imagem do projeto 3" />
                    <img class="w-full h-auto rounded-lg shadow-lg hover:scale-105 transition-transform duration-300" src="https://placehold.co/600x400/1f2937/d1d5db?text=Projeto+4" alt="Imagem do projeto 4" />
                    <img class="w-full h-auto rounded-lg shadow-lg hover:scale-105 transition-transform duration-300" src="https://placehold.co/600x400/1f2937/d1d5db?text=Projeto+5" alt="Imagem do projeto 5" />
                    <img class="w-full h-auto rounded-lg shadow-lg hover:scale-105 transition-transform duration-300" src="https://placehold.co/600x400/1f2937/d1d5db?text=Projeto+6" alt="Imagem do projeto 6" />
                </div>
            </div>
        </section>

        <!-- Seção Depoimentos -->
        <section id="depoimentos" class="py-16 md:py-24 bg-gray-800">
            <div class="max-w-4xl mx-auto px-6 md:px-8 text-center">
                <h2 class="text-3xl md:text-4xl font-bold text-orange-500 mb-4">O que nossos clientes dizem</h2>
                <div id="testimonial-carousel" class="relative overflow-hidden">
                    <!-- Carousel Wrapper -->
                    <div id="testimonial-wrapper" class="relative h-64 flex transition-transform duration-500 ease-in-out">
                        <!-- Depoimento 1 -->
                        <div class="testimonial w-full flex-shrink-0 flex items-center justify-center p-4">
                            <div class="max-w-2xl">
                                <p class="italic text-gray-300 text-lg mb-4">
                                    "O trabalho deles impulsionou nossas vendas em 50% em apenas três meses. A equipe é super profissional e criativa. Recomendo!"
                                </p>
                                <p class="font-bold text-xl text-orange-500">Maria Silva</p>
                                <p class="text-gray-400 text-sm">CEO, Startup Tech</p>
                            </div>
                        </div>
                        <!-- Depoimento 2 -->
                        <div class="testimonial w-full flex-shrink-0 flex items-center justify-center p-4 hidden">
                            <div class="max-w-2xl">
                                <p class="italic text-gray-300 text-lg mb-4">
                                    "A estratégia de SEO que desenvolveram foi fundamental para o nosso crescimento. Agora somos líderes em nosso nicho. Incrível!"
                                </p>
                                <p class="font-bold text-xl text-orange-500">João Costa</p>
                                <p class="text-gray-400 text-sm">Diretor de Marketing, Loja Online</p>
                            </div>
                        </div>
                        <!-- Depoimento 3 -->
                        <div class="testimonial w-full flex-shrink-0 flex items-center justify-center p-4 hidden">
                            <div class="max-w-2xl">
                                <p class="italic text-gray-300 text-lg mb-4">
                                    "Com o novo design e o conteúdo para redes sociais, nossa marca ganhou uma nova vida. O engajamento aumentou muito. Ótimo trabalho!"
                                </p>
                                <p class="font-bold text-xl text-orange-500">Ana Pereira</p>
                                <p class="text-gray-400 text-sm">Empreendedora, Marca de Moda</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Navegação do Carrossel -->
                    <div id="carousel-dots" class="absolute bottom-4 left-1/2 -translate-x-1/2 flex space-x-2">
                        <span class="carousel-dot w-3 h-3 bg-gray-600 rounded-full cursor-pointer active" data-index="0"></span>
                        <span class="carousel-dot w-3 h-3 bg-gray-600 rounded-full cursor-pointer" data-index="1"></span>
                        <span class="carousel-dot w-3 h-3 bg-gray-600 rounded-full cursor-pointer" data-index="2"></span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Rodapé -->
        <footer id="contato" class="bg-gray-800 text-gray-400 text-center py-8">
            <div class="max-w-6xl mx-auto px-6 md:px-8">
                <div class="flex flex-col md:flex-row justify-between items-center space-y-4 md:space-y-0">
                    <p class="text-sm">&copy; 2025 Meu Negócio. Todos os direitos reservados.</p>
                    <div class="flex justify-center space-x-4">
                        <a href="#" class="hover:text-orange-500 transition-colors duration-200">
                            <!-- Ícone do Instagram -->
                            <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 2.163c3.204 0 3.584.012 4.85.07c3.252.148 4.77 1.688 4.908 4.908.058 1.265.07 1.645.07 4.85s-.012 3.584-.07 4.85c-.148 3.252-1.688 4.77-4.908 4.908-1.265.058-1.645.07-4.85.07s-3.584-.012-4.85-.07c-3.252-.148-4.77-1.688-4.908-4.908-.058-1.265-.07-1.645-.07-4.85s.012-3.584.07-4.85c.148-3.252 1.688-4.77 4.908-4.908 1.265-.058 1.645-.07 4.85-.07zm0-2.163c-3.259 0-3.667.014-4.947.073-4.423.202-6.732 2.511-6.934 6.934-.059 1.28-.073 1.688-.073 4.947s.014 3.667.073 4.947c.202 4.423 2.511 6.732 6.934 6.934 1.28.059 1.688.073 4.947.073s3.667-.014 4.947-.073c4.423-.202 6.732-2.511 6.934-6.934.059-1.28.073-1.688.073-4.947s-.014-3.667-.073-4.947c-.202-4.423-2.511-6.732-6.934-6.934-1.28-.059-1.688-.073-4.947-.073zM12 5.838c-3.411 0-6.162 2.75-6.162 6.162s2.75 6.162 6.162 6.162 6.162-2.75 6.162-6.162-2.751-6.162-6.162-6.162zm0 10.162c-2.21 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm6.406-11.845a1.442 1.442 0 100 2.884 1.442 1.442 0 000-2.884z"></path></svg>
                        </a>
                        <a href="#" class="hover:text-orange-500 transition-colors duration-200">
                            <!-- Ícone do Twitter -->
                            <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 4.557a9.83 9.83 0 01-2.828.775 4.922 4.922 0 002.165-2.724 9.864 9.864 0 01-3.127 1.195 4.916 4.916 0 00-8.384 4.482A13.917 13.917 0 013.88 3.38a4.923 4.923 0 00-.666 2.463c0 1.706.87 3.21 2.185 4.09A4.905 4.905 0 01.996 9.07a4.918 4.918 0 001.988 4.103 4.912 4.912 0 01-2.228.084 4.924 4.924 0 004.568 3.42 9.805 9.805 0 01-6.143 2.122A13.924 13.924 0 002.934 19.78c12.213 0 18.835-10.155 18.835-18.836 0-.287-.008-.57-.019-.854A13.435 13.435 0 0024 4.557z"></path></svg>
                        </a>
                        <a href="#" class="hover:text-orange-500 transition-colors duration-200">
                            <!-- Ícone do LinkedIn -->
                            <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.768s.784-1.768 1.75-1.768 1.75.79 1.75 1.768-.784 1.768-1.75 1.768zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"></path></svg>
                        </a>
                    </div>
                </div>
            </div>
        </footer>
    </main>

    <!-- Script para o menu móvel e carrossel de depoimentos -->
    <script>
        // Lógica do Menu Móvel
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('-translate-y-full');
        });

        // Lógica do Carrossel de Depoimentos
        const testimonials = document.querySelectorAll('.testimonial');
        const dots = document.querySelectorAll('.carousel-dot');
        let currentIndex = 0;

        function updateCarousel() {
            testimonials.forEach((testimonial, index) => {
                testimonial.classList.add('hidden');
                if (index === currentIndex) {
                    testimonial.classList.remove('hidden');
                }
            });

            dots.forEach((dot, index) => {
                dot.classList.remove('active', 'bg-orange-500');
                dot.classList.add('bg-gray-600');
                if (index === currentIndex) {
                    dot.classList.add('active', 'bg-orange-500');
                    dot.classList.remove('bg-gray-600');
                }
            });
        }

        dots.forEach(dot => {
            dot.addEventListener('click', (e) => {
                currentIndex = parseInt(e.target.dataset.index, 10);
                updateCarousel();
            });
        });

        // Autoplay do carrossel
        setInterval(() => {
            currentIndex = (currentIndex + 1) % testimonials.length;
            updateCarousel();
        }, 5000); // Muda a cada 5 segundos
        
    </script>
</body>
</html>
