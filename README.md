# Tabbed Interface usando JavaScript

Este projeto implementa uma interface de abas simples usando HTML e JavaScript puro. Quando o usuário clica em uma aba, o conteúdo correspondente é exibido, enquanto os demais conteúdos são ocultados.

## Estrutura do HTML

O código contém uma estrutura HTML com os seguintes elementos principais:

1. Uma `<div>` com a classe "container", que envolve toda a interface de abas.
2. Dentro do contêiner, há duas seções principais:
   - Uma `<div>` com a classe "tabs_container" contendo as abas individuais (Aba1, Aba2, Aba3, Aba4 e Aba5).
   - Outra `<div>` com a classe "container_contents" contendo o conteúdo correspondente a cada aba (Conteúdo 1, Conteúdo 2, Conteúdo 3, Conteúdo 4 e Conteúdo 5), juntamente com imagens correspondentes.

## Funcionalidade JavaScript

O JavaScript desse projeto realiza o seguinte:

1. Seleciona todos os elementos com a classe "aba" (abas) e "content" (seções de conteúdo) usando `querySelectorAll`.
2. Cria um array vazio chamado `control` para acompanhar as abas selecionadas.

## Event Listeners

O código adiciona um event listener de clique a cada elemento de aba (`.aba`).
Quando uma aba é clicada, o event listener é acionado, e o conteúdo correspondente é exibido, enquanto os demais conteúdos são ocultados.
A aba clicada recebe a classe "selected" para destacar a aba ativa.
A aba previamente selecionada é desativada, removendo a classe "selected".

## Exibição/Ocultação de Conteúdo

As seções de conteúdo são ocultadas por padrão usando a classe "hidden".
O código JavaScript percorre todas as seções de conteúdo (`.content`) e verifica se o texto da aba está incluído no nome da classe da seção de conteúdo.
Se o texto da aba for encontrado no nome da classe de uma seção de conteúdo, essa seção de conteúdo é exibida, removendo a classe "hidden".
Se o texto da aba não for encontrado no nome da classe de uma seção de conteúdo, essa seção de conteúdo é ocultada, adicionando a classe "hidden".

Note que a implementação desse exemplo de interface de abas é bastante simples. Existem soluções mais robustas e escaláveis disponíveis usando bibliotecas como jQuery ou frameworks JavaScript modernos, como React ou Vue.js. No entanto, este código JavaScript puro demonstra o conceito básico de interfaces de abas e como exibir/ocultar conteúdo com base na seleção de abas.
