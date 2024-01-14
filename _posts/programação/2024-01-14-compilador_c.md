---
layout: post
permalink: /programacao/compilador-c
author: Rebecca
title: Ajeitando o compilador da linguagem C
---

Está animado para começar a aprender C, mas não sabe por onde baixar o compiler, ou ainda, está com dificuldades para configurar as variáveis de ambiente?

Neste post irei te ajudar com tudo isso, segue com eu <i class="fa-solid fa-turn-down"></i>

## O compilador
Para compilar códigos em C você irá precisar de um compilador de C. Você pode baixá-los tradicionalmente pelos links abaixo, mas ensinarei uma outra maneira que é mais conviniente e sem riscos de ter problemas com o computador.

| Compilador | Descrição |
|:----------:|:------------------------------------------------------------------------:|
| [MinGW-w64](https://www.mingw-w64.org) | O compilador "mãe". Sem sal, nem tempero, mas faz o esperado. |
| [Cygwin](https://cygwin.com) | A opção vegetaria, também funciona bem. |
| [Msys2](https://www.msys2.org) | Versão estendida do MinGW, conta com um gerenciador de pacotes. |
| [tdm-gcc](https://jmeubank.github.io/tdm-gcc/) | Combina o MinGW com alguns patches, geralmente usado com a linguagem [Go](https://go.dev). |
| [MSVC](https://visualstudio.microsoft.com/vs/features/cplusplus/) | Compilador de C/C++ da Microsoft. |

Neste post, irei usar o [scoop.sh](https://scoop.sh) como gerenciador de pacotes para instalar o compilador C.

### Instalando via scoop.sh
_(Recomendo visitar o site para mais detalhes, caso julgue necessário)_

Abra o Powershell apertando a combinação de teclas "Windows" e "X":

![image](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/bce6cb7f-4959-4aea-9d1a-8d28bb8acc43)

Clique em "Windows Powershell".

Cole o seguinte comando no terminal, e de enter: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`, a seguinte mensagem irá aparecer: 

![powershell_Y2Lsl4lBye](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/93f91a32-34b3-49d4-b097-6e289ced0cd3)

Aperte a tecla "S" e depois enter.

Após isso, cole o próximo comando e de enter: `Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression`, está mensagem vai aparecer caso tudo corra bem:

![powershell_bcigs5la5p](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/d211d43d-5b04-403a-bd40-e3b5b5675b0a)

> <i class="fa-solid fa-triangle-exclamation"></i> Se você estiver usando o Windows 7 ou inferior, é necessário [obter um powershell atualizado](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.4#msi).

Com isso, conseguimos instalar o scoop. Agora vamos instalar um compilador!

#### Passo opcional: instale o git
Instalar o Git acelera os downloads e também a extração de arquivos realizados pelo scoop. Você pode instalar usando `scoop install git`, como na imagem abaixo:

![powershell_8U4QHu1N6a](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/f41106c6-6084-44b8-b0a4-2e22a03821ac)

### Instalando o compilador
Com o scoop instalado, você pode usar o seguinte comando para instalar o mingw: `scoop install mingw`, como mostrado abaixo:

![image](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/d2339ac9-d37a-4955-aaca-0707d7feeb70)

Se tentarmos executar o comando `gcc`, veremos que ele está funcionando corretamente, como magica:

![image](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/17a923c5-5576-46c0-beef-d48fb22d8ab3)
![image](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/70839ba8-2363-49be-a0bd-35ea1664c0a0)


Se você so precisa instalar o compilador sem dor de cabeça, você pode parar por aqui. 

### Outros GCCs
Particulamente, gosto de usar o tdm-gcc, por ser mais otimizados que outros compiladores GCC no Windows, e por que eu particulamente programo principalmente na linguagem Go, que pode ter bindings para o C, além de usar linkagem estáticas. [(Leia mais sobre)](https://jmeubank.github.io/tdm-gcc/about/).

Para instalar, você precisar usar dois comandos:

- `scoop bucket add versions` - Adiciona o repositório "versions" ao scoop
![powershell_pBXCu9GhTZ](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/55115cb6-4431-4744-a61a-abe271cc20d6)

- `scoop install versions/tdm-gcc` - Instala o tdm-gcc
![powershell_9pwhcK9cx6](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/c2a90857-2ec0-44b3-b6d0-79b81d22aadf)

Além do tdm, existem [outros mais na lista de aplicativos do scoop](https://scoop.sh/#/apps?q=gcc):

![image](https://github.com/princessmortix/estudos-do-quarto/assets/47502554/515bf8dc-5670-4236-8202-462952719b44)

---
Gostou do post? Deixe um ❤ no blog!
