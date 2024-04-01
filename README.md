<p align="center">
  <a href="https://devsuperior.com.br">
    <img src="https://github.com/BrunoBuilder/customer_crud_challenge/assets/84381502/6b8cb2ad-5e4b-450b-a788-cd6c2d43a3c3" alt="DevSuperior Logo">
  </a>
</p>

<h1 align="center">Formação Desenvolvedor Moderno</h1>

<h2 align="center">Módulo: Front End</h2>

<h3 align="center">Capítulo: Eventos e estado global</h3>

### DESAFIO: DSFilter

Forma de entrega: link do projeto no seu Github

Você deverá entregar um projeto ReactJS conforme design Figma e caso de uso abaixo. Veja o vídeo
explicativo para mais detalhes sobre o que deve ser feito.

https://www.figma.com/file/s21JDtjv3cRyUfetFYAzIJ/DSFilter

Você deve usar o script abaixo para implementar a base de dados de produtos, bem como a função que busca
os produtos por preço:

https://gist.github.com/acenelio/fa7d03cb660b35cd9986623f1f07aeb3

Caso de uso: listar produtos
 
  1. [OUT] O sistema informa nome e preço de todos produtos, ordenados por preço.
  2. [IN] O usuário informa, opcionalmente, preço mínimo e preço máximo dos produtos
  3. [OUT] O sistema informa nome e preço dos produtos, ordenados por preço, conforme critérios

Informações complementares:
 
  - Não precisa fazer validação de formulário (assuma que o usuário vai digitar valores válidos).
  - Não precisa implementar rotas (pode montar a tela toda no App)
  - Se o valor do preço mínimo não for informado, usar por padrão o valor 0 (zero).
  - Se o valor do preço máximo não for informado, usar por padrão o valor Number.MAX_VALUE

O corpo da tela deve ser um componente (na imagem abaixo: ListingBody) que possui dois filhos: o card de
filtro, e o card de listagem. Você DEVE implementar um evento para fazer o componente de filtro notificar os
parâmetros de filtragem dos produtos:

<p align="center">
  <img src="https://github.com/BrunoBuilder/dsfilter/assets/84381502/441b66e1-bdbb-45bc-b68b-c68d6f559225">
</p>

Critérios de correção
Todos critérios a seguir devem ser contemplados:

1) O projeto deve conter os componentes principais (pode haver outros conforme você quiser):
  
    - Cabeçalho
  
    - Corpo da tela de listagem
 
    - Card de filtro
  
    - Card de listagem

2) A lista de produtos deve ser passada como Prop para o card de listagem.

3) O card de filtro deve emitir um evento onFilter(min, max). Este evento serve para comunicar os preços mínimo
e máximo sempre que o formulário for submetido.

4) Context API utilizada para manter o estado global do número de produtos mostrados na tela. Sempre que
for feita uma nova filtragem e o número de produtos listados mudar, o número deve ser atualizado no cabeçalho.


