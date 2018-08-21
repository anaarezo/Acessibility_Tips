# WCAG - Recomendações de Acessibilidade
Como tornar um site mais acessível?

## 1.1. Idioma do Documento
Sempre declarar o idioma do documento HTML, na tag principal da página <html> é necessário inserir a língua desejada de acordo com o país, no qual está sendo desenvolvido o site. Isso é referenciado por meio do atributo “lang” como, por exemplo:

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
## 1.4. Outline
## 1.5. Imagens
## 1.6. Roles
## 1.7. Tabindex
## 1.8. Aria-Label
## 1.9. Ícones
## 1.10. Formulários