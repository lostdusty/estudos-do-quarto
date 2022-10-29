---
layout: post
permalink: /matematica/poliedros-prismas
title: "Poliedros e Primas"
author: Rebecca
---

# Poliedros

## O que são poliedros?

Poliedro é todo sólido geométrico que são formados por superfícies planas, e cada uma dessas superfícies chamamos de **faces**, e cada uma dessas faces é um polígono.

## Vertice, Aresta e Faces

Todos os poliedros possuem Vertices (V), Arestas (A) e Faces (F).  
As verticies são os segmentos de reta que une duas arestas (as "linhas" dos poligonos), já as arestas são pontos que unem no minimo duas arestas (a "ponta" da figura). As faces, como explicado anteriormente, são as superficies dos poligonos.  
Veja a imagem a seguir:

![image](https://user-images.githubusercontent.com/47502554/173704551-46d849db-c09a-400f-8978-99a2072cbaa8.png)

## Poliedros convexos e não convexos

Poliedros convexos são poliedros que qualquer segmento que una dois pontos **não irá sair do poliedro**, ja nos não convexos (ou côncavos), é possível unir um par de pontos passando por fora dele.

![image](https://user-images.githubusercontent.com/47502554/173704847-7cf2802d-7c23-4ca6-9e30-0ce5fd2e76da.png)

# Relação de Euler

A formula $V + F = A + 2$ associa o número de vértices (V), faces (F) e arestas (A) de um poliedro.

> A relação é sempre valida para poliedros convexos. No caso de poliedros não convexos, essa relação _pode_ ser válida ou não.

## Aplicando a relação

Digamos que você saiba apenas quantas faces e arestas tem um prisma de base triangular, é possível saber quantas arestas e vertices esse cubo tem sem precisar contar, veja o exemplo:

$$V + F = A + 2$$

$$4 + 4 = A + 2$$

$$A + 2 = 8$$

$$A = 8 - 2$$

$$A = 6$$

Este poligono tem 6 arestas, como foi calculado na formula.

# Soma dos angulos internos

Para calcular a soma dos angulos internos, é necessário que saiba quantas vertices tem esse poligono.

A formula para calcular é a seguinte:

$${\color{red}180} (N{\color{red}-2})$$

Sendo N a única parte que muda na formula, sendo o número de vertices.

## Exemplos

### Triangulo

Todos os triangulos tem 3 vertices, logo:

$${\color{red}180} (N{\color{red}-2})$$

$${\color{red}180} (3{\color{red}-2})$$

$$180 * (1)$$

$$180$$

### Quadrado

Um quadrado tem 4 vertices, portanto:

$${\color{red}180} (N{\color{red}-2})$$

$${\color{red}180} (4{\color{red}-2})$$

$$180 * (2)$$

$$360$$

### Cubo

É um poliedro com 6 faces quadrangulares:

Usaremos a seguinte relação para saber o numero de arestas: $2A = nF_{N + 2}$, sendo N o número de vertices desse poligono
$$2A = 4 * 6$$

$$2A = 24$$

$$A = \frac{24}{2}$$

$$A = 12$$

E então, usaremos a relação de Euler para descobrirmos quantas vertices:

$$V + F = A + 2$$

$$V + 6 = 12 + 2$$

$$V + 6 = 14$$

$$V = 14 - 6$$

$$V = 8$$

E finalmente:

> Note que podemos fazer que $S_{f} = 360(V-2)$

$${\color{red}360} (V{\color{red}-2})$$

$${\color{red}180} (8{\color{red}-2})$$

$$180 * (6)$$

$$2160$$

# Poliedros regulares (Poliedros de Platão)

Um poliedro regular é quando todos as suas faces são congruentes a um unico poligono regular e em cada vertice ocorre o mesmo número de arestas.

> **ATENÇÃO:** Se um poliedro satisfaz apenas uma dessas condições, ele não é um poliedro regular.

Embora exista uma infinidade de poliedros convexos, apenas 5 são regulares (ou de Platão), e eles são:

- Tetraedro regular: 4 faces triangulares
- Hexaedro regular: 6 faces quadrangulares
- Octaedro regular: 8 faces triangulares
- Dodecaedro regular: 12 faces pentagonais
- Icosaedro regular: 20 faces triangulares

## Tetraedro

### Arestas

$$F_{3} = 4$$

> $2A = 3 * {\color{blue}F_{3} \leftarrow}$ faces triangulares

$$2A = 3 * 4$$

$$2A = 12$$

$$A = 6$$

### Vertices

$$V + F = A + 2$$

$$V + 4 = 8$$

$$V = 4$$

## Hexaedro

### Arestas

$$F_{4} = 6$$

> $2A = 4 * {\color{blue}F_{4}}$

$$2A = 4 * 6$$

$$2A = 24$$

$$A = 12$$

### Vertices

$$V + F = A + 2$$

$$V + 6 = 14$$

$$V = 8$$

## Octaedro

### Arestas

$$F_{3} = 8$$

> $2A = 3 * {\color{blue}F_{3}}$

$$2A = 3 * 8$$

$$2A = 24$$

$$A = 12$$

### Vertices

$$V + F = A + 2$$

$$V + 8 = 14$$

$$V = 5$$

## Dodecaedro

### Arestas

$$F_{5} = 12$$

> $2A = 5 * {\color{blue}F_{5}}$

$$2A = 5 * 12$$

$$2A = 60$$

$$A = 30$$

### Vertices

$$V + F = A + 2$$

$$V + 12 = 32$$

$$V = 20$$

## Icosaedro

### Arestas

$$F_{3} = 20$$

> $2A = 3 * {\color{blue}F_{3}}$

$$2A = 60$$

$$A = 30$$

### Vertices

$$V + F = A + 2$$

$$V + 20 = 32$$

$$V = 12$$

# Prismas

O conteúdo de prismas está disponível em .pdf

[<i class="fa-solid fa-file-pdf"></i> baixar conteúdo](https://github.com/princessmortix/estudos-do-quarto/files/8904826/bb818a7b-e01f-4e50-9ced-bb09629f97de.pdf)

## Volume de prismas

[<i class="fa-solid fa-file-pdf"></i> baixar conteúdo](https://github.com/princessmortix/estudos-do-quarto/files/8904828/a686428c-96a7-45a9-ac57-3fb6267b0628.pdf)

# Formulas

Veja a imagem anexada abaixo com as fórmulas de alguns poligonos. Os arquivos acima contém as fórmulas dos polígonos.

![img](https://media.discordapp.net/attachments/852886295679860776/1013559461174054923/IMG_20220825_110637.jpg)
