# Especificação Técnica e Roteiro de Arquitetura do Site e Plataforma Rota do Sol

## 1. Visão Geral e Posicionamento Estratégico

A plataforma digital **Rota do Sol** foi concebida não apenas como um portal web institucional ou catálogo de vendas, mas como um ecossistema multicultural e regenerativo vivo. Conforme registrado no projeto institucional e na biografia principal, a iniciativa é liderada por **Neta Honorata Maíta**, mulher afro-indígena, jurista formada pela Universidade de Brasília (UnB) com pesquisa em patentes e saúde pública, estudiosa de química orgânica na Colômbia, artista plástica, escultora e guardiã de saberes ancestrais.

A narrativa central do portal é ancorada na travessia continental realizada por Neta — retratada visualmente como a *Cavaleira Negra* em sua jornada de motocicleta e percursos fluviais pela América Latina. O site traduz essa experiência sensível e científica em uma arquitetura digital multifacetada, unindo cinema de prestígio, mapeamento georreferenciado, bioeconomia cultural e captação de investimentos internacionais de impacto social e ambiental (ESG).

```
Plataforma Rota do Sol
├── 1. Experiência Pública (Front-End Institucional)
│   ├── Hero Section & Manifesto Cinematográfico
│   ├── Mapa Interativo da Travessia (GIS / PostGIS)
│   ├── Galeria Curada — Atelier & Lore Botânica (Economia Solidária)
│   ├── Hub Audiovisual & Cinema (Trilogia de Atos)
│   └── Portal de Investidores & Transparência ESG
└── 2. Painel Multicultural (Dashboard Administrativo)
    ├── Gestão do Acervo Etnobotânico e Obras Autorais
    ├── Módulo de Rastreabilidade Cultural e Certificação
    └── Analytics de Impacto Territorial e Financeiro
```

---

## 2. Análise da Consultoria Técnica no WhatsApp: Enquadramento de Mercado e Arquitetura

A concepção das funcionalidades comerciais e da infraestrutura de tecnologia foi balizada pelas análises técnicas do engenheiro de software Pedro Henrique, registradas nas conversas de suporte e modelagem do projeto.

### 2.1 Posicionamento da Galeria e Risco de E-commerce Genérico

Conforme enfatizado na consultoria técnica do grupo de trabalho, o lançamento das peças exclusivas e dos produtos desenvolvidos por Neta (como o Atelier de esculturas e os itens de Lore Botânica) possui alto valor de atração de investimentos e engajamento do público, desde que seja enquadrado corretamente.

O engenheiro alertou que, se a primeira página do site transmitir a sensação de um "e-commerce comum de artesanato", o projeto corre o risco de perder a imponência institucional perante grandes fundos de investimento internacional (com aportes projetados entre R\$ 1.5M e R\$ 10M / £250k–£1.5M), plataformas de streaming e organismos globais como a UNESCO.

A solução estratégica definida na consultoria é posicionar a loja como o **Módulo Galeria / Atelier de Economia Solidária e Bioeconomia Cultural do Ecossistema Rota do Sol**. Desta forma, cada item comercializado é apresentado como uma obra de edição limitada vinculada à salvaguarda etnobotânica e à autonomia comunitária, com chancela formal de Economia Solidária aprovada pelo Ministério do Trabalho e Emprego (MTE).

### 2.2 Requisitos Funcionais Derivados da Consultoria (RF-10 e RF-11)

Para formalizar essa decisão estratégica na Estrutura de Requisitos de Software (SRS), foram incorporados os seguintes módulos essenciais:

*   **RF-10 — Módulo Galeria / Atelier de Economia Solidária na Home**: Apresentação de um carrossel nobre em mosaico na página principal contendo obras de arte (como esculturas e telas) e produtos biofílicos. Cada card exibirá fotografia em alta resolução, o Selo de Origem "Edição Limitada e Exclusiva Rota do Sol", o conceito ancestral/fitoquímico e o Botão de Ação (CTA) direcionado à aquisição consciente.
*   **RF-11 — Catálogo Curado com Rastreabilidade Cultural**: Exibição de ficha técnica completa de cada produto/obra, vinculando o valor arrecadado diretamente às ações de preservação ambiental do Instituto Rota do Sol. O módulo inclui um contador dinâmico de impacto (ex.: "Ao adquirir esta peça, você apoia diretamente a proteção de nascentes e o mapeamento etnobotânico no Cerrado").

---

## 3. Roteiro de Telas ("Scrime") da Plataforma Pública

A estrutura da interface pública foi dividida em cinco blocos principais, projetados para encantar o visitante, gerar autoridade intelectual e converter leads para investimentos e vendas sustentáveis.

### 3.1 Tela 1: Hero Section & Manifesto de Abertura

*   **Background Visual**: Vídeo cinematográfico em loop de alta definição mostrando Neta em sua motocicleta nas estradas sul-americanas, travessias de barco no Amazonas, montanhas andinas, rituais ao redor do fogo e paisagens do Cerrado.
*   **Headline de Capa**: *"ROTA DO SOL — Reconectando Humanidade, Ancestralidade e Natureza através da Arte."*
*   **Subheadline**: *"Um ecossistema cultural e regenerativo idealizado por Neta Honorata Maíta para integrar cinema, saberes tradicionais, bioeconomia e restauração territorial."*
*   **Chamadas para Ação (CTAs)**:
    *   `[Baixar Pitch Deck de Investimento]` (Dispara formulário de captura de lead).
    *   `[Explorar a Travessia Interativa]` (Scroll suave para o mapa GIS).
    *   `[Conhecer o Atelier & Lore Botânica]` (Acesso à loja de economia solidária).

### 3.2 Tela 2: Módulo Mapa Interativo da Travessia ("A Caminho da Cavaleira Negra")

Inspirado no *Mapa da Travessia* e na cartografia poética do projeto, o mapa interativo permite ao usuário navegar pelos pontos geográficos e energéticos da jornada de Neta:

| Ponto Geográfico | Categoria Teórica | Elemento / Lore Representada | Mídia Associada no Portal |
| :--- | :--- | :--- | :--- |
| **Brasília - DF** | Coração do Brasil / Cerrado | Portal de Partida, Jurídico e Ciência | Documentos de pesquisa UnB e arquivos OAB |
| **Amazonas** | Pulmão do Planeta / Rios | Medicina da Floresta, Batismo e Travessia | Vídeos 360° do Rio Amazonas e áudios nativos |
| **Andes & Atacama** | Coluna Vertebral / Deserto | Elevação, Conexão com o Céu e Renascimento | Fotografias de alta resolução e diários de campo |
| **Peru & Bolívia** | Templos Sagrados & Altiplano | Titicaca, Machu Picchu, Sabedoria Inca | Registros em áudio de cantos e cerimônias |
| **Colômbia (Valle del Cauca)** | Coração das Medicinas | Escultura da Virgem dos Remédios (90 cm) | Galeria 3D da escultura em gesso/argila |
| **Londres & Baku** | Portais Globais | Consciência Global, Diálogos e Paz | Proposta de difusão internacional UNESCO |

### 3.3 Tela 3: Galeria Curada do Atelier & Lore Botânica

Com base no planejamento de branding de produtos e na taxonomia premium definida para o ecossistema, o módulo e-commerce exibe três linhas principais de produtos autorais:

1.  **Linha Rituais (Kits Principais)**:
    *   *Ritual Raiz*: Foco em ancestralidade, fortalecimento e retorno ao essencial.
    *   *Ritual Fogo Vivo*: Foco em ativação da força interna, transformação e energia.
    *   *Ritual Águas Internas*: Foco em intuição, sensibilidade e cura emocional.
2.  **Linha Terra (Cosmética e Fitoquímica Ancestral)**:
    *   *Elixir da Terra*: Formulação botânica concentrada para uso diário.
    *   *Óleo Corpo Presente*: Óleo vegetal ritualístico de nutrição e ancoragem.
    *   *Sabonetes Artesanais*: Sabonete de Arruda (limpeza energética) e Sabonete de Barbatimão (regeneração e cuidado).
3.  **Linha Travessia (Artefatos Simbólicos e Obras de Arte)**:
    *   *Amuleto Travessia*: Peça artesanal carregada de simbolismo territorial.
    *   *Mapa da Travessia / Mapa Afetivo*: Impressão artística cartográfica em papel nobre.
    *   *Caderno de Retorno*: Diário para escrita emocional e registros pessoais.
    *   *Fragmentos da Travessia*: Obras visuais, esculturas exclusivas e telas moldadas por Neta Honorata durante a expedição.

```
+-----------------------------------------------------------------------------------+
|               GALERIA VIVA ROTA DO SOL — ARTES E BIOECONOMIA                      |
+-----------------------------------------------------------------------------------+
|  [ Card Obra: Virgem dos Remédios ]    [ Card Kit: Ritual Fogo Vivo ]            |
|  * Foto Autoral de Alta Resolução     * Foto do Kit e Ingredientes Botânicos      |
|  * Selo: Edição Limitada Rota do Sol   * Selo: Chancela Economia Solidária MTE    |
|  * História: Moldada em El Queremal   * Rastreabilidade: Impacto na Conservação    |
|  * CTA: [ Adquirir Peça Exclusiva ]    * CTA: [ Adquirir Kit Ritual ]             |
+-----------------------------------------------------------------------------------+
```

### 3.4 Tela 4: Hub Audiovisual & Cinema de Prestígio

Seção dedicada à exibição da obra cinematográfica em três atos, desenhada para o circuito de festivais internacionais e plataformas de streaming:

*   **Ato I — A Ruptura**: O desapego dos bens materiais em Brasília pós-homenagem da OAB, o batismo na Chapada dos Veadeiros e a travessia de barco pelo Rio Amazonas até a Tríplice Fronteira.
*   **Ato II — A Travessia e o Espelho**: A integração com a equipe de cinema mexicana na selva, a chegada a El Queremal na Colômbia, a criação da escultura da Virgem dos Remédios e o diálogo fluido em espanhol e línguas nativas.
*   **Ato III — O Retorno Modificado**: O rezo de ativação e proteção das águas e a mensagem final de reconexão planetária.

### 3.5 Tela 5: Portal de Investidores & Transparência ESG

Projetado especificamente para atração de fundos filantrópicos, empresas parceiras e organismos multilaterais:

*   **Matriz de Impacto Alinhada aos ODS da ONU**: Apresentação de metas em conservação hídrica (ODS 6), ação contra a mudança global do clima (ODS 13), vida terrestre (ODS 15) e igualdade de gênero e diversidade (ODS 5).
*   **Download Automatizado do Pitch Deck**: Módulo com formulário de qualificação (*lead generation*) para envio automático da apresentação executiva em PDF aos potenciais investidores.
*   **Garantias de Governança Jurídica**: Apresentação da estrutura institucional do Instituto Rota do Sol, registros de CNPJ, chancelas do MTE e relatórios de auditoria.

---

## 4. Especificação Funcional do Painel/Dashboard Multicultural

O Painel Administrativo (Backend / Content Management System) foi estruturado para ser operado por Neta Honorata e pela equipe gestora do Instituto, permitindo o lançamento contínuo de materiais e o acompanhamento financeiro e social da plataforma.

```
Painel Administrativo Multicultural
├── 1. Módulo de Lançamento de Conteúdo e Diários de Campo
│   ├── Upload de fotos, registros de áudio, textos poéticos e vídeos 360°
│   └── Vinculação de mídias aos pontos do Mapa GIS da Travessia
├── 2. Gestão de Acervo, Obras de Arte e Bioeconomia
│   ├── Cadastro de novas peças de artes e kits de Lore Botânica
│   ├── Emissão de Certificados Digitais de Autenticidade para obras autorais
│   └── Controle de estoque e expedição da Loja Herbária
└── 3. Painel de Transparência Financeira e Impacto ESG
    ├── Métricas de vendas da Economia Solidária
    ├── Relatórios automatizados para prestação de contas de editais/investidores
    └── Monitoramento do contador de impacto ambiental e territorial
```

### 4.1 Módulo de Lançamento de Conteúdo e Diários de Campo

Permite cadastrar novas expedições, encontros culturais e áudios ancestrais. Ao criar um novo registro, o operador seleciona as coordenadas geográficas para atualização automática do mapa interativo na Home.

### 4.2 Módulo de Gestão de Acervo e Certificação de Autenticidade

Cada escultura, tela ou produto exclusivo cadastrado no painel recebe um código único de Rastreabilidade Cultural. O sistema gera automaticamente um **Certificado Digital de Autenticidade em PDF**, detalhando a história da peça, o conceito fitoquímico/ancestral e o impacto social gerado pela compra.

### 4.3 Módulo de Métricas e Transparência ESG

Acompanhamento em tempo real das vendas de produtos, doações e aportes de patrocinadores. O painel calcula indicadores consolidados para exportação em relatórios institucionais compatíveis com exigências da UNESCO e fundos europeus.

---

## 5. Arquitetura de Infraestrutura de TI e Estimativa Orçamentária

Com base nas definições arquiteturais da consultoria com o engenheiro Pedro Henrique, a infraestrutura adota o **Cenário B (Produção Híbrida)**, otimizando o investimento inicial e garantindo alta disponibilidade.

### 5.1 Arquitetura Híbrida de Software e Nuvem

```
INFRAESTRUTURA LOCAL (Workstations / NAS)
└── Edição de Vídeo, GIS e Modelagem Local
    └── Conexão VPN Segura
        └── AMBIENTE CLOUD (AWS / Google Cloud / Hetzner)
            ├── Frontend: Next.js / React (Hospedado em Vercel / Cloudflare)
            ├── Backend API: Node.js / Python FastAPI
            ├── Banco de Dados Relacional & Geoespacial: PostgreSQL + PostGIS
            ├── Processamento de Imagens e Processamento Pesado: Cloud GPU Instance
            └── Armazenamento de Arquivos e Mídias 360°: S3 Object Storage
```

### 5.2 Estimativa de CAPEX e OPEX (Cenário Híbrido Recomendado)

As estimativas orçamentárias preliminares para a infraestrutura tecnológica do projeto foram dimensionadas da seguinte forma:

| Categoria | Item / Especificação | Quantidade | Estimativa CAPEX (R\$) |
| :--- | :--- | :--- | :--- |
| **Estações de Trabalho** | Workstations de Desenvolvimento (32-64 GB RAM, SSD 1-2 TB) | 6 unidades | R\$ 45.000,00 |
| **Processamento GIS / IA** | Workstations GIS / Audiovisual (64-128 GB + GPU NVIDIA) | 2 unidades | R\$ 40.000,00 |
| **Servidores de Aplicação** | Servidor de Rack 1U para serviços locais/backup | 2 unidades | R\$ 50.000,00 |
| **Banco de Dados & Storage** | Servidor PostGIS dedicado + NAS local (20-40 TB) | 2 unidades | R\$ 60.000,00 |
| **Rede & Segurança** | Firewall UTM, Switches Gerenciáveis e Rack 24U | Conjunto | R\$ 31.000,00 |
| **Infraestrutura Técnica** | NO-Break Online, Climatização, CFTV e Instalações | Conjunto | R\$ 43.000,00 |
| **Reserva Técnica** | Discos de reserva, spares e contingência | Conjunto | R\$ 20.000,00 |
| **SUBTOTAL CAPEX** | Infraestrutura Física de TI Inicial | - | **R\$ 289.000,00** |
| **Contingência (20%)** | Contingência Técnica Recomendada | - | **R\$ 57.800,00** |
| **TOTAL CAPEX** | Investimento Inicial em Infraestrutura Recomendado | - | **R\$ 346.800,00 (~R\$ 350.000,00)** |

*   **Custos Operacionais Mensais (OPEX)**: Estimados entre **R\$ 15.000,00 e R\$ 40.000,00/mês**, cobrindo hospedagem Cloud (Object Storage S3 para vídeos e imagens), consumo de APIs geoespaciais, links redundantes de internet e manutenção de segurança.

---

## 6. Matriz de Requisitos de Software (SRS) e Roadmap

Para viabilizar o desenvolvimento ágil do site e da plataforma, a Matriz de Requisitos consolida as entregas em três fases:

```
Roadmap de Implantação
├── Fase 1: MVP & Lançamento Institucional (Meses 1 a 3)
│   ├── Implementação da Home, Hero Section e Manifesto
│   ├── Publicação da Galeria Curada com RF-10 e RF-11
│   └── Formulário de Captura de Leads para Pitch Deck
├── Fase 2: Experiência Interativa e Portal de Investidores (Meses 4 a 6)
│   ├── Ativação do Mapa GIS Interativo da Travessia
│   ├── Lançamento da Loja de Lore Botânica com e-commerce completo
│   └── Portal de Investidores ESG e Transparência
└── Fase 3: Expansão Imersiva e Dashboard Avançado (Meses 7 a 12)
    ├── Integração de Mídia 360° e Tours Virtuais
    ├── Emissão Automatizada de Certificados de Autenticidade
    └── Módulo de Analytics Financeiro e Social do Painel
```

| Código | Requisito Funcional | Descrição Técnica | Prioridade |
| :--- | :--- | :--- | :--- |
| **RF-01** | Download do Pitch Deck | Formulário de captura de nome/e-mail/empresa com disparo automático do PDF. | Alta (Fase 1) |
| **RF-02** | Mapa Interativo GIS | Renderização de mapas via Leaflet/Mapbox alimentado por banco PostGIS. | Alta (Fase 2) |
| **RF-10** | Galeria de Economia Solidária | Módulo na Home para exibição em carrossel nobre das peças autorais e produtos. | Alta (Fase 1) |
| **RF-11** | Rastreabilidade Cultural | Ficha detalhada do produto com conceito etnobotânico e contador de impacto social. | Alta (Fase 1) |
| **RF-12** | Emissão de Certificados | Geração automática de PDF assinado digitalmente para obras do Atelier. | Média (Fase 3) |
| **RF-13** | Painel Administrativo | Dashboard intuitivo para publicação de diários de campo e gestão do acervo. | Alta (Fase 1) |

Com este roteiro e especificação técnica, a plataforma Rota do Sol assegura um equilíbrio entre o prestígio cinematográfico institucional, a atração de grandes investimentos internacionais de impacto e a rentabilidade sustentável da bioeconomia e do atelier da artista Neta Honorata.
