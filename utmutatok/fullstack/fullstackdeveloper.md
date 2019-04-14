# Fullstack (web) developer, 2019

## Egy falatnyi történelem 

A webes, illetve a webes alkalmazásfejlesztés hatalmasat fejlődött az elmúlt akár 5 évben, sőt, mióta léteznek modern webalkalmazásokhoz használatos framework-ök, komoly változás következik be akár minden hatodik hónapban. Ilyenkor természetesen, illetve jobb esetben, a fejlesztőre van bízva, hogy ezeket mennyire, és milyen intenzitással hajlandó követni. 

## Mi az a fullstack fejlesztő? 

A fullstack fejlesztő az alkalmazás összes rétegét és annak összes stackjét ismeri: 

- Szerver, hálózat, és hosting ismerete
- alkalmazás skálázhatóságának ismerete 
- cloud storage ismerete
- adat redundancia 
- adat modellek imserete
- relációs, nem relációs adatbázisok ismerete
- üzleti logika ismerete
- API réteg ismerete
- MVC pattern ismerete 
- clean code alkalmazása 
- user interface átfogó ismerete 
- modern frameworkok ismerete 
- user experience 
- tisztában lenni a végfelhasználó igényeivel

##Alapok

### HTML

A `HTML` (azaz `Hypertext Markup Language`) az alapja minden weboldalnak, vagy webalkalmazásnak. A `HTML` határozza meg a weboldal (vagy webapp) szerkezetét, struktúráját, és a tartalmát. 

A `HTML` fájl `tag`-ekből, áll, aminek alapvetően két típusát különböztetjük meg:

1) Önzáró tagek (_self-closing_)

Pl.: 

```
<img src="./images/logo.png" alt="logo" />
```

2) Önzáró tagek (_self-closing_)

1) Nem önzáró tagek (_non-self-closing_)

```
<span>hello worlds</span>
```

A `HTML` tageket _tulajdonságokkal_ más néven attribútumokkal tudjuk ellátni. A fenti példában, az `img` tag-nak az `src` (azaz _source_, forrás) egy attribútuomat, ami meghatározza, a fájl nevét, és a hozzá vezető útvonalat. 

Vannak alapvető szabályok, amiket be kellt tartani `HTML` írása közben, ilyen például az a szabyályrendszer ami leírja, hogy adott elemnek milyen _leszármazottjai_ lehetnek.

Például: 

_helytelen_: 

```
<a href="demo.html">
    <label>lorem</label>
</a>
```

Ugyanis az `a` tag nem tartalmazhat `label` taget. Az ilyen, és ehhez hasonló hibák kijavítására való a [`w3c validator`](https://validator.w3.org/).  


Az összes `HTML` tag-ről elérhető egy teljes lista [itt](https://www.tutorialrepublic.com/html-reference/html5-tags.php)

#### HTML Frameworkok



### CSS

A `CSS` (azaz `Cascading Style Sheet`) egy egyszerű módszer arra, hogy adjunk _stílusokat_ adjunk az oldalainkoz, amikkel definiáljuk, hogy mi hogyan nézzen ki. 

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


#### Preprocesszorok

* [`dart-sass`](https://github.com/sass/dart-sass)
* [`less`](https://github.com/less/less.js)
* [`stylus`](https://github.com/stylus/stylus)
* [`post-css`](https://github.com/postcss/postcss)

A preprocesszorok olyan programok, amely `CSS`-t generál, a preprocesszorok saját szintaktikájából. Azeknek a hagyományos `CSS` írásával szemben olyan előnyei vannak, mint pl a változó használat, ciklusok, _nested_ szelektorok, mixinek. Ezek használatával a `CSS` írása gyorsabb, a kód tagolható, átlátható. Ezen felül segít elkerülni a kódismétlést is, amelyek nagyobb projekteknél különösen hasznos. 

A(z egyik legelterjettebb), a `sass`, vagy újabban `dart-sass`, ugyanis a régi `ruby` implementációja már elavulttá vált, az új verzió pedig a [`dart-sass`](https://github.com/sass/dart-sass) névre hallgat. 

_natív_ `CSS` kód: 

```
body p { color: #fff; }

```

A fenti selector a `body`-tagkben az összes `p` tagban lévő szöveg színét fehérre állítja. 

Ugyanez, az `SCSS` által is biztosított ún _beágyazott_ (nested) szintaktikával a következőképpen alakul: 

```
body {
    p {
        color: #fff;
    }
}
```

Majd pedig a fordító az `.scss` fájlunkból készít `.css`-t. 

Az `dart-sass`, a `less`, és a `stylus` is hasonló módon működik. Néhány szintaktikai eltérés van ezek között, azonban az közös, hogy mindegyiket _natív_ `CSS`-re kell fordítani, amiket a megszokott módon be kell húzni a `HTML` fájlokba. 

Ezek használata akkor javallott, ha semmilyen front-end frameworkot (amikről lentebb lesz szó) nem használunk, azaz lényegében a _hagyományos_ módon építünk weboldalat. 

Ezeken felül van még néhány `css-in-js` elképzelésen alapuló megoldás is. Lényeges különsbég az `SCSS`, `LESS` és társai között, hogy ezekből nem lesz _natív_ `CSS` kód, hiszen ahogy a neve is mutatja, ezek a `CSS` deklarációk `Javascript`-ben lesznek, pl. egy javascript  [`objektumban`](http://gabor.molnar.es/blog/2013/05/05/javascript-programozas-jegyzet-objektumok/).

```
const Title = styled.div`
    color: #fff;
    padding: .5rem;
    color: #000;
`;
```

Ezt a megoldást akkor érdemes használni, ha valami Javascript frameworkot használunk, vagy szeretnénk használni egy jövőbeli projekthez.  A fenti példa a [`styled-components`](https://github.com/styled-components/styled-components) nevű, `ReactJS`-ez írt komponens _formázó_ csomag (_pacakge_). 

A `styled-components`-en kívül, a `JSS`, ami framework független, de az elve ugyanaz: 

```
const styles = {
  '@global': {
    body: {
      color: '###'
    }
}
```

`CSS`-hez nagyon hasonlító stílus deklarációkat írunk, de `JS` szintaktikával. 

Ezek előnyei: 

A `JSS` egyedi osztályneveket generál amikor a deklarált stílusok `CSS`-re konvertálódnak. Ez azt a problémát oldja meg, hogy modern web komponensek fejlesztésekor a stílusok között átfedés (`conflit`) lépjen fel. Természetesen, ha haználunk bármilyen konvenciót, ez a probléma nem is lépethe fel, azonban nagyon gyorsan, nagyon átláthatlan és csúnya `CSS`-t kapnánk, ami jelentősen ront a skálázhatósági faktoron is. 

Ha használni szeretnénk valamilyen modern `javascript` frameworkot, ez a megközelítés javallott. 

* [`styled-components](https://github.com/styled-components/styled-components)
* [`css-in-js`](https://github.com/cssinjs/jss)
* [`emotion`](https://github.com/emotion-js/emotion)

### CSS frameworks 

* [`bulma`](https://github.com/jgthms/bulma)
* [`foundation`](`https://github.com/zurb/foundation-sites)
* [`flexgrid`](https://github.com/ptb/flexgrid)
* [`Gridlex`](https://github.com/devlint/gridlex)
* [`Flexbox Grid`](https://github.com/kristoferjoseph/flexboxgrid)
* [`sharps`](https://github.com/awinogradov/sharps)

### Task runners

* [`npm scripts`](https://docs.npmjs.com/misc/scripts)
* [`gulp`](https://github.com/gulpjs/gulp)

### Javascript

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

* [`redux`](https://github.com/reduxjs/redux)
* [`mobx`](https://github.com/mobxjs/mobx)
* [`rxjs`](https://github.com/ReactiveX/rxjs)
* [`flux`](https://github.com/facebook/flux)

### Module Loader & Bundler

* [`webpack`](https://github.com/webpack)

### Design Patterns 

* [`Revealing Prototype Pattern`](https://gist.github.com/zcaceres/bb0eec99c02dda6aac0e041d0d4d7bf2)

# Források 

1) `w3c`
2) [`css`](http://web.axelero.hu/fodorsi/html/css1.html)
