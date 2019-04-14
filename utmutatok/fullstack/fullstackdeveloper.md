# Fullstack (web) developer, 2019

## Egy falatnyi történelem 

A webes, illetve a webes alkalmazásfejlesztés hatalmasat fejlődött az elmúlt akár 5 évben, sőt, mióta léteznek modern webalkalmazásokhoz használatos framework-ök, komoly változás következik be akár minden hatodik hónapban. Ilyenkor természetesen, illetve jobb esetben, a fejlesztőre van bízva, hogy ezeket mennyire, és milyen intenzitással hajlandó követni. 

## Mi az a fullstack fejlesztő? 

A fullstack fejlesztő az alkalmazás összes rétegét és annak összes stackjét ismeri: 

- Szerver, hálózat, és hosting ismerete
- alkalmazás skálázhatóságának ismerete 
- cloud storage ismerete
- adat redundancia 
- adat modellek ismerete
- relációs, nem relációs adatbázisok ismerete
- üzleti logika ismerete
- API réteg ismerete
- MVC pattern ismerete 
- clean code alkalmazása 
- user interface átfogó ismerete 
- modern frameworkok ismerete 
- user experience 
- tisztában lenni a végfelhasználó igényeivel

## Alapok

### HTML

A `HTML` (azaz `HyperText Markup Language`) az alapja minden weboldalnak, vagy webalkalmazásnak. A `HTML` határozza meg a weboldal (vagy webapp) szerkezetét, struktúráját, és a tartalmát. 

A `HTML` fájl `tag`-ekből áll, aminek alapvetően két típusát különböztetjük meg:

1. Önzáró tagek (_self-closing_)

Pl.:
```
<img src="./images/logo.png" alt="logo" />
```

2. Nem önzáró tagek (_non self-closing_)

```
<span>hello worlds</span>
```

A `HTML` tageket _tulajdonságokkal_ (más néven attribútumokkal) tudjuk ellátni. A fenti példában, az `img` tag-nak az `src` (azaz _source_, forrás) egy attribútuma, ami meghatározza a fájl nevét, és a hozzá vezető útvonalat. 

Vannak alapvető szabályok, amiket be kell tartani `HTML` írása közben, ilyen például az a szabyályrendszer ami leírja, hogy adott elemnek milyen _leszármazottjai_ lehetnek.

Például: 

_helytelen_: 

```
<a href="demo.html">
    <label>lorem</label>
</a>
```

Ugyanis az `a` tag nem tartalmazhat `label` taget. Az ilyen, és ehhez hasonló hibák kijavítására való a [`w3c validator`](https://validator.w3.org/).  

Az összes `HTML` tag-ről elérhető egy teljes lista [itt](https://www.tutorialrepublic.com/html-reference/html5-tags.php)

### CSS
A `CSS` (azaz `Cascading Style Sheets`) egy egyszerű módszer arra, hogy _stílusokat_ adjunk az oldalainkoz, amikkel definiáljuk, hogy mi hogyan nézzen ki. 

A stíluslapokon stílusmegadásokkal (stílusdefiníciókkal) formázhatjuk meg a kívánt oldalelemeket: a böngésző az itt megadott definíciók alapján fogja megjeleníteni az oldalt. A böngészők nem teljesen kompatibilisek egymással a stíluslapok használatát illetően, ezért teszteljük oldalainkat a több böngészőben, ha lehetséges, illetve a 4-esnél kisebb verziójú böngészőkben is.

A `CSS` definíciókat `.css` fájlokban tároljuk, amit aztán hozzá kell adnunk a `.html` oldalainkhoz. 

`<link rel="stylesheet" type="text/css" href="style.css">`

#### Stílus szabályok
 
 > öröklödés, szelektorok, osztályok, stb. 

 A stílusok öröklődhetnek, és a tagen belüli stílusdefiníciókkal felülírhatjuk a globális stílusmegadásokat. Ez azt is jelenti, hogyha egy tag-hez tartozik globális és lokális stílusmegadás is egy adott tulajdonságra, akkor a lokálisan megadott érték felülírja a globálisan megadottat az adott helyen. (Általában a később megadott, tehát a dokumentumban lejjebb található stílusmegadás érvényesül.) De ha a stílusmegadás végén az !important kulcsszót is elhelyezzük, biztos, hogy az ott megadott stílus fog megjelenni, nem lehet lokálisan felüldefiniálni azt.

 ```
 body {
     color: #000;
 }
 ```

 A `html` tageket ún. osztályokkal láthatjuk el, amikkel aztán hivatkozhatunk rájuk a `css` fájlokban. 

`html`:

 ```
 <p> class="text">
 hello world
 </p>
 ```

`css`: 

```
.text { border: 1px solid #000; }
```

* [`html`](https://www.w3schools.com/html/)
* [`css`](https://www.w3schools.com/css/)
* [`javascript`](https://developer.mozilla.org/hu/docs/Web/JavaScript)

## CSS 

### Preprocesszor

* [`dart-sass`](https://github.com/sass/dart-sass)
* [`less`](https://github.com/less/less.js)
* [`stylus`](https://github.com/stylus/stylus)
* [`post-css`](https://github.com/postcss/postcss)
* [`css-in-js`](https://github.com/cssinjs/jss)
* [`emotion`](https://github.com/emotion-js/emotion)

### CSS framework

* [`bulma`](https://github.com/jgthms/bulma)
* [`foundation`](`https://github.com/zurb/foundation-sites)
* [`flexgrid`](https://github.com/ptb/flexgrid)
* [`Gridlex`](https://github.com/devlint/gridlex)
* [`Flexbox Grid`](https://github.com/kristoferjoseph/flexboxgrid)
* [`sharps`](https://github.com/awinogradov/sharps)

### Task runner

- [`npm scripts`](https://docs.npmjs.com/misc/scripts)
- [`gulp`](https://github.com/gulpjs/gulp)

### Javascript

* [`ES6`](https://www.ecma-international.org/ecma-262/6.0/)
* [`ES7`](https://www.ecma-international.org/ecma-262/7.0/)
* [`Typescript`](https://github.com/Microsoft/TypeScript)
* [`flow`](https://github.com/facebook/flow)

### Package Manager 

* [`npm`](https://github.com/npm/cli)
* [`yarn`](https://github.com/yarnpkg/yarn)

### Javascript Framework

* [`react`](https://github.com/facebook/react)
* [`preact`](https://github.com/developit/preact)
* [`gatsbyJS`](https://github.com/gatsbyjs/gatsby)
* [`VueJS`](https://github.com/vuejs/vue)
* [`Angular`](https://github.com/angular/angular)

### JS State 

- [`redux`](https://github.com/reduxjs/redux)
- [`mobx`](https://github.com/mobxjs/mobx)
- [`rxjs`](https://github.com/ReactiveX/rxjs)
- [`flux`](https://github.com/facebook/flux)

### Module Loader & Bundler

* [`webpack`](https://github.com/webpack)

### Design Patterns (tervezési minták)

* [`Revealing Prototype Pattern`](https://gist.github.com/zcaceres/bb0eec99c02dda6aac0e041d0d4d7bf2)

# Források 

1) `w3c`
2) [`css`](http://web.axelero.hu/fodorsi/html/css1.html)
