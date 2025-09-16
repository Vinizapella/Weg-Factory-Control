# 🚀 Desafio Programação – WEG Factory Control

## 📖 Contexto

A WEG precisa simular uma linha de produção de motores elétricos, onde cada linha de produção funciona em paralelo (através de uma `thread`).

Cada linha vai produzir um certo número de motores, e cada motor terá um código e um status. O sistema deve registrar a produção em um `Map`, com a seguinte estrutura:

-   **Chave:** Código do motor (`String` ou `Integer`)
-   **Valor:** Status (`“Produzido”`, `“Em teste”`, `“Reprovado”`)

## 🎯 Objetivo

-   Criar `threads` que simulam as linhas de produção.
-   Cada `thread` deve inserir os dados dos motores em um `Map` (ex: `HashMap`).
-   Ao final, o programa deve listar todo o estoque de motores com seus códigos e status.

## 💡 Possíveis Variações

-   Cada motor pode ter um status aleatório: “Produzido”, “Em teste”, “Reprovado”.
-   Usar `ConcurrentHashMap` para evitar problemas de concorrência.
-   Criar 3 ou mais `threads` representando setores diferentes (Produção, Teste, Embalagem).
-   Adicionar `LocalDateTime` para registrar quando cada motor foi produzido.
