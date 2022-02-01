# EQI Simulador de Investimentos API
Este repositório contém uma simples API para o desafio de front-end da EQI Investimentos.

Requisitos:
* NodeJS
* NPM

## Como executar
Faça o clone/download deste repositório, execute `npm install` e `npx json-server db.json`. A API fica localizada em `http://localhost:3000`.

## Rotas
Todas as requisições de POST para esta API devem conter o header `Content-Type: application/json`.
Esta API contém as seguintes rotas:

* `GET /indicadores` : lista de todos os indicadores
* `GET /simulacoes` : lista de todas as simulações possíveis

Para efetuar os filtros em `GET /indicadores`, é possível:
* fazer uma busca global utilizando a query string `?q=:busca`;
* fazer uma busca por campo individual utilizando a query string `?nome=:busca`.

Para efetuar os filtros em `GET /simulacoes`, é possível:
* fazer uma busca global utilizando a query string `?q=:busca`;
* fazer uma busca por campo individual utilizando a query string `?tipoIndexacao=:busca&tipoRendimento=:busca`.
