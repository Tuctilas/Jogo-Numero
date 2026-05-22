# 🎲 Amigo Secreto

Aplicação web para organizar sorteios de amigo secreto com visual futurista. Adicione os participantes, realize o sorteio e descubra quem tirou quem — tudo com uma interface estilo HUD cyberpunk.

---

## Funcionalidades

- Adicionar participantes à lista
- Remover participantes clicando no nome
- Sortear os pares automaticamente (mínimo de 3 pessoas)
- Reiniciar o sorteio a qualquer momento
- Dado 3D animado e interativo como elemento visual

---

## Tecnologias utilizadas

- **HTML5**
- **CSS3** — animações 3D, `clip-path`, `transform-style: preserve-3d`
- **JavaScript** — manipulação do DOM, algoritmo de embaralhamento Fisher-Yates
- **Google Fonts** — Chakra Petch, Inter, Share Tech Mono

---

## Estrutura do projeto

```
amigo-secreto/
├── index.html
├── style.css
├── js/
│   └── app.js
└── assets/
```

---

## Como usar

1. Clone ou baixe o repositório
2. Abra o arquivo `index.html` no navegador
3. Digite o nome de um participante e clique em **Adicionar**
4. Repita até ter pelo menos 3 participantes
5. Clique em **Sortear** para revelar os pares
6. Clique em um nome na lista para removê-lo
7. Clique em **Reiniciar** para começar do zero

> Clique no dado 3D para rolá-lo — ele gira e para em uma face aleatória.

---

## Lógica do sorteio

O sorteio utiliza o algoritmo **Fisher-Yates** para embaralhar a lista de participantes de forma aleatória e imparcial. Cada pessoa sorteia o próximo da fila, e o último sorteia o primeiro, formando um ciclo fechado.

```
Alice  -->  Carlos
Carlos -->  Beatriz
Beatriz --> Alice
```

---

## Validações

| Situação | Comportamento |
|---|---|
| Campo vazio | Alerta pedindo o nome |
| Nome duplicado | Alerta informando que já está na lista |
| Menos de 3 participantes | Alerta pedindo mais participantes |

---


## Autor

Desenvolvido por **Gustavo Macedo** como projeto de prática de HTML, CSS e JavaScript.
