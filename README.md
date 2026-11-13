# API Books

Catálogo estático de livros sobre desenvolvimento web, front-end, design e acessibilidade. Os dados ficam em `livros.json` e cada item contém identificador, título, resumo e endereço da capa.

## Conteúdo

- `livros.json`: coleção de livros em formato JSON.
- `imgs/`: capas utilizadas pelo catálogo.
- `img_low/`: imagens de apoio usadas em materiais e exemplos de integração.

## Como consumir

Não há servidor ou etapa de instalação. O JSON pode ser acessado diretamente pelo endereço:

`https://raw.githubusercontent.com/ProfLucasSousa/api-books/main/livros.json`

Exemplo com JavaScript:

```js
const response = await fetch(
  "https://raw.githubusercontent.com/ProfLucasSousa/api-books/main/livros.json"
);
const livros = await response.json();

console.log(livros);
```

## Estrutura de um item

```json
{
  "id": 1,
  "imagem": "URL da capa",
  "titulo": "Título do livro",
  "resumo": "Descrição curta"
}
```

Este repositório funciona como uma API mockada para aulas, protótipos e exercícios de consumo de dados.
