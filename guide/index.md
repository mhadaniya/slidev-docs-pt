# Começar

## Visão Geral

O **Slidev** <sup>(slide + dev, `/slʌɪdɪv/`)</sup> é uma criador e apresentador de slides baseado em tecnologias web. O **Slidev** foi projetado para que desenvolvedores concentrem-se essencialmente em escrever conteúdo em Markdwon e, ao mesmo tempo, ter a possibilidade de utilizar componentes HTML e Vue para fornecer *layouts* e *designs* perfeitos e demonstrações interativas.

Este usa um arquivo Markdown rico em recursos que permite gerar slides bonitos com *refresh* automático instantâneo, junto com várias integrações possíveis, desde desenvolvimento de código ao vivo, exportação pada PDF, gravação da apresentação, entre outros. Como o **Slidev** tem como por base tecnologias web é possível fazer qualquer coisa, a tua imaginação é o limite.

Para saber mais sobre a lógica por baixo dos panos basta aceder à secção [Why Slidev](/guide/why).


### Funcionalidades

- 📝 [**Baseado em Markdown**](/guide/syntax.html) - usa os teus editores favoritos e melhora o teu workflow
- 🧑‍💻 [**Amigo dos Desenvolvedores**](/guide/syntax.html#code-blocks) - com desenvolvimento de código ao vivo, destaque de sintaxe, etc.
- 🎨 [**Possibilidade de usar temas**](/themes/gallery.html) - tema pode ser partilhado e utilizado através de packages npm
- 🌈 [**Estiloso**](/guide/syntax.html#embedded-styles) - [Windi CSS](https://windicss.org/) estilos CSS incorporados e de fácil utilização, bem como diversas ferramentas
- 🤹 [**Interativo**](/custom/directory-structure.html#components) - incorporação de componentes Vue com facilidade e sem problemas
- 🎙 [**Modo Apresentador**](/guide/presenter-mode.html) - use outra janela, ou até mesmo um smartphone para controlar a tua apresentação
- 🧮 [**LaTeX**](/guide/syntax.html#latex) - Conta com suporte integrado para equações matemáticas utilizando Latex
- 📰 [**Diagramas**](/guide/syntax.html#diagrams) - Criação de diagramas com descrições textuais
- 🌟 [**Ícones**](/guide/syntax.html#icons) - Acessa qualquer ícone de qualquer conjunto de ícones diretamente
- 💻 [**Editores**](/guide/editors.html) - Editor integrado, ou [extensão para o VS Code](https://github.com/slidevjs/slidev-vscode)
- 🎥 [**Gravação**](/guide/recording.html) - funcionalidade incluída para a gravação da apresentação bem como visão da tua câmera
- 📤 [**Portátil**](/guide/exporting.html) - exporta para PDF, PNGs, ou hospeda online uma SPA
- ⚡️ [**Rápido**](https://vitejs.dev) - referesh automático instantâneo fornecido por [Vite](https://vitejs.dev)
- 🛠 [**Hackeavel**](/custom/config-vite.html) - usa plugins Vite, componentes Vue, ou qualquer package npm

### Stack Tecnológica

O **Slidev** é possível através da combinação das seguintes ferramentas e tecnologias.

- [Vite](https://vitejs.dev) - Uma ferramenta de *front-end* extremamente rápida
- [Vue 3](https://v3.vuejs.org/) com [Markdown](https://daringfireball.net/projects/markdown/syntax) - Foco no conteúdo, tendo ainda a possibilidade de utilizar componentes HTML e componentes Vue sempre que necessário
- [Windi CSS](https://github.com/windicss/windicss) - framework CSS super útil, que permite dar estilo aos teus slides facilmente
- [Prism](https://github.com/PrismJS/prism), [Shiki](https://github.com/shikijs/shiki), [Monaco Editor](https://github.com/Microsoft/monaco-editor) - Suporte a *snippets* de código, bem como a possibilidade de desenvolver código ao vivo
- [RecordRTC](https://recordrtc.org) - Gravação integrada e visualização da tua câmera
- Família [VueUse](https://vueuse.org) -  [`@vueuse/core`](https://github.com/vueuse/vueuse), [`@vueuse/head`](https://github.com/vueuse/head), [`@vueuse/motion`](https://github.com/vueuse/motion), etc.
- [Iconify](https://iconify.design/) - coleções de ícones.
- [KaTeX](https://katex.org/) - renderização de equações matemáticas em LaTeX.
- [Mermaid](https://mermaid-js.github.io/mermaid) - Diagramas textuais.

### Começa a tua primeira apresentação

Com NPM:

```bash
$ npm init slidev
```

Com Yarn:

```bash
$ yarn create slidev
```

Segue as instruções e começa a fazer os teus slides agora! Para mais detalhes sobre a sintaxe em markdown, lê o [guia de sintaxe](/guide/syntex)

### Linha de Comandos

Num projeto onde o **Slidev** está instalado, podes utilizar o binário `slidev` nos teus *scripts* npm.


```json
{
  "scripts": {
    "dev": "slidev", // iniciar servidor de desenvolvimento
    "build": "slidev build", // build do projeto para produção
    "export": "slidev export" // exportção para PDF
  }
}
```

Ou então, podes também usar com o [`npx`](https://www.npmjs.com/package/npx)

```bash
$ npx slidev
```

Executa o comando `slidev --help` para saberes todas as opções disponíveis.

### Sintaxe Markdown

O **Slidev** lê o teu ficheiro `slides.md` na raiz do teu projeto e converte em slides. Sempre que realizares alguma alteração, o conteúdo dos slides será atualizado de forma automática. Por exemplo:

~~~md
# Slidev

Olá Mundo

---

# Página 2

Uso directo de blocos de código com highlight da sintaxe

//```ts
console.log('Olá, Mundo!')
//```

---

# Página 3
~~~

Sabe mais sobre a sintaxe Markdown utilizada no [guia de sintaxe](/guide/syntax).