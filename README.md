# Rota-da-Oca-do-Sol-
site <!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rota da Oca do Sol — Ecossistema Multicultural e Regenerativo</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Plus Jakarta Sans', sans-serif; }
        .font-cinzel { font-family: 'Cinzel', serif; }
    </style>
</head>
<body class="bg-stone-950 text-stone-100 antialiased selection:bg-amber-600 selection:text-white">

    <!-- Header / Navegação -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-stone-950/80 backdrop-blur-md border-b border-stone-800">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <div class="flex items-center space-x-3">
                <span class="text-2xl font-cinzel tracking-widest text-amber-500 font-bold">ROTA DA OCA DO SOL</span>
            </div>
            <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-stone-300">
                <a href="#manifesto" class="hover:text-amber-400 transition">Manifesto</a>
                <a href="#galeria" class="hover:text-amber-400 transition">Atelier & Bioeconomia</a>
                <a href="#travessia" class="hover:text-amber-400 transition">A Travessia</a>
                <button onclick="openModal()" class="bg-amber-600 hover:bg-amber-500 text-stone-950 font-semibold px-5 py-2.5 rounded-full transition shadow-lg shadow-amber-900/20">
                    Baixar Pitch Deck
                </button>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center justify-center pt-20 px-6 overflow-hidden">
        <div class="absolute inset-0 z-0 opacity-40 bg-[radial-gradient(circle_at_center,_var(--tw-gradient-stops))] from-amber-950/40 via-stone-950 to-stone-950"></div>
        <div class="relative z-10 max-w-4xl text-center space-y-8">
            <span class="inline-block text-xs uppercase tracking-[0.3em] px-4 py-1.5 rounded-full bg-amber-500/10 text-amber-400 border border-amber-500/20 font-semibold">
                Economia Solidária & Ancestralidade
            </span>
            <h1 class="text-4xl md:text-6xl lg:text-7xl font-cinzel font-bold tracking-wide leading-tight">
                Reconectando Humanidade, Ancestralidade e Natureza através da Arte.
            </h1>
            <p class="text-lg md:text-xl text-stone-400 max-w-2xl mx-auto font-light leading-relaxed">
                Um ecossistema cultural e regenerativo idealizado para integrar cinema, saberes tradicionais, bioeconomia e restauração territorial.
            </p>
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4 pt-4">
                <button onclick="openModal()" class="w-full sm:w-auto bg-amber-600 hover:bg-amber-500 text-stone-950 font-bold px-8 py-4 rounded-full transition duration-300 shadow-xl shadow-amber-600/20">
                    Baixar Pitch Deck de Investimento
                </button>
                <a href="#galeria" class="w-full sm:w-auto bg-stone-900 hover:bg-stone-800 text-stone-200 border border-stone-800 font-medium px-8 py-4 rounded-full transition duration-300">
                    Conhecer o Atelier & Lore Botânica
                </a>
            </div>
        </div>
    </section>

    <!-- Módulo Galeria / Atelier de Economia Solidária -->
    <section id="galeria" class="py-24 px-6 bg-stone-900/40 border-t border-stone-900">
        <div class="max-w-7xl mx-auto space-y-12">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-6">
                <div>
                    <span class="text-amber-500 text-xs font-bold tracking-widest uppercase">RF-10 & RF-11 — Coleção Exclusiva</span>
                    <h2 class="text-3xl md:text-4xl font-cinzel font-bold mt-2">Galeria Viva & Bioeconomia</h2>
                </div>
                <!-- Botão de Upload Local para testar as fotos da pasta do PC -->
                <div>
                    <label class="cursor-pointer bg-stone-800 hover:bg-stone-700 text-stone-200 text-sm font-medium px-5 py-3 rounded-xl border border-stone-700 transition inline-flex items-center gap-2">
                        <span>📁 Carregar Fotos da Pasta Local</span>
                        <input type="file" id="localFolderInput" webkitdirectory directory multiple class="hidden" onchange="handleLocalFiles(event)">
                    </label>
                </div>
            </div>

            <!-- Grid de Produtos / Obras -->
            <div id="galleryGrid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card Padrão 1 -->
                <div class="bg-stone-900 rounded-2xl border border-stone-800 overflow-hidden flex flex-col group hover:border-amber-500/50 transition">
                    <div class="h-64 bg-stone-800 relative overflow-hidden flex items-center justify-center">
                        <span class="text-stone-500 text-sm font-medium">Foto: Obra / Escultura Autoral</span>
                        <span class="absolute top-4 left-4 bg-amber-500 text-stone-950 text-xs font-bold px-3 py-1 rounded-full uppercase tracking-wider">Edição Limitada</span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between space-y-4">
                        <div>
                            <span class="text-xs text-amber-500 font-semibold tracking-wider uppercase">Chancela MTE — Economia Solidária</span>
                            <h3 class="text-xl font-cinzel font-bold mt-1">Virgem dos Remédios (Réplica Autoral)</h3>
                            <p class="text-stone-400 text-sm mt-2 font-light">Escultura moldada em elementos orgânicos e argila, carregando a memória fitoquímica da travessia.</p>
                        </div>
                        <div class="pt-4 border-t border-stone-800 text-xs text-stone-400 bg-stone-950/40 p-3 rounded-lg">
                            🌿 <strong class="text-stone-300">Impacto Territorial:</strong> Apoia diretamente a proteção de nascentes e o mapeamento etnobotânico.
                        </div>
                        <button onclick="alert('Redirecionando para aquisição consciente da obra.')" class="w-full bg-stone-800 hover:bg-amber-600 hover:text-stone-950 text-stone-200 font-semibold py-3 rounded-xl transition text-sm">
                            Adquirir Peça Exclusiva
                        </button>
                    </div>
                </div>

                <!-- Card Padrão 2 -->
                <div class="bg-stone-900 rounded-2xl border border-stone-800 overflow-hidden flex flex-col group hover:border-amber-500/50 transition">
                    <div class="h-64 bg-stone-800 relative overflow-hidden flex items-center justify-center">
                        <span class="text-stone-500 text-sm font-medium">Foto: Kit Ritual Fogo Vivo</span>
                        <span class="absolute top-4 left-4 bg-amber-500 text-stone-950 text-xs font-bold px-3 py-1 rounded-full uppercase tracking-wider">Lore Botânica</span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between space-y-4">
                        <div>
                            <span class="text-xs text-amber-500 font-semibold tracking-wider uppercase">Selo de Origem Ancestral</span>
                            <h3 class="text-xl font-cinzel font-bold mt-1">Kit Ritual Fogo Vivo</h3>
                            <p class="text-stone-400 text-sm mt-2 font-light">Formulação botânica concentrada e óleos ritualísticos para ancoragem e energia vital.</p>
                        </div>
                        <div class="pt-4 border-t border-stone-800 text-xs text-stone-400 bg-stone-950/40 p-3 rounded-lg">
                            🌿 <strong class="text-stone-300">Impacto Territorial:</strong> 100% da renda revertida para a autonomia comunitária e bioeconomia.
                        </div>
                        <button onclick="alert('Redirecionando para aquisição do kit ritual.')" class="w-full bg-stone-800 hover:bg-amber-600 hover:text-stone-950 text-stone-200 font-semibold py-3 rounded-xl transition text-sm">
                            Adquirir Kit Ritual
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Modal de Captura de Leads (Pitch Deck) -->
    <div id="leadModal" class="fixed inset-0 z-50 bg-stone-950/80 backdrop-blur-sm hidden items-center justify-center p-4">
        <div class="bg-stone-900 border border-stone-800 rounded-3xl max-w-lg w-full p-8 relative shadow-2xl space-y-6">
            <button onclick="closeModal()" class="absolute top-6 right-6 text-stone-400 hover:text-white text-xl font-bold">✕</button>
            
            <div class="space-y-2">
                <span class="text-amber-500 text-xs font-bold tracking-widest uppercase">Acesso Exclusivo</span>
                <h3 class="text-2xl font-cinzel font-bold">Baixar Pitch Deck de Investimento</h3>
                <p class="text-stone-400 text-sm">Preencha seus dados para receber imediatamente o documento estratégico da Rota da Oca do Sol (PDF).</p>
            </div>

            <form onsubmit="handleLeadSubmit(event)" class="space-y-4">
                <div>
                    <label class="block text-xs font-medium text-stone-300 mb-1">Nome Completo</label>
                    <input type="text" required class="w-full bg-stone-950 border border-stone-800 rounded-xl px-4 py-3 text-stone-100 text-sm focus:outline-none focus:border-amber-500" placeholder="Seu nome">
                </div>
                <div>
                    <label class="block text-xs font-medium text-stone-300 mb-1">E-mail Profissional</label>
                    <input type="email" required class="w-full bg-stone-950 border border-stone-800 rounded-xl px-4 py-3 text-stone-100 text-sm focus:outline-none focus:border-amber-500" placeholder="seu.email@empresa.com">
                </div>
                <div>
                    <label class="block text-xs font-medium text-stone-300 mb-1">Organização / Fundo de Investimento</label>
                    <input type="text" class="w-full bg-stone-950 border border-stone-800 rounded-xl px-4 py-3 text-stone-100 text-sm focus:outline-none focus:border-amber-500" placeholder="Nome da instituição">
                </div>
                <button type="submit" class="w-full bg-amber-600 hover:bg-amber-500 text-stone-950 font-bold py-3.5 rounded-xl transition shadow-lg shadow-amber-600/20 text-sm">
                    Enviar e Baixar Apresentação
                </button>
            </form>
        </div>
    </div>

    <!-- Footer -->
    <footer class="py-12 border-t border-stone-900 text-center text-stone-500 text-sm">
        <p>© 2026 Rota da Oca do Sol. Todos os direitos reservados.</p>
    </footer>

    <script>
        function openModal() {
            document.getElementById('leadModal').classList.remove('hidden');
            document.getElementById('leadModal').classList.add('flex');
        }
        function closeModal() {
            document.getElementById('leadModal').classList.remove('flex');
            document.getElementById('leadModal').classList.add('hidden');
        }
        function handleLeadSubmit(e) {
            e.preventDefault();
            alert('Cadastro realizado com sucesso! O download do Pitch Deck da Rota da Oca do Sol foi iniciado.');
            closeModal();
        }

        // Função para simular o carregamento visual das imagens da pasta local do computador
        function handleLocalFiles(event) {
            const files = event.target.files;
            if (files.length === 0) return;
            
            const grid = document.getElementById('galleryGrid');
            // Mantém os originais ou limpa, aqui vamos adicionar os itens carregados
            for (let i = 0; i < files.length; i++) {
                const file = files[i];
                if (!file.type.startsWith('image/')) continue;

                const reader = new FileReader();
                reader.onload = function(e) {
                    const card = document.createElement('div');
                    card.className = 'bg-stone-900 rounded-2xl border border-stone-800 overflow-hidden flex flex-col group hover:border-amber-500/50 transition';
                    card.innerHTML = `
                        <div class="h-64 bg-stone-800 relative overflow-hidden flex items-center justify-center">
                            <img src="${e.target.result}" class="w-full h-full object-cover" alt="Obra local">
                            <span class="absolute top-4 left-4 bg-amber-500 text-stone-950 text-xs font-bold px-3 py-1 rounded-full uppercase tracking-wider">Acervo Pessoal</span>
                        </div>
                        <div class="p-6 flex-1 flex flex-col justify-between space-y-4">
                            <div>
                                <span class="text-xs text-amber-500 font-semibold tracking-wider uppercase">Registro da Pasta Local</span>
                                <h3 class="text-xl font-cinzel font-bold mt-1">${file.name.replace(/\.[^/.]+$/, "")}</h3>
                                <p class="text-stone-400 text-sm mt-2 font-light">Peça carregada diretamente do diretório local selecionado para o ecossistema.</p>
                            </div>
                            <div class="pt-4 border-t border-stone-800 text-xs text-stone-400 bg-stone-950/40 p-3 rounded-lg">
                                🌿 <strong class="text-stone-300">Rastreabilidade Cultural:</strong> Integrado ao painel do atelier.
                            </div>
                            <button onclick="alert('Item selecionado do acervo local.')" class="w-full bg-stone-800 hover:bg-amber-600 hover:text-stone-950 text-stone-200 font-semibold py-3 rounded-xl transition text-sm">
                                Visualizar Detalhes
                            </button>
                        </div>
                    `;
                    grid.appendChild(card);
                }
                reader.readAsDataURL(file);
            }
            alert(`${files.length} arquivo(s) carregado(s) da pasta com sucesso para a galeria do MVP!`);
        }
    </script>
</body>
</html>
