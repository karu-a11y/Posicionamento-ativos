<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Análise Estratégica — Posicionamento de Mercado</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* cool-gray-50 */
            scroll-behavior: smooth;
        }
        .section-title {
            @apply text-3xl font-bold text-slate-800 mb-10 text-center;
        }
        .card {
            @apply bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-1;
        }
        
        /* Animation on Scroll */
        .fade-in-section {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .fade-in-section.is-visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Timeline styles */
        .timeline-container {
            position: relative;
            padding: 2rem 0;
        }
        .timeline-container::before {
            content: '';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 3px;
            height: 100%;
            background-color: #cbd5e1; /* slate-300 */
        }
        .timeline-item {
            position: relative;
            width: 50%;
            margin-bottom: 50px;
        }
        .timeline-item:nth-child(odd) {
            padding-right: 50px;
            left: 0;
            text-align: right;
        }
        .timeline-item:nth-child(even) {
            padding-left: 50px;
            left: 50%;
            text-align: left;
        }
        .timeline-dot {
            content: '';
            position: absolute;
            top: 0;
            right: -10px;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background-color: white;
            border: 4px solid;
            z-index: 10;
        }
        .timeline-item:nth-child(even) .timeline-dot {
            left: -10px;
        }
        .timeline-content {
            @apply bg-white p-6 rounded-xl shadow-lg;
        }
        
        /* Responsive timeline for mobile */
        @media screen and (max-width: 768px) {
            .timeline-container::before {
                left: 10px;
            }
            .timeline-item {
                width: 100%;
                padding-left: 40px;
                padding-right: 0;
                text-align: left;
            }
            .timeline-item:nth-child(odd) {
                 padding-right: 0;
            }
             .timeline-item:nth-child(even) {
                left: 0%;
                padding-left: 40px;
            }
            .timeline-dot {
                left: 0;
            }
            .timeline-item:nth-child(odd) .timeline-dot {
                left: 0;
            }
        }

    </style>
</head>
<body class="text-slate-700">

    <!-- Header -->
    <header class="bg-white">
         <div class="container mx-auto px-6 py-12 text-center bg-gradient-to-br from-blue-50 to-indigo-100 rounded-b-3xl">
            <h1 class="text-4xl md:text-5xl font-extrabold text-slate-900">Análise Estratégica</h1>
            <p class="mt-3 text-lg text-blue-700 font-semibold">Posicionamento no mercado — Múltiplas Marcas no Portfólio</p>
        </div>
    </header>

    <main class="container mx-auto px-6 py-12 md:py-20">

        <!-- Cenário Atual -->
        <section id="cenario" class="mb-20 fade-in-section">
            <div class="max-w-3xl mx-auto bg-blue-50 border-l-4 border-blue-600 p-8 rounded-lg shadow-sm">
                <h2 class="text-2xl font-bold text-slate-800 mb-4">Cenário Atual</h2>
                <p class="text-lg leading-relaxed">
                    Atualmente, a empresa possui três produtos e uma marca institucional, totalizando <span class="font-bold text-blue-700">quatro marcas ativas</span> no portfólio.
                </p>
            </div>
        </section>

        <!-- Vantagens e Desvantagens -->
        <section id="vantagens-desvantagens" class="mb-20 fade-in-section">
            <div class="grid md:grid-cols-2 gap-12">
                <!-- Vantagens -->
                <div>
                    <h2 class="text-2xl font-bold text-slate-800 mb-6 flex items-center gap-3">
                        <i data-lucide="thumbs-up" class="text-green-500"></i>
                        Vantagens
                    </h2>
                    <div class="space-y-4">
                        <div class="card flex items-start gap-4"><i data-lucide="users" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Atende diferentes perfis de clientes com propostas de valor distintas.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="shield" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Aumenta a presença de mercado e dificulta a entrada de concorrentes.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="unlink-2" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Crises em uma marca não afetam diretamente as demais.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="flask-conical" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Permite testar novas soluções com menor impacto reputacional.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="message-circle" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Possibilita comunicação direcionada e mais eficaz.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="target" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Evita diluição de posicionamento por tentar agradar a todos.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="award" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>A marca institucional pode reforçar a confiança nas demais.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="trending-up" class="w-6 h-6 text-blue-600 mt-1 shrink-0"></i><p>Um portfólio forte eleva o valor de mercado da empresa.</p></div>
                    </div>
                </div>

                <!-- Desvantagens -->
                <div>
                    <h2 class="text-2xl font-bold text-slate-800 mb-6 flex items-center gap-3">
                        <i data-lucide="thumbs-down" class="text-red-500"></i>
                        Desvantagens
                    </h2>
                    <div class="space-y-4">
                        <div class="card flex items-start gap-4"><i data-lucide="dollar-sign" class="w-6 h-6 text-red-600 mt-1 shrink-0"></i><p>Multiplicação de investimentos em branding, campanhas e suporte.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="git-merge" class="w-6 h-6 text-red-600 mt-1 shrink-0"></i><p>Exige coordenação robusta entre marcas e times.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="swords" class="w-6 h-6 text-red-600 mt-1 shrink-0"></i><p>Marcas podem disputar os mesmos clientes se não forem bem diferenciadas.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="pie-chart" class="w-6 h-6 text-red-600 mt-1 shrink-0"></i><p>Recursos e atenção da liderança são divididos.</p></div>
                        <div class="card flex items-start gap-4"><i data-lucide="help-circle" class="w-6 h-6 text-red-600 mt-1 shrink-0"></i><p>Falta de clareza na relação entre marcas prejudica a decisão de compra.</p></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Roteiro da Transformação -->
        <section id="roteiro" class="mb-20 fade-in-section">
            <h2 class="section-title">Roteiro da Transformação (2 anos)</h2>
            <div class="timeline-container">
                <!-- NOW -->
                <div class="timeline-item">
                    <div class="timeline-dot border-blue-600"></div>
                    <div class="timeline-content">
                        <h3 class="text-xl font-bold text-blue-700 mb-1">NOW</h3>
                        <p class="text-sm text-slate-500 mb-4 font-medium">(6–8 meses)</p>
                        <p class="font-semibold mb-2">Foco: Diagnóstico estratégico</p>
                        <p class="mb-4"><strong>Objetivo:</strong> Analisar melhor opção de posicionamento que gere mais valor ao grupo.</p>
                        <ul class="list-disc list-inside space-y-3 text-sm">
                            <li><strong>Definir caminho da marca:</strong><ul class="list-['›'] list-inside pl-4 mt-1 space-y-1"><li>Qual marca principal assumir?</li><li>Criar uma nova marca?</li><li>Renomear os ativos?</li><li>Manter a estrutura atual?</li></ul></li>
                            <li><strong>Analisar Base de clientes:</strong><ul class="list-['›'] list-inside pl-4 mt-1 space-y-1"><li>Mapear jornadas e identificar atritos solucionáveis com unificação.</li><li>Identificar oportunidades de integração.</li></ul></li>
                        </ul>
                    </div>
                </div>
                <!-- NEXT -->
                <div class="timeline-item">
                     <div class="timeline-dot border-purple-600"></div>
                    <div class="timeline-content">
                        <h3 class="text-xl font-bold text-purple-700 mb-1">NEXT</h3>
                        <p class="text-sm text-slate-500 mb-4 font-medium">(6–12 meses)</p>
                        <p class="font-semibold mb-2">Foco: Aproximação</p>
                        <p class="mb-4"><strong>Objetivo:</strong> Entregar valor imediato percebido, facilitar adoção cruzada e preparar o mercado para a unificação.</p>
                        <ul class="list-disc list-inside space-y-2 text-sm"><li>Manter nomes dos produtos com subtítulo ou selo ("by marca").</li><li>Aplicar identidade visual semelhante em todos os produtos.</li></ul>
                    </div>
                </div>
                 <!-- LATER -->
                <div class="timeline-item">
                    <div class="timeline-dot border-teal-600"></div>
                    <div class="timeline-content">
                        <h3 class="text-xl font-bold text-teal-700 mb-1">LATER</h3>
                        <p class="text-sm text-slate-500 mb-4 font-medium">(12–24 meses)</p>
                        <p class="font-semibold mb-2">Foco: Plataforma unificada</p>
                        <p class="mb-4"><strong>Objetivo:</strong> Consolidar as soluções em um único produto com nova identidade.</p>
                        <ul class="list-disc list-inside space-y-2 text-sm"><li>Comunicar reposicionamento com uma nova narrativa.</li></ul>
                    </div>
                </div>
            </div>
        </section>
        
         <!-- Nova Narrativa -->
        <section id="narrativa" class="fade-in-section">
            <div class="max-w-4xl mx-auto text-center bg-slate-800 text-white p-10 rounded-xl shadow-2xl">
                <h2 class="text-3xl font-bold mb-4">A Nova Narrativa da Marca</h2>
                <p class="text-lg md:text-xl italic leading-relaxed">
                    "Fomos DisparoPro, EasyCDP e Brasilfone. Agora somos uma só marca, porque integração real começa com união. Somos uma única plataforma, com uma só missão: <span class="font-bold text-blue-400">facilitar seu crescimento</span>."
                </p>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-slate-800 text-slate-400 mt-20">
        <div class="container mx-auto px-6 py-6 text-center">
            <p>&copy; 2024 Análise Estratégica. Todos os direitos reservados.</p>
        </div>
    </footer>

    <script>
        lucide.createIcons();

        // Script for fade-in animation on scroll
        const sections = document.querySelectorAll('.fade-in-section');
        const options = {
            root: null,
            rootMargin: '0px',
            threshold: 0.15
        };

        const observer = new IntersectionObserver(function(entries, observer) {
            entries.forEach(entry => {
                if (!entry.isIntersecting) {
                    return;
                }
                entry.target.classList.add('is-visible');
                observer.unobserve(entry.target);
            });
        }, options);

        sections.forEach(section => {
            observer.observe(section);
        });
    </script>
</body>
</html>
