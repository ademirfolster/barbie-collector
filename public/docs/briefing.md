🧠 PROJETO: Landing Page — Barbie Collector (Luxo / Edição Limitada)
🎯 OBJETIVO DO PRODUTO

Criar uma landing page para:

👉 vender uma Barbie colecionável premium
👉 gerar desejo + percepção de valor + ação

🧠 O que isso muda no seu código?

Você NÃO está:

só exibindo dados (como na Pokédex)

Você está:

construindo experiência
guiando o usuário até uma ação
🧱 ESTRUTURA COMPLETA (arquitetura da página)
body
└── .container

        ├── header (navbar)
        ├── section.hero
        ├── section.sobre
        ├── section.detalhes
        ├── section.galeria
        ├── section.depoimentos
        ├── section.cta
        └── footer

👉 Isso aqui é sua “árvore mental”

🔷 1. HEADER (navbar)
Objetivo:
identidade
ação rápida
Conteúdo:
nome da marca (texto mesmo)
botão “Comprar”
Pensamento CSS:
display: flex
justify-content: space-between

👉 esquerda = logo
👉 direita = botão

🔥 2. HERO (parte mais importante)
Objetivo:

👉 causar impacto em 3 segundos

Conteúdo:
título forte
subtítulo
imagem principal
preço
botão
Estrutura mental:
.hero
├── texto
└── imagem
Pensamento CSS:

👉 mobile primeiro:

tudo em coluna

👉 depois (se quiser evoluir):

lado a lado com flex
Hierarquia:
h1 → chama atenção
p → complementa
botão → ação
🧩 3. SOBRE
Objetivo:

👉 aumentar percepção de valor

Conteúdo:
pequeno texto descritivo
CSS:
largura controlada (não deixa texto gigante)
line-height maior
💎 4. DETALHES (features)
Objetivo:

👉 justificar o preço

Conteúdo:
lista de benefícios
✓ edição limitada
✓ acabamento premium
✓ caixa colecionável
Pensamento:

👉 isso é um “bloco repetível”

CSS:
pode usar flex-direction: column
espaçamento entre itens (gap)
🖼️ 5. GALERIA (JS entra forte aqui)
Objetivo:

👉 mostrar o produto de forma interativa

Estrutura:
.galeria
├── imagem principal
└── thumbnails (imagens menores)
🔥 JS que você vai implementar:
Quando clicar na imagem pequena:

👉 ela vira a imagem principal

Lógica:
clicou thumbnail
→ pega src da imagem
→ substitui na imagem principal
🧠 Conceitos usados:
addEventListener
src
querySelectorAll
forEach
🗣️ 6. DEPOIMENTOS
Objetivo:

👉 prova social (muito importante em produto real)

Conteúdo:
texto curto
nome
CSS:
cards
sombra leve
borda arredondada
🚀 7. CTA FINAL
Objetivo:

👉 capturar o usuário indeciso

Conteúdo:
frase de urgência
botão grande
Exemplo:
Últimas unidades disponíveis
[Comprar agora]
CSS:
centralizado
destaque visual
🔻 8. FOOTER
Objetivo:
finalizar
dar credibilidade
Conteúdo:
nome
contato fictício
🎨 CSS — ESTRATÉGIA COMPLETA

Agora o mais importante.

🔥 ORDEM DE ESTILIZAÇÃO (não fuja disso)

1. body
   fonte
   fundo
   centralização
2. container
   largura máxima
   padding lateral
3. sections
   espaçamento vertical
4. layout interno (flex)
5. componentes
   botões
   cards
   imagens
6. detalhes visuais
   cores
   sombras
   hover
   🎯 PADRÕES QUE VOCÊ DEVE CRIAR
   Botão (reutilizável)
   .botao
   .botao--primario
   Card
   .card
   Seção
   .section
   .section--escura (se quiser variar)
   ⚙️ JS — FUNCIONALIDADES OBRIGATÓRIAS
   🔹 1. Galeria interativa

✔ troca imagem principal

🔹 2. Botão comprar

Simula ação:

Opção 1:

alert("Compra simulada")

Opção 2 (melhor):
👉 redireciona pro WhatsApp

🔹 3. Scroll suave

Botão leva até seção:

👉 usar:

scrollIntoView()
🔹 4. Destaque de botão

Quando clicar:

muda estilo (classe ativa)
🧠 LÓGICA DO PROJETO (visão profissional)
usuário entra
↓
vê hero (impacto)
↓
entende produto
↓
vê valor (detalhes)
↓
interage (galeria)
↓
confia (depoimentos)
↓
clica (CTA)
🚀 ORDEM DE EXECUÇÃO (REAL)
DIA 1:
HTML completo (tudo estruturado)
CSS base (layout funcionando)
Hero bonito
DIA 2:
Galeria com JS
Botões funcionando
Refino visual
🔥 DIFERENCIAL (se fizer isso, sobe de nível)

Se quiser ir além:

hover nas imagens
animação leve (transition)
botão com efeito
📊 ONDE ISSO TE COLOCA

Depois desse projeto:

👉 você já consegue fazer:

landing pages reais
páginas de produto
sites institucionais

👉 nível:
júnior inicial → júnior sólido (quase pleno visual)

⚠️ REGRAS (segue isso à risca)
NÃO começa pelo CSS bonito
NÃO mistura lógica com estilo
NÃO faz tudo de uma vez

---

---

Perfeito. Agora a gente vai fazer CSS do jeito certo — sem tentativa e erro, com método.

Vou te guiar como se estivesse do teu lado.

🧠 ESTRATÉGIA GERAL (não pula isso)

Você NÃO vai sair estilizando tudo.

Você vai seguir essa ordem:

1. Base (reset + body)
2. Container
3. Sections (espaçamento)
4. Layout (hero, navbar, etc)
5. Componentes (botão, card)
6. Refino visual

👉 Se pular ordem = bagunça

🧱 1. RESET + BASE

Cola isso no topo do seu CSS:

- {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }
  BODY
  body {
  font-family: 'Poppins', sans-serif;
  background: #f5e9dc;
  color: #111;
  }
  📦 2. CONTAINER
  .container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 2rem;
  }
  🧩 3. SECTIONS (organização vertical)
  section {
  margin-bottom: 4rem;
  }
  🔝 4. NAVBAR (primeiro layout)
  .navBar {
  display: flex;
  justify-content: space-between;
  align-items: center;

  padding: 1.5rem 2rem;
  }
  Logo
  .nav-left img {
  width: 120px;
  }
  🎯 BOTÃO (cria padrão agora)
  .btn-default {
  background: #c9a24a;
  color: white;

  padding: 10px 20px;
  border-radius: 999px;

  text-decoration: none;
  font-weight: 600;

  transition: 0.3s;
  }

.btn-default:hover {
opacity: 0.85;
}
🔥 5. HERO (parte mais importante)

Agora vem o nível.

Container do hero
.hero {
display: flex;
align-items: center;
gap: 40px;
}
Imagem
.hero-image {
width: 100%;
max-width: 400px;
border-radius: 16px;
}
Conteúdo
.hero-content {
display: flex;
flex-direction: column;
gap: 16px;
}
Título
.hero-title {
font-size: 2.5rem;
font-family: 'Playfair Display', serif;
}
Subtítulo
.hero-subtitle {
color: #666;
line-height: 1.6;
}
Preço
.hero-price {
font-size: 1.5rem;
font-weight: bold;
color: #6b3e2e;
}
🧩 6. ABOUT
.about {
padding: 3rem 0;
}
.about-content {
max-width: 600px;
margin: 0 auto;
text-align: center;
}
.about-text {
line-height: 1.6;
color: #666;
}
💎 7. FEATURES
.features {
display: flex;
justify-content: center;
gap: 30px;
}
.feature-item {
display: flex;
align-items: center;
gap: 8px;

background: white;
padding: 10px 16px;
border-radius: 12px;
}
.feature-icon {
color: #c9a24a;
}
🖼️ 8. GALERIA
.gallery {
text-align: center;
}
.gallery-principal {
width: 100%;
max-width: 400px;
margin-bottom: 20px;
border-radius: 12px;
}
.gallery-grid {
display: flex;
justify-content: center;
gap: 10px;
}
.thumb {
width: 80px;
cursor: pointer;
border-radius: 8px;
}
🗣️ 9. TESTIMONIALS
.testimonials {
display: flex;
gap: 20px;
}
.testimonial {
background: white;
padding: 20px;
border-radius: 12px;
flex: 1;
}
🚀 10. CTA
.cta-section {
text-align: center;
}
.cta-title {
font-size: 1.8rem;
margin-bottom: 10px;
}
.cta-text {
color: #666;
margin-bottom: 20px;
}
🔻 11. FOOTER
.footer {
text-align: center;
padding: 2rem;
background: #3e2419;
color: white;
}
⚠️ AGORA O MAIS IMPORTANTE

👉 NÃO tenta “deixar bonito perfeito” agora

👉 Primeiro verifica:

layout funcionando?
nada quebrado?
alinhamento ok?
🧠 CHECK FINAL (antes de avançar)
hero lado a lado
navbar alinhada
sections com espaço
nada colado
imagens proporcionais
