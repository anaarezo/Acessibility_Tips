# WCAG - Recomendações de Acessibilidade
Dicas de como tornar um site mais acessível à leitores de tela, para ajudar na leitura de pessoas com deficiência visual ou baixa visão.

## 1.1. Idioma do Documento
Sempre declarar o idioma do documento HTML, na tag principal da página `<html>` é necessário inserir a língua desejada de acordo com o país, no qual está sendo desenvolvido o site. Isso é referenciado por meio do atributo `lang` como, por exemplo:

```html
<html lang="en">

...

</html>
```
Outras línguas:

* Português do Brasil: `lang="pt-br"`
* Francês: `lang="fr"`
* Espanhol: `lang="es"`

## 1.2. Heading Tags
### 1.2.1. H1
A utilização do heading tag H1 necesita ser limitado a 1 por página, a existência de mais de um dessa mesma tag traz conflitos para a leitura, direcionamento e entendimento da página, não só para acessibilidade como também para SEO, pois a utilização desta tag consiste em fazer com que o usuário seja direcionado à primeira vista com a página na qual ele se encontra.

```html
<h1>Título Exemplo de H1</h1>
```
### 1.2.2. H1 ao H6
Para que a leitura tenha um seguimento ideal, é necessário que os heading tags estejam ordenados corretamente, isso porque os softwares de leitura de tela trabalham buscando por onde é necessário iniciar a leitura para fazer mais sentido ao contexto do conteúdo como um todo. Logo, em ferramentas de monitoria de código para verificação de acessibilidade, é crucial que os heading tags estejam ordenados corretamente em um bloco. Exemplo:

```html
<div class="wrapper">
    <div class="block">
        <h2>Title</h2>
        <div class="infos">
        <h3>Subtitle</h3>
        <h4>Description</h4>
        </div>
    </div>
</div>
```
## 1.3. Skip Link
Os Skip Links colaboram para a objetividade na leitura de páginas para usuários de leitores de tela. Isso ajuda durante a navegação da página atual, pois são utilizados para ignorar o conteúdo repetitivo da página, fazendo com que os principais pontos da página sejam destacados.
Consiste numa espécie de link que pula o conteúdo do header para o conteúdo principal da página.
Ele é aplicado como no exemplo abaixo:

```html
<a href="#link"> Pule para o conteúdo principal </a>
```

```css
a {
    display: none;
}
```
Desta forma, o Skip Link é ignorado pelo usuário que consegue ver o site, apenas é lido pelos usuários de leitores de tela, que conseguem acessar essa opção por meio do `html`

## 1.4. Outline
Outline é uma propriedade de contorno do CSS, na qual é crucial para a leitura de todas as informações e elementos da página. Esta propriedade exibe bordas por todos os elementos do site enquanto é pressionada a tecla `tab` para navegação, porque quando navegada por via da tecla, faz com que os softwares de leitura reconheçam, campos, botões, palavras, dentre outros elementos com foco.
Caso seja removida essa leitura é perdida, fazendo com que o texto do site ou campos sejam confusos ou não reconhecidos por meio de softwares de leitura.
Uma regra muito importante se quer desenvolver um site acessível é nunca remover o `outline`.

## 1.5. Imagens
A primeira regra para acessibilidade de imagens é nunca remover os atributos `alt` e `title` das imagens, isto, porque com estes atributos é possível inserir textos explicativos para os usuários de leitores de tela, fazendo com que fique claro o que se encontre na imagem, é muito importante ser descritivo e ao mesmo tempo sucinto, para que a pessoa consiga mentalizar o que aparece na imagem.

## 1.6. Roles
```html
<header role="banner"></header>

<nav role="navigation"></nav>

<main id="conteudoPrincipal" role="main"></main>

<form action="search.php" role="search"></form>

<p class="copyright" role="info"></p>

<div class="left-btn" aria-label="Anterior" role="button">🢂</div>
```

## 1.7. Tabindex
(ignorado pelo screen header pelo tabindex -1)
## 1.8. Aria-Label
## 1.9. Ícones
```html
<div class="star" tabindex="-1">😄</div>
```
## 1.10. Formulários

## Referências
* [W3C - Geral](https://www.w3.org/TR/WCAG20/)
* [W3C - Referência Rápida](https://www.w3.org/WAI/WCAG20/quickref/)
* [Nomensa](https://www.nomensa.com/blog/2004/what-are-skip-links)
* [UX - Acessibilidade](https://ux.sapo.pt/acessibilidade/)
* [Accessible Bootstrap Date Picker](http://eureka2.github.io/ab-datepicker/)
* [Felipe Fialho](https://www.felipefialho.com/blog/2016/sobre-wai-aria-acessibilidade-e-semantica)