## 🧘 Roda da Vida (Life Wheel)

Este é um projeto simples e interativo, construído com **HTML, CSS e JavaScript Vanilla**, que implementa a popular ferramenta de *Coaching* e autoconhecimento conhecida como **Roda da Vida** (*Life Wheel*).

A Roda da Vida é um diagrama que ajuda indivíduos a visualizar e avaliar o nível de satisfação em diversas áreas chave de suas vidas, promovendo o equilíbrio e o foco no desenvolvimento pessoal.

-----

### ✨ Funcionalidades

  * **Avaliação Interativa:** O usuário pode clicar ou arrastar no gráfico para atribuir uma pontuação (de 1 a 10) para cada uma das 12 áreas da vida.
  * **Visualização Dinâmica:** O gráfico de radar (Roda) é atualizado instantaneamente conforme as pontuações são inseridas, mostrando visualmente as áreas que precisam de mais atenção.
  * **Exportação em PDF:** Permite que o usuário baixe o resultado da sua avaliação (incluindo o gráfico e a lista de pontuações) como um documento PDF.

[Image of Life Wheel Chart]

  * **Definição de Ação:** Há um campo para o usuário registrar o que fará para melhorar a área de menor pontuação.

-----

### 💻 Tecnologias Utilizadas

| Tecnologia | Descrição |
| :--- | :--- |
| **HTML5** | Estrutura base da interface e do formulário. |
| **CSS3** | Estilização moderna (Dark Theme) e responsividade. |
| **JavaScript (Vanilla)** | Lógica para cálculo, manipulação do gráfico, e processamento das ações (PDF, Email). |
| **`Chart.js`** | Biblioteca utilizada para renderizar o gráfico de radar dinâmico da Roda da Vida. |
| **`jspdf`** | Biblioteca utilizada para a criação do documento PDF. |
| **`dom-to-image-more`** | Biblioteca para capturar o gráfico e os dados (HTML/CSS) em imagem antes de serem inseridos no PDF. |

-----

### 🚀 Como Configurar e Rodar

Este projeto é totalmente *front-end* e não requer servidor.

1.  **Clone o repositório:**
    ```bash
    git clone [LINK DO SEU REPOSITÓRIO]
    ```
2.  **Abra o arquivo:**
    Abra o arquivo `roda-da-vida.html` (ou o nome que você salvou) em seu navegador web.
3.  **Interação:**
    Clique e arraste os pontos ou use os campos de input para definir a pontuação de 1 a 10 para cada área.

-----

### ⚙️ Estrutura do Código

O projeto está contido em um único arquivo HTML para simplicidade, organizado da seguinte forma:

1.  **CSS:** Contém todas as regras de estilo e definição de variáveis do tema.
2.  **HTML:**
      * `canvas#radarChart`: Onde o gráfico é desenhado.
      * `div#input-grid`: Contém os 12 campos de input para as pontuações.
3.  **JavaScript:**
      * **Inicialização do `Chart.js`:** Define o layout inicial do gráfico de radar.
      * **Listeners:** Captura as alterações nos inputs e atualiza o gráfico em tempo real.
      * **`generatePdf()`:** Contém a lógica de captura do DOM (`dom-to-image-more`) e a criação do PDF (`jspdf`) para exportação dos resultados.


