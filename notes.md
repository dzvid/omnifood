Resources: Contains code made by myself.
Vendors: contain

## Tips

RESPONSIBLE LAYOUT
0 - 600px: Phone
600 - 900px: Tablet portrait
900 - 1200px: Tablet landscape
[1200 - 1800]: is where our normal styles apply
1800px +: Big desktop  
_/
/_ \$breakpoint argument choices:

- phone
- tab-port
- tab-land
- big-desktop

Use em instead of rem because media queries responds better with em.
1em = 16px

ORDER to do media queries: base + typography > general layout + grid > page layout > components

## Prepare environment: First development steps

- Setup Normalize.css: Makes the browsers render all elements more consistently.
  - o CSS Reset tem como objetivo reduzir as inconsistências de browser para browser em pontos como margins, line-height, tamanhos dos headings e assim por diante (esses valores variam de browser para browser, o que pode vir a quebrar seu layout). Dito isso, o CSS Reset nos garante que partiremos de um ponto em comum independente de qual browser nosso cliente pode estar utilizando.
  - **O CSS Reset por se tratar de uma folha de estilo independente, deve ser carregado antes de qualquer estilo aplicado no seu site**, e isso pode sim acarretar uma queda de performance, mas ao meu ver, observando os prós e os contras, geralmente vale a pena.
- Set font: get Lato font from google fonts;
- Basic css:

```css
* {
  /*Remove margin and padding from all elements and sets box-sizing*/
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  background-color: #fff;

  color: #555;
  font-family: "Lato", "Arial", sans-serif;
  font-size: 20px;
  font-weight: 300;
  text-rendering: optimizeLegibility;
}
```

---

## Setup fluid grid for responsive webdesign

- Three ingredients to responsive design:
  1. **Fluid grid**: All layout elements are sized in relative units, such as percentages, instead of absolute units like pixels;
  2. **Flexible images**: are also sized in relative units;
  3. **Media queries**: Allow to specify different CSS style rules for different browser widths.

---

## Build header

### Part I

Key tasks:
[x] New HTML elements: header, nav, ul, li;
[x] Put text on a image;
[x] Make image darker (Use a linear gradient on top of the image);
[x] Make a image as big as the browser viewport (Set height to 100vh);
[x] Make a vertically/horizontally centered box(center the content using top and left positioning, then use transform -50% for (x,y));

### Part II

[x] How to design buttons;
[x] The 4 link states in CSS: link, visited, hover, active (Use pseudo classes to set the desired behavior);
[x] CSS3 transitions for small animations;

### Part III

[x] Add site logo;
[x] How to create a simple navigation.

---

## Section 1: Build features section (class="section-features")

[x] Use the fluid grid for the first time (Make a div for each column)
[x] Learn how to use icons
[x] How to put content on a website directly from CSS with the :after pseudo-class

<!-- Section 1: Features
Title: Get food fast — not fast food.

Hello, we’re Omnifood, your new premium food delivery service. We know you’re always busy. No time for cooking. So let us take care of that, we’re really good at it, we promise!

Up to 365 days/year
Never cook again! We really mean that. Our subscription plans include up to 365 days/year coverage. You can also choose to order more flexibly if that's your style.

Ready in 20 minutes
You're only twenty minutes away from your delicious and super healthy meals delivered right to your home. We work with the best chefs in each town to ensure that you're 100% happy.

100% organic
All our vegetables are fresh, organic and local. Animals are raised without added hormones or antibiotics. Good for your health, the environment, and it also tastes better!

Order anything
We don't limit your creativity, which means you can order whatever you feel like. You can also choose from our menu containing over 100 delicious meals. It's up to you! -->

## Section 2: Build favorite meal section (class="section-meals")

[x] Make a grid with images
[] Make a "zoom-in" transition, only using CSS
[] A way to make img elements darker

<!--
Section 2:Favorite meals
Title: None
1.Korean bibimbapwith egg and vegetables
2.Simple italian pizza with cherry tomatoes
3.Chicken breast steak with vegetables
4.Autumn pumpkin soup
5.Paleo beef steak with vegetables
6.Healthy baguette with egg and vegetables
7.Burger with cheddar and bacon
8.Granola with cherries and strawberries
 -->
