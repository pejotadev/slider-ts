# Slider-TS

## Descrição
Slider-TS é um projeto de slide dinâmico e responsivo desenvolvido com TypeScript. Este projeto oferece uma experiência suave e personalizável para apresentações de slides.

## Demonstração
Confira o projeto em ação: [Slider-TS na Vercel](https://slider-ts-five.vercel.app/)

## Funcionalidades
- Navegação entre slides com suporte a gestos de toque e cliques.
- Configuração de tempo de transição entre slides.
- Suporte para slides infinitos.
- Personalização de animações e efeitos de transição.
- Responsividade para adaptação em diferentes tamanhos de tela.
- Aceita 

## Tecnologias Utilizadas
- TypeScript
- CSS

## Instalação e Uso 1
1. Clone o repositório: `git clone https://github.com/pejotadev/slider-ts.git`
2. Entre no diretório do projeto: `cd slider-ts`
3. Instale as dependências: `npm install` ou `yarn`
4. Execute o projeto: `npm start` ou `yarn start`
5. Acesse `http://localhost:3000` em seu navegador.

## Uso da classe Slide

```html
<div id="slide">
    <div id="slide-elements">
      <img src="./assets/imagem_1.jpg" alt="Lobo">
      <img src="./assets/imagem_2.jpg" alt="Lobo">
      <img src="./assets/imagem_3.jpg" alt="Lobo">
      <video playsinline src="./assets/video.mp4"></video>
    </div>
    <div id="slide-controls"></div>
  </div>
```

```typescript
import Slide from "./Slide.js";

const container = document.getElementById("slide");
const elements = document.getElementById("slide-elements");
const controls = document.getElementById("slide-controls");

if (container && elements && controls && elements.children.length) {
  const slide = new Slide(
    container, // Container Element to show slides
    Array.from(elements.children), // Slides elements
    controls, // Controls block element
    3000 // Time to change slide
  );
}
```
```
    container: Element;
    slides: Element[];
    controls: Element;
    time: number = 5000;
```

## Como Contribuir
Contribuições são sempre bem-vindas! Para contribuir, por favor, faça um fork do repositório, crie uma branch para sua feature ou correção, faça os commits e abra um Pull Request.

