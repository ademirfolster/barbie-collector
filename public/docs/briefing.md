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
