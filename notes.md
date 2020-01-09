## Folders structure

Resources: Contains code made by myself.

Vendors: contain

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
[x] Make a "zoom-in" transition, only using CSS (Use transform with scale(), and transition properties)
[x] A way to make img elements darker

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

## Section 3: Build how it works section (class="section-steps")

[x] Draw circles with CSS
[x] A technique to make separation between containers
[x] How to incorporate App Store and Play Store buttons

<!--
Section 3: How it works
Title:How it works - Simple as 1, 2, 3
1.Choose the subscription plan that best fits your needs and sign up today.
2.Order your delicious meal using our mobile app or website. Or you can even call us!
3.Enjoy your meal after less than 20 minutes. See you the next time!
 -->

## Section 4: Build cities section (class="section-cities")

Key tasks:
[x] How to use small icons aligned with some text
[x] How o style generic links

<!--
Section 4: Cities
Title: We're currently in these cities

Lisbon
1600+ happy eaters
60+ top chefs
@omnifood_lx

San Francisco
3700+ happy eaters
160+ top chefs
@omnifood_sf

Berlin
2300+ happy eaters
110+ top chefs
@omnifood_berlin

London
1200+ happy eaters
50+ top chefs
@omnifood_london

 -->

## Section 5: Build customer testimonials section (class="section-testimonials")

Key tasks:
[x] How to create a beautiful background-image effect
[x] How to effectively communicate what customers have to say

<!--

Section 5: Customer testimonials
Title:Our customers can't live without us

Omnifood is just awesome! I just launched a startup which leaves me with no time for cooking, so Omnifood is a life-saver. Now that I got used to it, I couldn't live without my daily meals!
(Alberto Duncan)

Inexpensive, healthy and great-tasting meals, delivered right to my home. We have lots of food delivery here in Lisbon, but no one comes even close to Omifood. Me and my family are so in love!
(Joana Silva)

I was looking for a quick and easy food delivery service in San Franciso. I tried a lot of them and ended up with Omnifood. Best food delivery service in the Bay Area. Keep up the great work!
(Milton Chapman)

 -->

## Section 6: Sign up and pricing plans (class="section-plans")

 <!-- 
 Section 6: Sign up and pricing plans
 Title: Start eating healthy today
 
 Plan 1: Premium
 399$ per month
 That’s only 13.30$ per meal
 1 meal every day
 Order 24/7
 Access to newest creations
 Free delivery
 
 Plan 2: Pro
 149$ per month
 That’s only 14.90$ per meal
 1 meal 10 days/month
 Order 24/7
 Access to newest creations
 Free delivery
 
 Plan 3: Starter
 19$ per meal
 1 meal
 Order from 8 am to 12 pm
 Free delivery

  -->

## Section 7: Contact form (class="section-form")

Key concepts and tasks:
[x] How to use a set of HTML elements to create forms: form, label, input, select, option, textarea
[x] How to style these elements

<!--
Title: We're happy to hear from you

Fields to include:
Name
Email
How did you find us?
Newsletter
Drop us a line
 -->

## Section 8: Footer (class="footer")

<!--
Title: None

Navigation:
1. About us
2. Blog
3. Press
4. iOS App
5. Android App

Also include links to facebook, twitter, google+ and Instagram accounts.
 -->

---

## Responsive web design with media queries

**RESPONSIBLE LAYOUT**

- 0 <= screen size <=480px: Phone
- 480 < screen size < 768px: Tablet portrait
- 768 <= screen size < 1024px: Tablet landscape
- 1024 <= screen size < 1200px: Desktop
- 1200px+: Big desktop

OR

- 0 - 600px: Phone
- 600 - 900px: Tablet portrait
- 900 - 1200px: Tablet landscape
- 1200 - 1800px: is where our normal styles apply
- 1800px+: Big desktop

Breakpoint argument names:

- phone
- tab-port
- tab-land
- desktop
- big-desktop

Use em instead of rem because media queries responds better with em.
1em = 16px

ORDER to do media queries: base + typography > general layout + grid > page layout > components

### Steps to define media queries:

- Define screen size breakpoints;
- Create a CSS file to define the media queires;
- Import the media queries CSS file in the page and add the meta tag (`<meta name="viewport" content="width=device-width, initial-scale=1.0" />`)

### CSS Browser prefixes

Allow CSS3 features to work between browsers, use autoprefixer plugin to automagically apply it.

**To enable features in older browsers** - will be used 03 scripts:

- respond.js: enables browsers to understand and execute css media queries;
- html5shiv: enable to use and style HTML5 elements in older browsers;
- selectivizr: utility that emulates CSS3 pseudo-classes and attribute selectors in Internet Explorer 6-8.

### jQuery

**Plugins used:**

- Waypoints: jQuery plugin to trigger a function when you scroll to an element.

**Scroll to elements:**

- Scroll animation added to the header and navigator buttons.

**Animate.css**: For ready to use CSS animations.

## Step 5: Enhancing page speed

1 - Optimize heavy images;
2 - Minify CSS and jQuery code.

### Basic Search Engine Optimization (SEO)

- Use metatags;
- Check if the HTML code produced is valid;
- Add keywords: in the title, meta description tag, headings and links.
- Backlinks: Try to make other websites have links to your site.

# Steps to launch the website

1 - Chose and buy a domain name;
2 - Buy web hosting;
3 - Upload the website.
