Resources: Contains code made by myself.
Vendors: contain

## Tips

RESPONSIBLE LAYOUT
0 - 600px:      Phone
600 - 900px:    Tablet portrait
900 - 1200px:   Tablet landscape
[1200 - 1800]:  is where our normal styles apply
1800px +:       Big desktop    
*/
/* $breakpoint argument choices:
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
    
-----------------------------------------------------

## Setup fluid grid for responsive webdesign
  
- Three ingredients to responsive design:
  1. **Fluid grid**: All layout elements are sized in relative units, such as percentages, instead of absolute units like pixels;
  2. **Flexible images**: are also sized in relative units;
  3. **Media queries**: Allow to specify different CSS style rules for different browser widths.