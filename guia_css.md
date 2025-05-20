# Guia Completo de Propriedades CSS

Este guia apresenta as principais propriedades CSS organizadas por seções, com suas funções e exemplos.

---

## 🔹 1. Layout e Posicionamento

| Propriedade         | Função                                                  | Exemplo                        |
|---------------------|----------------------------------------------------------|--------------------------------|
| `display`           | Define o tipo de caixa de renderização (block, flex, etc) | `display: flex;`              |
| `position`          | Define o método de posicionamento (static, absolute...) | `position: absolute;`         |
| `top, right, bottom, left` | Define a posição em relação ao contêiner | `top: 10px;`                  |
| `z-index`           | Define a ordem de empilhamento                          | `z-index: 5;`                 |
| `float`             | Posiciona elementos ao lado (obsoleto com flex/grid)    | `float: left;`               |
| `clear`             | Cancela floats                                           | `clear: both;`                |
| `flex`, `justify-content`, `align-items` | Layout flexível e alinhamento        | `display: flex; justify-content: center;` |
| `grid`, `grid-template-columns`, `grid-gap` | Layout em grade                  | `display: grid; grid-template-columns: repeat(3, 1fr);` |

---

## 🔹 2. Tamanho e Espaçamento

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `width`, `height`  | Largura e altura                                 | `width: 100px;`                |
| `max-width`, `min-width` | Limites de largura                         | `max-width: 600px;`            |
| `margin`           | Espaçamento externo                              | `margin: 10px 20px;`           |
| `padding`          | Espaçamento interno                              | `padding: 15px;`               |
| `box-sizing`       | Define se o `padding` e `border` contam no tamanho total | `box-sizing: border-box;` |

---

## 🔹 3. Tipografia

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `font-family`      | Tipo de fonte                                    | `font-family: Arial, sans-serif;` |
| `font-size`        | Tamanho da fonte                                 | `font-size: 16px;`             |
| `font-weight`      | Espessura da fonte                               | `font-weight: bold;`           |
| `line-height`      | Altura da linha                                  | `line-height: 1.5;`            |
| `text-align`       | Alinhamento horizontal                           | `text-align: center;`          |
| `text-decoration`  | Sublinhar, riscar, etc                           | `text-decoration: underline;`  |
| `text-transform`   | Capitalização de texto                           | `text-transform: uppercase;`   |
| `letter-spacing`, `word-spacing` | Espaço entre letras/palavras     | `letter-spacing: 2px;`         |

---

## 🔹 4. Cores e Fundo

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `color`            | Cor do texto                                     | `color: #333;`                 |
| `background-color` | Cor de fundo                                     | `background-color: #f1f1f1;`   |
| `background-image` | Imagem de fundo                                  | `background-image: url("img.jpg");` |
| `background-size`  | Tamanho da imagem de fundo                       | `background-size: cover;`      |
| `background-repeat`| Repetição de fundo                               | `background-repeat: no-repeat;`|
| `opacity`          | Opacidade                                         | `opacity: 0.8;`                |

---

## 🔹 5. Borda e Sombra

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `border`           | Define uma borda                                 | `border: 1px solid #000;`      |
| `border-radius`    | Bordas arredondadas                              | `border-radius: 10px;`         |
| `box-shadow`       | Sombra em volta da caixa                         | `box-shadow: 0 4px 8px rgba(0,0,0,0.2);` |

---

## 🔹 6. Animações e Transições

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `transition`       | Anima transições de propriedades                 | `transition: all 0.3s ease;`   |
| `animation`        | Define animações completas (com `@keyframes`)    | `animation: pulse 2s infinite;`|
| `transform`        | Transforma elementos (escala, rotação, etc)      | `transform: scale(1.1);`       |
| `@keyframes`       | Define os quadros da animação                    | `@keyframes pulse { from { opacity: 1; } to { opacity: 0.5; } }` |

---

## 🔹 7. Responsividade e Media Queries

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `@media`           | Estilos condicionais por tamanho de tela         | `@media (max-width: 768px) { ... }` |
| `viewport units`   | Unidades relativas à tela (`vw`, `vh`)           | `width: 100vw; height: 100vh;` |
| `clamp()`, `min()`, `max()` | Funções para escalas responsivas      | `font-size: clamp(1rem, 2vw, 2rem);` |

---

## 🔹 8. Cursor e Interatividade

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `cursor`           | Tipo de cursor ao passar o mouse                 | `cursor: pointer;`             |
| `pointer-events`   | Controla se o elemento responde a cliques        | `pointer-events: none;`        |
| `user-select`      | Define se o usuário pode selecionar o texto      | `user-select: none;`           |

---

## 🔹 9. Outros Avançados e Utilitários

| Propriedade        | Função                                           | Exemplo                        |
|--------------------|--------------------------------------------------|--------------------------------|
| `visibility`       | Visibilidade (oculta mas mantém espaço)          | `visibility: hidden;`          |
| `overflow`         | Como o conteúdo transborda do contêiner          | `overflow: auto;`              |
| `clip-path`        | Máscara de corte (formas)                        | `clip-path: circle(50%);`      |
| `filter`           | Efeitos visuais como blur                        | `filter: blur(4px);`           |
| `mix-blend-mode`   | Modo de mesclagem de camadas                     | `mix-blend-mode: multiply;`    |
