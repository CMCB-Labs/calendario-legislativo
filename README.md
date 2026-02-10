# Calendário de Sessões e Reuniões

Este repositório contém o código-fonte de um calendário interativo desenvolvido em HTML, CSS e JavaScript, projetado para ser facilmente incorporado (embed) em websites, como o da Câmara Municipal de Coronel Barros/RS. O calendário exibe as sessões e reuniões agendadas para o ano de 2026, com funcionalidades que facilitam a visualização e interação do usuário.

## Funcionalidades

-   **Mês Atual Automático**: Ao carregar a página, o calendário inicia automaticamente no mês corrente, proporcionando uma experiência sempre atualizada.
-   **Destaque do Dia Atual**: O dia atual é visualmente destacado no calendário, facilitando a identificação da data presente.
-   **Eventos do Dia Selecionado**: Ao clicar em um dia, ou ao carregar a página no dia atual, os eventos agendados para aquela data são exibidos em uma seção dedicada.
-   **Navegação por Mês**: Botões intuitivos permitem a navegação rápida entre os meses do ano.
-   **Responsividade**: O layout é adaptável a diferentes tamanhos de tela, garantindo uma boa visualização em dispositivos móveis e desktops.

## Como Usar (Embed)

Para incorporar este calendário em seu website, siga os passos abaixo:

1.  **Hospede o arquivo**: Faça o upload do arquivo `index.html` (ou o nome que você preferir) para um serviço de hospedagem de páginas estáticas.
2.  **Copie o link**: Obtenha a URL pública do arquivo HTML hospedado.
3.  **Use um `<iframe>`**: No seu site, adicione um elemento `<iframe>` apontando para a URL do calendário. Exemplo:

    ```html
    <iframe 
      src="SUA_URL_DO_CALENDARIO.html" 
      style="border:0; width:100%; height:600px;" 
      title="Calendário de Sessões e Reuniões">
    </iframe>
    ```

    Ajuste os valores de `width` e `height` conforme a necessidade do seu layout.

## Estrutura do Código

O projeto é composto por um único arquivo HTML que integra CSS e JavaScript:

-   **HTML (`<head>` e `<body>`)**: Define a estrutura da página, incluindo o título, a área dos botões de mês, a grade do calendário e a área de exibição de eventos.
-   **CSS (`<style>`)**: Estiliza todos os elementos do calendário, garantindo um design limpo e responsivo. Inclui estilos para os dias, botões de mês, e o destaque para o dia atual e tipos de eventos.
-   **JavaScript (`<script>`)**: Contém a lógica para:
    -   Gerar dinamicamente a grade do calendário para cada mês.
    -   Identificar e destacar o mês e o dia atual.
    -   Exibir os eventos correspondentes ao dia selecionado.
    -   Gerenciar os dados das sessões e comissões.

## Personalização

Você pode personalizar o calendário editando o arquivo HTML/CSS/JavaScript diretamente:

-   **Eventos**: As constantes `sessoes` e `comissoes` no JavaScript (`<script>`) podem ser atualizadas com novas datas ou tipos de eventos. Certifique-se de manter o formato `"AAAA-MM-DD"`.
-   **Ano do Calendário**: Atualmente, o calendário está fixo para o ano de `2026`. Para adaptá-lo a outros anos, você precisará ajustar a variável `currentYear` dentro da função `showMonth` e, possivelmente, as datas nas constantes `sessoes` e `comissoes`.
-   **Estilos**: Modifique as regras CSS dentro da tag `<style>` para alterar cores, fontes, tamanhos e outros aspectos visuais.
-   **Textos**: Altere os títulos e textos diretamente no HTML.

## Créditos

Desenvolvido por Tiago Treter para a Câmara Municipal de Coronel Barros/RS.