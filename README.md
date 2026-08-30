# 🌿 Garden Wars --- Insect Tower Defense

> A browser-based Tower Defense game inspired by the strategic tower
> evolution and crosspathing of **Bloons TD-style games**, reimagined
> around insects defending a garden against an invasion of slugs,
> snails, flying pests, and bosses.

> Um jogo de Tower Defense para navegador inspirado na estratégia de
> evolução e *crosspathing* de jogos no estilo **Bloons TD**, mas
> ambientado em um jardim onde insetos defendem seu território contra
> lesmas, caracóis, pragas voadoras e chefes.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow.svg)
![Game](https://img.shields.io/badge/Genre-Tower%20Defense-brightgreen.svg)
![Pixel
Art](https://img.shields.io/badge/Graphics-Pixel%20Art-purple.svg)

------------------------------------------------------------------------

## 🌐 Language / Idioma

-   [🇧🇷 Português](#-português)
-   [🇬🇧 English](#-english)

------------------------------------------------------------------------

# 🇧🇷 Português

## 💡 Visão Geral

**Garden Wars** é um Tower Defense desenvolvido inteiramente para
navegador, no qual o jogador precisa proteger um jardim de ondas
progressivamente mais perigosas de inimigos.

A proposta combina uma jogabilidade acessível com um sistema
relativamente profundo de evolução: o jogador recruta diferentes
espécies de insetos, posiciona suas torres estrategicamente e escolhe
entre **três caminhos de evolução**, cada um com **cinco Tiers**.

A invasão começa com lesmas, mas rapidamente ganha reforços como
**caracóis-tanque, inimigos voadores, elites e chefes**, exigindo que o
jogador adapte sua composição e seus caminhos de upgrade.

O jogo possui **seis mapas com trajetórias diferentes**, permitindo que
a posição das torres e o controle do caminho tenham impacto direto na
estratégia.

------------------------------------------------------------------------

## ⚡ Principais Funcionalidades

-   🌿 **Tower Defense em HTML5 Canvas** --- todo o jogo é executado
    diretamente no navegador.
-   🐜 **Exército de insetos** --- o jogador pode recrutar **10 tipos
    diferentes de insetos**.
-   🛤️ **6 mapas** --- cada mapa possui um traçado próprio para a
    invasão.
-   🌱 **3 caminhos de evolução por torre** --- cada caminho possui 5
    Tiers.
-   🔀 **Sistema de Crosspathing** --- é possível levar um caminho até
    T5 e um segundo caminho até T2, enquanto o terceiro permanece
    bloqueado.
-   ✨ **Habilidades ativas** --- determinadas evoluções desbloqueiam
    habilidades com cooldown próprio.
-   🐌 **Diversidade de inimigos** --- lesmas, caracóis, elites,
    inimigos voadores e variantes especiais.
-   👑 **Chefes e inimigos especiais** --- inimigos mais resistentes
    introduzem desafios diferentes ao longo das ondas.
-   💰 **Economia baseada em moedas** --- derrotar inimigos permite
    investir em novas torres e evoluções.
-   ♻️ **Venda de torres** --- torres podem ser vendidas recuperando 60%
    do valor.
-   🔄 **Reset de caminhos** --- permite recuperar 50% das moedas
    investidas em um caminho para mudar a estratégia.
-   🤖 **Autoplay** --- opção para deixar as ondas avançarem
    automaticamente.
-   ⏩ **Controle de velocidade** --- permite acelerar a simulação do
    jogo.
-   🏆 **Recorde de maior onda** --- o melhor resultado é armazenado
    usando `localStorage`, com fallback em memória caso o navegador não
    permita armazenamento.
-   🔊 **Controle de áudio** --- o jogo possui opção para ativar ou
    desativar o som.
-   🎨 **Pixel Art procedural** --- os sprites dos insetos são
    desenhados diretamente no Canvas utilizando formas e padrões
    pixelados.

------------------------------------------------------------------------

## 🧠 Sistema de Evolução

Cada inseto possui três especializações independentes.

``` text
                    ┌───────────────┐
                    │    INSETO     │
                    └───────┬───────┘
                            │
             ┌──────────────┼──────────────┐
             ▼              ▼              ▼
        Caminho 1       Caminho 2       Caminho 3
             │              │              │
          T1 → T2 → T3 → T4 → T5
             │
             └── Especialização principal

Regra de Crosspath:
• Um caminho pode chegar ao T5
• Um segundo caminho pode chegar ao T2
• O terceiro caminho fica bloqueado
```

Isso cria decisões estratégicas diferentes para a mesma torre. Em vez de
simplesmente aumentar dano, as evoluções podem alterar:

-   dano;
-   alcance;
-   cadência de ataque;
-   velocidade dos projéteis;
-   dano em área;
-   perfuração / múltiplos alvos;
-   veneno;
-   lentidão;
-   atordoamento;
-   empurrão;
-   dano contra elites;
-   dano contra caracóis;
-   geração de moedas;
-   cura;
-   redução de custos;
-   bônus para torres próximas;
-   efeitos de área;
-   habilidades ativas.

------------------------------------------------------------------------

## 🐛 Exemplos de Insetos

### 🦗 Gafanhoto

Uma torre versátil com especializações que vão desde ataques
extremamente rápidos até formas pesadas capazes de controlar inimigos.

Alguns exemplos de evolução:

-   **Hero Mode**
-   **Gafanhoto-do-Deserto**
-   **Gafanhoto-Pedra**
-   **Grasshopper Zero-One**
-   **Titan do Triássico**

O sistema de evolução também altera visualmente os insetos, adicionando
elementos como armaduras, viseiras, placas e outras características
especiais.

### 🐝 Abelha

Uma torre especializada em ataques contra diferentes tipos de inimigos e
em fornecer suporte para outras torres.

Exemplos:

-   **Vespão-Mandarim**
-   **Abelha-Rainha**
-   **Enxame de Operárias**

Algumas evoluções fornecem efeitos de aura, redução de custos e
habilidades de enxame.

------------------------------------------------------------------------

## 🐌 Inimigos

A invasão é construída para aumentar gradualmente a dificuldade.

Entre os inimigos apresentados pelo jogo estão:

-   **Lesmas** --- inimigos básicos.
-   **Caracóis** --- unidades mais resistentes introduzidas a partir das
    primeiras ondas.
-   **Elites** --- inimigos que exigem torres e upgrades especializados.
-   **Pragas voadoras** --- exigem insetos capazes de atingir alvos
    aéreos.
-   **Chefes** --- unidades de grande resistência utilizadas para
    aumentar a pressão sobre o jogador.
-   **Caracol Arcano** --- inimigo especial com resistência a
    atordoamento.

A existência de diferentes resistências faz com que uma única estratégia
dificilmente seja ideal para todas as situações.

------------------------------------------------------------------------

## 🗺️ Mapas

O jogo possui **6 mapas**, cada um com uma rota diferente para os
inimigos.

Alguns exemplos:

  Mapa                 Característica
  -------------------- ------------------------------------------------
  🌱 Jardim Clássico   Traçado em zigue-zague
  🐍 Serpentina        Caminho sinuoso
  🧩 Labirinto         Grande quantidade de mudanças de direção
  🌿 Outros mapas      Rotas alternativas para diferentes estratégias

A posição das torres é limitada por regras de posicionamento: a torre
não pode ser colocada sobre o caminho dos inimigos ou excessivamente
próxima de outras torres.

------------------------------------------------------------------------

## 🎮 Controles e Interface

### Mouse

-   **Clique em uma torre do menu** → seleciona a torre para
    posicionamento.
-   **Clique no mapa** → posiciona a torre.
-   **Clique em uma torre existente** → abre suas informações e
    upgrades.
-   **Botão direito** → cancela a seleção.
-   **Botão "Usar Habilidade"** → ativa habilidades disponíveis.

### Interface

-   **Iniciar Onda** → começa a próxima onda.
-   **Pausar** → pausa a simulação.
-   **Autoplay** → inicia ondas automaticamente.
-   **Velocidade** → altera a velocidade do jogo.
-   **Vender Torre** → remove a torre e recupera parte do investimento.
-   **Resetar caminho** → permite reconstruir uma especialização.

------------------------------------------------------------------------

## ⚙️ Arquitetura Técnica

O projeto foi desenvolvido sem frameworks ou engines externas,
utilizando principalmente:

-   **HTML5**
-   **CSS3**
-   **JavaScript**
-   **HTML5 Canvas**
-   **Web APIs**, incluindo `localStorage`

O Canvas utiliza renderização pixelada com
`imageSmoothingEnabled = false`, mantendo a aparência visual baseada em
pixel art.

O loop principal utiliza `setInterval` com cálculo de `delta time`
baseado em `performance.now()`. Isso permite que o jogo continue
atualizando mesmo quando a aba perde foco, enquanto limita o `dt` para
evitar saltos exagerados de simulação quando a página fica em segundo
plano.

------------------------------------------------------------------------

## 🧩 Estrutura do Projeto

A versão atual foi desenvolvida como um projeto compacto, concentrando a
lógica principal em um único arquivo HTML:

``` text
Garden-Wars/
├── Garden-Wars.html       # Jogo completo
├── README.md              # Documentação
└── LICENSE                # Licença do projeto
```

A implementação reúne no HTML:

``` text
HTML
 ├── Interface
 ├── Menus
 ├── Canvas
 └── Overlays

CSS
 ├── Layout
 ├── Interface
 ├── Menu de mapas
 └── Estilo visual

JavaScript
 ├── Mapas
 ├── Estado do jogo
 ├── Torres
 ├── Evoluções
 ├── Inimigos
 ├── Projéteis
 ├── Colisões
 ├── Ondas
 ├── Economia
 ├── Habilidades
 ├── Renderização
 └── Persistência do recorde
```

------------------------------------------------------------------------

## 🚀 Como Executar

Não é necessário instalar dependências ou configurar um servidor.

### 1. Clone o repositório

``` bash
git clone https://github.com/Jos3ng/Garden-Wars.git
```

### 2. Entre na pasta

``` bash
cd Garden-Wars
```

### 3. Execute

Abra o arquivo:

``` text
Garden-Wars.html
```

em um navegador moderno.

Também é possível simplesmente abrir o arquivo diretamente pelo
explorador de arquivos.

------------------------------------------------------------------------

## 🎯 Objetivo do Projeto

O objetivo do **Garden Wars** é explorar a implementação de um jogo de
Tower Defense do zero utilizando tecnologias web básicas.

Além da parte visual e de gameplay, o projeto envolve conceitos como:

-   programação orientada a estado;
-   estruturas de dados para definir torres e upgrades;
-   detecção de colisões;
-   vetores e distância euclidiana;
-   gerenciamento de entidades;
-   sistemas de cooldown;
-   máquinas de estado;
-   game loops;
-   cálculo de `delta time`;
-   balanceamento de atributos;
-   persistência de dados no navegador;
-   renderização procedural em Canvas.

O sistema de torres foi estruturado para que novos insetos, caminhos e
efeitos possam ser adicionados sem precisar reescrever toda a lógica de
combate.

------------------------------------------------------------------------

## 🔮 Possíveis Expansões

Algumas ideias naturais para futuras versões:

-   [ ] Mais mapas.
-   [ ] Mais espécies de insetos.
-   [ ] Mais tipos de inimigos.
-   [ ] Sistema de ondas com eventos especiais.
-   [ ] Sistema de dificuldade.
-   [ ] Menu de seleção de dificuldade.
-   [ ] Mais efeitos visuais.
-   [ ] Sistema de partículas.
-   [ ] Sistema de conquistas.
-   [ ] Sons e músicas adicionais.
-   [ ] Melhor balanceamento entre torres.
-   [ ] Separação do JavaScript em módulos.
-   [ ] Portabilidade para uma engine de jogo.

------------------------------------------------------------------------

`<br>`{=html}

------------------------------------------------------------------------

# 🇬🇧 English

## 💡 Overview

**Garden Wars** is a browser-based Tower Defense game where the player
must protect a garden from progressively stronger waves of enemies.

The game combines accessible gameplay with a deeper upgrade system:
players recruit different insect species, strategically place their
towers, and choose between **three evolution paths**, each containing
**five tiers**.

The invasion starts with basic slugs but progressively introduces
**armored snails, flying pests, elite enemies, special enemies, and
bosses**, forcing the player to adapt their tower composition and
upgrade strategy.

The game currently contains **six maps with different enemy paths**,
making tower positioning an important part of the gameplay.

------------------------------------------------------------------------

## ⚡ Key Features

-   🌿 **HTML5 Canvas Tower Defense** --- runs directly in a modern web
    browser.
-   🐜 **Insect Army** --- **10 different insect towers** are available.
-   🗺️ **6 Maps** --- each map has its own enemy route.
-   🌱 **3 Upgrade Paths per Tower** --- each path contains 5 tiers.
-   🔀 **Crosspathing System** --- one path can reach T5, a second path
    can reach T2, while the third becomes locked.
-   ✨ **Active Abilities** --- specific upgrades unlock abilities with
    individual cooldowns.
-   🐌 **Multiple Enemy Types** --- slugs, snails, elites, flying
    enemies, and special variants.
-   👑 **Bosses and Special Enemies** --- stronger units create
    additional strategic pressure.
-   💰 **Coin Economy** --- defeating enemies provides resources for
    towers and upgrades.
-   ♻️ **Tower Selling** --- towers return 60% of their value when sold.
-   🔄 **Path Reset** --- resets an upgrade path while returning 50% of
    its invested coins.
-   🤖 **Autoplay Mode** --- automatically progresses through waves.
-   ⏩ **Game Speed Control** --- speeds up the simulation.
-   🏆 **Best Wave Record** --- the highest reached wave is persisted
    through `localStorage`.
-   🔊 **Audio Toggle** --- enables or disables game audio.
-   🎨 **Procedural Pixel Art** --- insect sprites are generated
    directly on the Canvas.

------------------------------------------------------------------------

## 🧠 Upgrade System

Every insect has three specialization paths with five tiers each.

``` text
                    ┌───────────────┐
                    │     INSECT    │
                    └───────┬───────┘
                            │
             ┌──────────────┼──────────────┐
             ▼              ▼              ▼
          Path 1          Path 2          Path 3
             │              │              │
          T1 → T2 → T3 → T4 → T5
             │
             └── Main specialization

Crosspathing:
• One path can reach T5
• A second path can reach T2
• The third path becomes locked
```

Upgrades can modify damage, range, attack speed, splash damage,
projectile behavior, status effects, economy, support auras, and active
abilities.

------------------------------------------------------------------------

## 🐛 Insects

The game currently features **10 different insect towers**, each
designed around different combat or support roles.

Examples include:

-   🦗 **Grasshopper**
-   🐝 **Bee**
-   🦋 **Moth**
-   🐜 **Ant**

Each species can evolve into radically different specializations,
including offensive, support, control, economic, and anti-elite roles.

------------------------------------------------------------------------

## 🐌 Enemies

Enemy difficulty increases as waves progress.

The game includes:

-   **Slugs** --- basic enemies.
-   **Snails** --- heavily resistant enemies.
-   **Elite enemies** --- require specialized tower builds.
-   **Flying pests** --- require towers capable of attacking airborne
    targets.
-   **Bosses** --- high-health enemies that pressure the player's
    defense.
-   **Arcane Snail** --- a special enemy immune to stun effects.

------------------------------------------------------------------------

## 🗺️ Maps

Garden Wars contains **six different maps**, each with its own route.

Examples include:

-   **Classic Garden**
-   **Serpentine**
-   **Labyrinth**
-   and additional alternate layouts.

Because tower placement is restricted around enemy paths and nearby
towers, every map encourages different defensive layouts.

------------------------------------------------------------------------

## 🎮 Controls

### Mouse

-   **Click an insect in the shop** → select it for placement.
-   **Click the map** → place the tower.
-   **Click an existing tower** → open its information and upgrade
    panel.
-   **Right click** → cancel selection.
-   **Ability button** → activate available abilities.

### Interface

-   **Start Wave** → starts the next wave.
-   **Pause** → pauses the game.
-   **Autoplay** → automatically starts waves.
-   **Speed** → changes simulation speed.
-   **Sell Tower** → removes a tower and refunds part of its value.
-   **Reset Path** → refunds part of the investment in an upgrade path.

------------------------------------------------------------------------

## ⚙️ Technical Stack

The project was built without external frameworks or game engines.

**Technologies:**

-   HTML5
-   CSS3
-   Vanilla JavaScript
-   HTML5 Canvas
-   Browser Web APIs
-   `localStorage`

The Canvas uses pixelated rendering to preserve the game's retro visual
style.

The main game loop uses `setInterval` together with `performance.now()`
to calculate elapsed time and keep gameplay simulation independent from
rendering timing.

------------------------------------------------------------------------

## 🧩 Project Structure

The current version is intentionally compact:

``` text
Garden-Wars/
├── Garden-Wars.html       # Complete game
├── README.md              # Documentation
└── LICENSE                # Project license
```

The HTML file contains the complete implementation:

``` text
HTML
 ├── UI
 ├── Menus
 ├── Canvas
 └── Overlays

CSS
 ├── Layout
 ├── UI styling
 ├── Map selection
 └── Visual theme

JavaScript
 ├── Maps
 ├── Game state
 ├── Towers
 ├── Upgrades
 ├── Enemies
 ├── Projectiles
 ├── Collision detection
 ├── Waves
 ├── Economy
 ├── Abilities
 ├── Rendering
 └── Record persistence
```

------------------------------------------------------------------------

## 🚀 Getting Started

No dependencies or build tools are required.

### 1. Clone the repository

``` bash
git clone https://github.com/Jos3ng/Garden-Wars.git
```

### 2. Enter the project directory

``` bash
cd Garden-Wars
```

### 3. Run the game

Open:

``` text
Garden-Wars.html
```

in any modern web browser.

The game can also be launched directly by double-clicking the HTML file.

------------------------------------------------------------------------

## 🎯 Project Goals

**Garden Wars** was created as an exploration of building a complete
Tower Defense game from scratch using fundamental web technologies.

The project involves concepts such as:

-   state-driven programming;
-   data structures for towers and upgrades;
-   collision detection;
-   vector mathematics;
-   entity management;
-   cooldown systems;
-   state machines;
-   game loops;
-   delta-time simulation;
-   gameplay balancing;
-   browser persistence;
-   procedural Canvas rendering.

The tower definition system was designed so that new insects, upgrade
paths, and effects can be added without rewriting the entire combat
system.

------------------------------------------------------------------------

## 🔮 Future Improvements

Potential future additions include:

-   [ ] More maps.
-   [ ] More insect species.
-   [ ] More enemy types.
-   [ ] Special wave events.
-   [ ] Difficulty system.
-   [ ] Difficulty selection.
-   [ ] More visual effects.
-   [ ] Particle system.
-   [ ] Achievement system.
-   [ ] Additional music and sound effects.
-   [ ] Further tower balancing.
-   [ ] Modular JavaScript architecture.
-   [ ] Porting to a dedicated game engine.

------------------------------------------------------------------------

## 📜 License / Licença

Distributed under the MIT License. See `LICENSE` for more information.

------------------------------------------------------------------------

*Built with JavaScript, Canvas, pixel art, and an unreasonable number of
insects.* 🐜🌿
