<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  data() {
    return {
      // Dati per i link a sinistra
      headerleftLinks: [
        { text: 'Download App', url: '#', extra: 'IOS' },
        { text: 'Advertise with us', url: '#' }
      ],
      // Dati per i link a destra con icone Font Awesome
      headerrightLinks: [
        { iconClass: 'fa-brands fa-facebook', url: '#' },
        { iconClass: 'fa-brands fa-instagram', url: '#' },
        { iconClass: 'fa-brands fa-twitter', url: '#' },
        { iconClass: 'fa-brands fa-youtube', url: '#' }
      ],
      //logo del sito
      logo: '/imgs/avada-food-logo.png',

      // Dati per i link in centro header
      headermainlink: [
        { text: 'Home', url: '#' },
        { text: 'Recipes', url: '#' },
        { text: 'Places', url: '#' },
        { text: 'Blog', url: '#' },
        { text: 'About', url: '#' },
        { text: 'Contact', url: '#' },
        { text: '<i class="fa-solid fa-magnifying-glass"></i>', url: '#' } // Icona Font Awesome
      ],

      //-----------------------------------------------MAIN CONTETNT---------------------------------------------------------

      //Dati per jumbotron
      jumbocontent: {
        desc: 'Today\'s pick',
        title: 'Food Corner: Top Japanese Restaurants for Sushi',
        data: 'March 25, 2019',
      },

      //Dati per giornale sul cibo titolo/ tre immagini con titolo e descrizione
      journalcontent: {
        maintitle: ' Foodie Journal',
        articles: [
          {
            img: './imgs/single-post-img3-400x263.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            desc: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-roundup-400x263.jpg',
            title: 'Roundup: My New Favourite Recipes For Healthy Living',
            desc: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-toasts-400x263.jpg',
            title: 'Why These Toasts with Tea are My New Favorite',
            desc: 'By admin | March 25th, 2019'
          }
        ]
      },
      //Dati per popular recipes 
      popularrecipes: {
        articles: [
          {
            img: './imgs/Yogurt-Nan-600x395.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: 'Bakery,Featured,Healthy,Latest Recipes, Staff Picks',
            desc: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/Mixed-fruits-200x132.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/r-rachel-park-366508-unsplash-min-200x132.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/r-michelle-tsang-500721-unsplash-min-200x132.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/quick-summer-drink-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/perfect-cosmopolitan-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/fi2x-6-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
          {
            img: './imgs/r-brooke-lark-96398-unsplash-min-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: ''
          },
        ]
      },
      //Dati per sezione immagini 4x4 con hover
      culinarycoll: [
        { img: './imgs/drinks-recipes.png',
          title: 'DRINKS'
         },
        { img: './imgs/soups-recipes.png',
          title: 'SOUPS'
         },
        { img: './imgs/baking-recipes.png',
          title: 'BAKERY'
         },
        { img: './imgs/dinner-recipes.png',
          title: 'DINNER'
         },
        { img: './imgs/healthy-recipes.png',
          title: 'HEALTHY'
         },
        { img: './imgs/staff-picks.png',
          title: 'STAFF PICKS'
         },
        { img: './imgs/premium-recipes.png',
          title: 'APPETISERS'
         },
        { img: './imgs/quick-easy-recipes.png',
          title: 'QUICK & EASY'
         },
      ],











      //array immagini footer
      footerimgs: [
        { img: './imgs/Yogurt-Nan-400x263.jpg' },
        { img: './imgs/Mixed-fruits-400x263.jpg' },
        { img: './imgs/r-rachel-park-366508-unsplash-min-400x263.jpg' },
        { img: './imgs/r-michelle-tsang-500721-unsplash-min-400x263.jpg' },
      ],

      //logo del footer
      footerlogo: '/imgs/avada-food-logo-mob-2x-200x87.png',

      //Dati per i Link del footer
      footerlink: [
        { text: 'Recipes', url: '#' },
        { text: 'Places', url: '#' },
        { text: 'Blog', url: '#' },
        { text: 'About', url: '#' },
        { text: 'Contact', url: '#' },
      ],
      appicon: {
        imggplay: './imgs/download-android-200x66.png',
        imgstore: './imgs/download-app-store-200x66.png'
      }
    };
  }
}
</script>

<template>
  <div>
    <header>
      <div class="container d-flex justify-content-between py-2">
        <!-- Link a sinistra -->
        <div>
          <a class="text-decoration-none text-secondary px-1 " v-for="(link, index) in headerleftLinks" :key="index"
            :href="link.url">
            {{ link.text }}
            <span class="ios-text" v-if="link.extra">{{ link.extra }}</span>
          </a>
        </div>

        <!-- Link a destra con icone -->
        <div>
          <a class="text-secondary px-2" v-for="(icon, index) in headerrightLinks" :key="index" :href="icon.url">
            <i :class="icon.iconClass"></i>
          </a>
        </div>
      </div>
      <div class="container d-flex justify-content-center py-4"><!--logo al centro della pagina/container avada food-->
        <div><img :src="logo" alt="logo.png"></div>
      </div>
      <div class="container d-flex justify-content-center">
        <!-- Al centro della pagina/container con pseudo-elemento all'hover -->
        <ul class="d-flex justify-content-center">
          <li class="px-3 py-1" v-for="(link, index) in headermainlink" :key="index">
            <a :href="link.url" class="nav-link" v-html="link.text"></a>
          </li>
        </ul>
      </div>
    </header>
    <main>
      <section>
        <!--jumbotron con sfondo e container all'interno con scritte  -->
        <div class="jumbotron text-center d-flex align-items-center p-5 bg-light">
          <div class="rounded-div mx-auto">
            <div class="f py-2 px-4 rounded"><span class="text-white text-uppercase">{{ jumbocontent.desc }}</span>
            </div>
            <div>
              <h1>{{ jumbocontent.title }}</h1>
              <p>{{ jumbocontent.data }}</p>
            </div>
          </div>
        </div>

      </section>
      <section class="relative-cont">
        <!--container con titolo e tre carte con immagine titolo e titoletto e alzato leggemente sopra all'altro container-->
        <div class="container border border-2 z">
          <div class="d-flex justify-content-center">
            <h3>{{ journalcontent.maintitle }}</h3>
          </div>
          <div class="d-flex justify-content-center">
            <!-- Ciclo sui contenuti del journal -->
            <div v-for="(article, index) in journalcontent.articles" :key="index"
              class="col-4 card d-flex justify-content-betweeen border-0 text-center my-2 px-4 py-4">
              <img :src="article.img" alt="Journal image" class="journal-img">
              <h4>{{ article.title }}</h4>
              <p>{{ article.desc }}</p>
            </div>
          </div>
        </div>
      </section>
      <section class="fixed-cont">
        <!-- Titolo e paragrafo -->
        <div class="container text-center">
          <h3>POPULAR RECIPES</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, quae.</p>
        </div>

        <div class="container d-flex justify-content-between">
          <!-- Container di sinistra: mostra solo il primo articolo -->
          <div class="card col-6 mx-3 border-0 rounded-0">
            <img :src="popularrecipes.articles[0].img" alt="Recipe Image" class="img-fluid">
            <h4 class="px-4 py-4">{{ popularrecipes.articles[0].title }}</h4>
            <p class="px-4">{{ popularrecipes.articles[0].desc }}</p>
            <div class="px-4">
              <hr>
            </div>
            <p class="px-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam cupiditate quam, cum
              quaerat sed
              debitis qui aperiam maiores voluptas exercitationem quo. Optio maiores minima ipsa animi unde ab illo
              aliquam sit, qui eaque eum quasi corporis id, alias corrupti odit ea laboriosam dignissimos nostrum error!
              Fugiat adipisci ea dolorum maiores.</p>
            <div class="px-4 my-5"><button class="py-2 sub-button">LEARN MORE</button></div>
          </div>

          <!-- Container di destra: mostra solo le immagini degli altri articoli -->
          <div class="col-6 mx-3">
            <div class="row">
              <!-- Itera su tutti gli articoli tranne il primo e mostra 2 immagini per riga -->
              <div v-for="(article, index) in popularrecipes.articles.slice(1)" :key="index"
                class="col-6 mb-3 d-flex justify-content-center">
                <img :src="article.img" alt="Recipe Image" class="img-articles">
              </div>
            </div>
          </div>
        </div>
      </section>

      <section class="py-5">
        <!--container con titolo paragrafo e un altro container con dentro 8 immagini con sfondo e titolo-->
        <div class="container text-center py-5">
          <h3 class="py-5">CULINARY COLLECTION</h3>
          <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, quae.</p>
        </div>
        <div class="container">
          <div class="row">
            <!-- Itera sui dati della collezione culinaria per creare la griglia 4x2 -->
            <div v-for="(item, index) in culinarycoll" :key="index" class="col-3 mb-4">
              <div class="card border-0 rounded-0 text-center hover-card">
                <img :src="item.img" alt="Culinary Image" class="img-fluid img-culinary">
                <h5 class="mt-2">{{ item.title }}</h5>
              </div>
            </div>
          </div>
        </div>
        
      </section>
      <section>
        <!--container con a sinistra titolo e paragrafo e a destra un buttone arancione-->
        <div class="container d-flex">
          <div>
            <div>TITOLO</div>
            <div>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quasi, quas.</div>
          </div>
          <div>
            <button>READ OUR BLOG</button>
          </div>
        </div>
      </section>
      <section>
        <!--mega section con un container diviso in due 80/20 a sinistra il container di 80% con una card principale enorme con sotto 6 cards da 2 per riga con  titolo/paragrafo/descrizione/ a sinistra readm more e a destra icona commenti e sotto una riga con load more posts
        la seconda parte a destra di 20% del container avrà a immagine con sotto un altra immagine-descrizione laterale e sotto una hr una search bar un div con "follow us" e icone FB/ISNT/X/YT/P , sotto ancora un altro div con tre righe di icone rotonde paragrafo , infine un div con simulazione di tweets-->
        <div class="container d-flex justify-content-between">
          <div>
            CONTAINER DI SINISTRA AL 80%
            <div>CARD PIù GRANDE</div>
            <div>CARD PIù PICCOLA</div>
            <div>CARD PIù PICCOLA</div>
            <div>CARD PIù PICCOLA</div>
            <div>CARD PIù PICCOLA</div>
            <div>CARD PIù PICCOLA</div>
            <div>CARD PIù PICCOLA</div>
            <div>LOAD MORE POSTS</div>
          </div>
          <div>
            CONTAINER DI DESTRA AL 20%
            <div>card con immagine</div>
            <div>card più piccola con immagine e descrizione</div>
            <hr>
            <div>searchbar</div>
            <div>
              <div>Follow Us</div>
              <div>FB INST X YT P</div>
            </div>
            <div>
              <div>
                <button>Popular</button>
                <button>Recent</button>
              </div>
              <div>
                <div>img/desc</div>
                <div>img/desc</div>
                <div>img/desc</div>
              </div>
            </div>
            <div>
              finto tweet
            </div>
          </div>
        </div>
      </section>
    </main>
    <footer>
      <section>
        <!--sezione sopra con sfondo background al centro un container con titolo/paragrafo/searchbar/subscribe button/ paragrafo piccolino-->
        <div class="jumbotron text-center p-5 bg-light footer-jumbo">
          <div class="center-div mx-auto">
            <h1 class="col-12 my-4">Subscribe <span class="special-text">&</span> Receive A Free eBook</h1>
            <p class="col-12 my-4 py-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore, aspernatur.
            </p>
            <div class="col-12 my-4 py-3"><input class="border border-1 rounded-2 px-5 py-2 mx-2" type="email"
                placeholder="Insert your email _*"><button class="py-2 sub-button">SUBSCRIBE</button></div>
            <p class="col-12 my-4 py-3">Lorem ipsum dolor sit amet.</p>
          </div>
        </div>
      </section>
      <section>
        <!-- Sezione di mezzo con solo 4 immagini che occupano tutta la larghezza -->
        <div class="footer-imgs-container d-flex">
          <div v-for="(image, index) in footerimgs" :key="index" class="footer-img flex-fill">
            <img :src="image.img" alt="Footer image" class="img-fluid" />
          </div>
        </div>
      </section>
      <section>
        <!--sezione inferiore diviso in 4 container il primo con logo/icone FB/INST/X/YT  il secondo con una lista di link Recipes/places/blog/about/contact il terzo con titolo e una lista con info non link il quarto con titolo e due bottoni-->
        <div class="container d-flex py-5">
          <div class="col-3 py-4 border-end">
            <img :src="footerlogo" alt="footerlogo">
            <div class="py-4">
              <a class="text-secondary px-2" v-for="(icon, index) in headerrightLinks" :key="index" :href="icon.url">
                <i :class="icon.iconClass"></i>
              </a>
            </div>
          </div>
          <div class="col-3 py-4 border-end">
            <ul>
              <li class="py-2" v-for="(link, index) in footerlink" :key="index">
                <a :href="link.url" class="footer-link" v-html="link.text"></a>
              </li>
            </ul>
          </div>
          <div class="col-3 py-4 px-4 border-end">
            <h5 class="footer-titles">Contact</h5>
            <ul>
              <li class="py-3"><span><i class="fa-solid fa-location-dot"></i></span><span class="px-2">775 New York Ave,
                  Brooklyn,Kings, New York 11203</span></li>
              <li class="py-3"><span><i class="fa-solid fa-phone-flip"></i></span><span class="px-2">+
                  0100-505-0000</span></li>
              <li class="py-3"><span><i class="fa-solid fa-envelope"></i></span><span
                  class="px-2">info@your-domain.com</span></li>
            </ul>
          </div>
          <div class="col-3 py-4 px-4">
            <h5 class="footer-titles">GET OUR APP!</h5>
            <button class="border-0 rounded my-2"><img :src="appicon.imggplay" alt="Google Play Store"></button>
            <button class="border-0 rounded"><img :src="appicon.imgstore" alt="Apple App Store"></button>
          </div>
        </div>
      </section>
      <section class="copyright-cont">
        <!--sezione ultima inferiore con colore di sfondo diverso e solo una scritta copyright centrale-->
        <p>copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</p>
      </section>
    </footer>
  </div>
</template>

<style lang="scss">
@import 'bootstrap/scss/bootstrap';

header {
  background-color: #f5f5f1;

}

header>div a {
  font-size: 0.9rem;
}

ul>li {
  /* rimozione dei pallini nelle liste */
  list-style: none;
}

.ios-text {
  background-color: #ff6347;
  border-radius: 2px;
  border: 1px;
  color: white;
  font-size: 0.75rem;
  padding: 2px;
}

a.nav-link {
  position: relative;
  text-decoration: none;
  font-size: bold;
  color: #000;
  /* Colore del testo */
  font-size: 18px;
  font-weight: 500;
  padding: 10px;
  transition: color 0.3s ease;
  /* Transizione del colore */
}

/* Pseudo-elemento per l'effetto hover */
a.nav-link::after {
  content: '';
  position: absolute;
  bottom: -5px;
  /* Posiziona la linea subito sotto il link */
  left: 50%;
  width: 0;
  height: 2px;
  background-color: #ff6347;
  /* Colore della linea */
  transition: width 0.3s ease, left 0.3s ease;
}

a.nav-link:hover {
  color: #ff6347;
  /* Colore quando si passa sopra il link  */
}

a.nav-link:hover::after {
  width: 100%;
  left: 0;
}

.rounded-div {
  width: 800px;
  height: 300px;
  background-color: white;
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}

main {
  background-color: #f5f5f1;
}

.jumbotron {
  height: 700px;
  background-image: url(../public/imgs/single-post-img3.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

.f {
  background-color: #ff6347;
  position: absolute;
  top: -20px;
}

.relative-cont {
  position: relative;
}

.z {
  position: absolute;
  left: 0;
  right: 0;
  top: -70px;
  background-color: white;
}

.fixed-cont {
  padding-top: 500px;
}

.img-articles {
  width: 100%;
  height: 100%;
}
.img-culinary {
  width: 50%;
  height: 50%;
  display: block; 
  margin: 0 auto;
}




.footer-jumbo {
  background-image: url(../public/imgs/subscribe-sec-bg.png);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  background-color: white;
}

.center-div {
  width: 800px;
  height: 300px;
}

.special-text {
  color: #ff6347;
}

.sub-button {
  background-color: #ff6347;
  color: white;
  padding-left: 15px;
  padding-right: 15px;
  border: none;
  font-weight: bold;
}

.footer-imgs-container {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.footer-img {
  flex: 1;
}

.footer-img img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.footer-link {
  text-decoration: none;
  list-style: none;
  color: #000;
  font-size: 18px;
  font-weight: 500;
}

.footer-titles {
  color: #ff6347;
}

.copyright-cont {
  text-align: center;
  background-color: #f5f5f1;
}

.copyright-cont>p {
  padding: 30px;
}
</style>
