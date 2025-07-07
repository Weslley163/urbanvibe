<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Urban Vibe - Estilo Urbano e Performance</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #3a0ca3;
            --secondary: #f72585;
            --accent: #4cc9f0;
            --dark: #1a1a1a;
            --light: #f8f9fa;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
        }
        
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0,0,0,0.2);
        }
        
        .category-badge {
            transition: all 0.3s ease;
        }
        
        .category-badge.active {
            background-color: var(--primary);
            color: white;
            transform: scale(1.05);
        }
        
        .nav-link::after {
            content: '';
            display: block;
            width: 0;
            height: 2px;
            background: var(--secondary);
            transition: width 0.3s;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
    </style>
</head>
<body class="bg-gray-50 font-sans">
    <!-- Header/Navbar -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20 items-center">
                <div class="flex items-center">
                    <img src="https://placehold.co/40x40" alt="Logo Urban Vibe - Letra U e V entrelaçadas com design urbano moderno" class="h-10 w-10">
                    <span class="ml-3 text-2xl font-bold bg-gradient-to-r from-primary to-secondary bg-clip-text text-transparent">URBAN VIBE</span>
                </div>
                
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="nav-link text-gray-800 font-medium">Início</a>
                    <a href="#products" class="nav-link text-gray-800 font-medium">Produtos</a>
                    <a href="#categories" class="nav-link text-gray-800 font-medium">Categorias</a>
                    <a href="#about" class="nav-link text-gray-800 font-medium">Sobre</a>
                    <a href="#contact" class="nav-link text-gray-800 font-medium">Contato</a>
                </div>
                
                <div class="flex items-center space-x-4">
                    <button class="p-2 rounded-full hover:bg-gray-100">
                        <i class="fas fa-search text-gray-600"></i>
                    </button>
                    <button class="p-2 rounded-full hover:bg-gray-100 relative">
                        <i class="fas fa-shopping-cart text-gray-600"></i>
                        <span class="absolute -top-1 -right-1 bg-secondary text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">3</span>
                    </button>
                    <button class="md:hidden p-2 rounded-full hover:bg-gray-100">
                        <i class="fas fa-bars text-gray-600"></i>
                    </button>
                </div>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient text-white py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-8 items-center">
                <div>
                    <h1 class="text-4xl md:text-5xl font-bold mb-4">ESTILO URBANO. PERFORMANCE. ATITUDE.</h1>
                    <p class="text-xl mb-8">Descubra os melhores produtos para complementar seu lifestyle urbano e ativo.</p>
                    <div class="flex space-x-4">
                        <button class="bg-white text-primary px-6 py-3 rounded-lg font-bold hover:bg-opacity-90 transition">COMPRE AGORA</button>
                        <button class="border-2 border-white text-white px-6 py-3 rounded-lg font-bold hover:bg-white hover:bg-opacity-10 transition">EXPLORAR</button>
                    </div>
                </div>
                <div class="relative">
                    <img src="https://placehold.co/800x600" alt="Modelo urbano usando produtos Urban Vibe em ambiente de cidade moderna" class="rounded-xl shadow-2xl border-4 border-white">
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Categories -->
    <section id="categories" class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-12">NOSSAS CATEGORIAS</h2>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                <div class="category-card bg-gray-50 rounded-xl p-6 text-center hover:shadow-lg transition cursor-pointer">
                    <div class="bg-primary bg-opacity-10 p-4 rounded-full w-20 h-20 mx-auto flex items-center justify-center mb-4">
                        <i class="fas fa-spa text-3xl text-primary"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Cosméticos</h3>
                    <p class="text-gray-600 text-sm">Cuidados que realçam sua beleza urbana</p>
                </div>
                
                <div class="category-card bg-gray-50 rounded-xl p-6 text-center hover:shadow-lg transition cursor-pointer">
                    <div class="bg-secondary bg-opacity-10 p-4 rounded-full w-20 h-20 mx-auto flex items-center justify-center mb-4">
                        <i class="fas fa-dumbbell text-3xl text-secondary"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Academia</h3>
                    <p class="text-gray-600 text-sm">Performance máxima para seus treinos</p>
                </div>
                
                <div class="category-card bg-gray-50 rounded-xl p-6 text-center hover:shadow-lg transition cursor-pointer">
                    <div class="bg-accent bg-opacity-10 p-4 rounded-full w-20 h-20 mx-auto flex items-center justify-center mb-4">
                        <i class="fas fa-tshirt text-3xl text-accent"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Roupas</h3>
                    <p class="text-gray-600 text-sm">Estilo que combina com sua atitude</p>
                </div>
                
                <div class="category-card bg-gray-50 rounded-xl p-6 text-center hover:shadow-lg transition cursor-pointer">
                    <div class="bg-purple-500 bg-opacity-10 p-4 rounded-full w-20 h-20 mx-auto flex items-center justify-center mb-4">
                        <i class="fas fa-glasses text-3xl text-purple-500"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Acessórios</h3>
                    <p class="text-gray-600 text-sm">Detalhes que completam seu visual</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Products -->
    <section id="products" class="py-16 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center mb-12">
                <h2 class="text-3xl font-bold">PRODUTOS EM DESTAQUE</h2>
                <div class="flex space-x-2">
                    <button class="category-badge px-4 py-2 rounded-full border border-gray-300 text-sm font-medium">TODOS</button>
                    <button class="category-badge px-4 py-2 rounded-full border border-gray-300 text-sm font-medium">COSMÉTICOS</button>
                    <button class="category-badge px-4 py-2 rounded-full border border-gray-300 text-sm font-medium">ACADEMIA</button>
                </div>
            </div>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Product 1 -->
                <div class="product-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <div class="relative">
                        <img src="https://placehold.co/600x600" alt="Kit de maquiagem profissional Urban Vibe com diversas cores vibrantes" class="w-full h-64 object-cover">
                        <span class="absolute top-2 right-2 bg-secondary text-white text-xs px-2 py-1 rounded-full">NOVO</span>
                    </div>
                    <div class="p-4">
                        <div class="flex justify-between items-start mb-2">
                            <h3 class="font-bold text-lg">Kit Maquiagem Pro</h3>
                            <span class="text-primary font-bold">R$ 149,90</span>
                        </div>
                        <p class="text-gray-600 text-sm mb-4">Paleta completa com 18 cores profissionais</p>
                        <button class="w-full bg-primary text-white py-2 rounded-lg hover:bg-opacity-90 transition">ADICIONAR AO CARRINHO</button>
                    </div>
                </div>
                
                <!-- Product 2 -->
                <div class="product-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <div class="relative">
                        <img src="https://placehold.co/600x600" alt="Halteres ajustáveis para musculação em preto e roxo" class="w-full h-64 object-cover">
                        <span class="absolute top-2 right-2 bg-secondary text-white text-xs px-2 py-1 rounded-full">-20%</span>
                    </div>
                    <div class="p-4">
                        <div class="flex justify-between items-start mb-2">
                            <h3 class="font-bold text-lg">Halteres Ajustáveis</h3>
                            <div>
                                <span class="text-gray-400 text-sm line-through mr-2">R$ 299,90</span>
                                <span class="text-primary font-bold">R$ 239,90</span>
                            </div>
                        </div>
                        <p class="text-gray-600 text-sm mb-4">De 5kg a 20kg em um único equipamento</p>
                        <button class="w-full bg-primary text-white py-2 rounded-lg hover:bg-opacity-90 transition">ADICIONAR AO CARRINHO</button>
                    </div>
                </div>
                
                <!-- Product 3 -->
                <div class="product-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <img src="https://placehold.co/600x600" alt="Jaqueta urbana corta-vento preta com detalhes em neon" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <div class="flex justify-between items-start mb-2">
                            <h3 class="font-bold text-lg">Jaqueta Corta-Vento</h3>
                            <span class="text-primary font-bold">R$ 189,90</span>
                        </div>
                        <p class="text-gray-600 text-sm mb-4">Proteção e estilo para o clima urbano</p>
                        <button class="w-full bg-primary text-white py-2 rounded-lg hover:bg-opacity-90 transition">ADICIONAR AO CARRINHO</button>
                    </div>
                </div>
                
                <!-- Product 4 -->
                <div class="product-card bg-white rounded-xl overflow-hidden shadow-md transition duration-300">
                    <img src="https://placehold.co/600x600" alt="Relógio esportivo inteligente com pulseira preta e tela digital" class="w-full h-64 object-cover">
                    <div class="p-4">
                        <div class="flex justify-between items-start mb-2">
                            <h3 class="font-bold text-lg">Smartwatch Esportivo</h3>
                            <span class="text-primary font-bold">R$ 329,90</span>
                        </div>
                        <p class="text-gray-600 text-sm mb-4">Monitoramento completo de atividades</p>
                        <button class="w-full bg-primary text-white py-2 rounded-lg hover:bg-opacity-90 transition">ADICIONAR AO CARRINHO</button>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="border-2 border-primary text-primary px-6 py-3 rounded-lg font-bold hover:bg-primary hover:text-white transition">VER TODOS OS PRODUTOS</button>
            </div>
        </div>
    </section>

    <!-- Features/Benefits -->
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-3 gap-8">
                <div class="text-center p-6">
                    <div class="bg-gradient-to-r from-primary to-secondary p-3 rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <i class="fas fa-truck text-white text-2xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Entrega Rápida</h3>
                    <p class="text-gray-600">Receba seus produtos em até 48h nas principais cidades</p>
                </div>
                
                <div class="text-center p-6">
                    <div class="bg-gradient-to-r from-primary to-secondary p-3 rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <i class="fas fa-shield-alt text-white text-2xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Garantia Urban</h3>
                    <p class="text-gray-600">Trocas e devoluções sem complicação em até 30 dias</p>
                </div>
                
                <div class="text-center p-6">
                    <div class="bg-gradient-to-r from-primary to-secondary p-3 rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <i class="fas fa-headset text-white text-2xl"></i>
                    </div>
                    <h3 class="font-bold text-lg mb-2">Suporte Premium</h3>
                    <p class="text-gray-600">Atendimento especializado quando você precisar</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h2 class="text-3xl font-bold mb-6">SOBRE A URBAN VIBE</h2>
                    <p class="text-gray-700 mb-4">Na Urban Vibe, acreditamos que estilo e performance andam juntos. Nascemos para oferecer produtos que complementem o lifestyle urbano moderno, unindo design, funcionalidade e qualidade.</p>
                    <p class="text-gray-700 mb-6">Nossa curadoria reúne apenas os melhores itens para quem busca expressar sua personalidade sem abrir mão do conforto e desempenho no dia a dia.</p>
                    <div class="flex space-x-4">
                        <button class="bg-primary text-white px-6 py-3 rounded-lg font-bold hover:bg-opacity-90 transition">NOSSA HISTÓRIA</button>
                        <button class="border-2 border-primary text-primary px-6 py-3 rounded-lg font-bold hover:bg-primary hover:text-white transition">EQUIPE</button>
                    </div>
                </div>
                <div>
                    <img src="https://placehold.co/800x600" alt="Equipe da Urban Vibe em ambiente de trabalho moderno e descontraído" class="rounded-xl shadow-lg">
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section class="py-16 bg-gradient-to-r from-primary to-secondary text-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl font-bold mb-4">JUNTE-SE AO NOSSO CLUBE</h2>
            <p class="text-xl mb-8">Receba ofertas exclusivas e novidades antes de todo mundo</p>
            <div class="flex flex-col sm:flex-row gap-4 max-w-md mx-auto">
                <input type="email" placeholder="Seu melhor e-mail" class="flex-grow px-4 py-3 rounded-lg text-gray-900 focus:outline-none">
                <button class="bg-white text-primary px-6 py-3 rounded-lg font-bold hover:bg-opacity-90 transition whitespace-nowrap">ASSINAR</button>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 flex items-center">
                        <img src="https://placehold.co/30x30" alt="Logo reduzido Urban Vibe" class="mr-2">
                        URBAN VIBE
                    </h3>
                    <p class="text-gray-400">Estilo. Performance. Atitude. Tudo em um só lugar.</p>
                    <div class="flex space-x-4 mt-4">
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-tiktok"></i></a>
                    </div>
                </div>
                
                <div>
                    <h4 class="font-bold text-lg mb-4">LINKS ÚTEIS</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Minha Conta</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Meus Pedidos</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Rastreamento</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Trocas e Devoluções</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold text-lg mb-4">INFORMAÇÕES</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white">Sobre Nós</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Blog</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Trabalhe Conosco</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Termos e Condições</a></li>
                    </ul>
                </div>
                
                <div id="contact">
                    <h4 class="font-bold text-lg mb-4">CONTATO</h4>
                    <ul class="space-y-2">
                        <li class="flex items-center"><i class="fas fa-map-marker-alt mr-2 text-gray-400"></i> <span class="text-gray-400">Av. Paulista, 1000 - São Paulo/SP</span></li>
                        <li class="flex items-center"><i class="fas fa-phone-alt mr-2 text-gray-400"></i> <span class="text-gray-400">(11) 4002-8922</span></li>
                        <li class="flex items-center"><i class="fas fa-envelope mr-2 text-gray-400"></i> <span class="text-gray-400">contato@urbanvibe.com.br</span></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
                <p>&copy; 2023 Urban Vibe. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple filter functionality
        document.addEventListener('DOMContentLoaded', function() {
            const categoryButtons = document.querySelectorAll('.category-badge');
            
            categoryButtons.forEach(button => {
                button.addEventListener('click', function() {
                    categoryButtons.forEach(btn => btn.classList.remove('active'));
                    this.classList.add('active');
                    
                    // Here you would filter products by category in a real implementation
                    // This is just a UI demo
                });
            });
        });
    </script>
</body>
</html>
