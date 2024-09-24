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

      //Dati per i sales in futuro può essere aggiornato
      saleslink : 39,

  
    

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
            desc: 'By admin | March 25th, 2019',
            url: '#'
          },
          {
            img: './imgs/fi-roundup-400x263.jpg',
            title: 'Roundup: My New Favourite Recipes For Healthy Living',
            desc: 'By admin | March 25th, 2019',
            url: '#'
          },
          {
            img: './imgs/fi-toasts-400x263.jpg',
            title: 'Why These Toasts with Tea are My New Favorite',
            desc: 'By admin | March 25th, 2019',
            url: '#'
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
            desc: 'By admin | March 25th, 2019',
            url: '#'
          },
          {
            img: './imgs/Mixed-fruits-200x132.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/r-rachel-park-366508-unsplash-min-200x132.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/r-michelle-tsang-500721-unsplash-min-200x132.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/quick-summer-drink-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/perfect-cosmopolitan-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/fi2x-6-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
          {
            img: './imgs/r-brooke-lark-96398-unsplash-min-460x295.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            type: '',
            desc: '',
            url: '#'
          },
        ]
      },
      //Dati per sezione immagini 4x4 con hover
      culinarycoll: [
        {
          img: './imgs/drinks-recipes.png',
          title: 'DRINKS'
        },
        {
          img: './imgs/soups-recipes.png',
          title: 'SOUPS'
        },
        {
          img: './imgs/baking-recipes.png',
          title: 'BAKERY'
        },
        {
          img: './imgs/dinner-recipes.png',
          title: 'DINNER'
        },
        {
          img: './imgs/healthy-recipes.png',
          title: 'HEALTHY'
        },
        {
          img: './imgs/staff-picks.png',
          title: 'STAFF PICKS'
        },
        {
          img: './imgs/premium-recipes.png',
          title: 'APPETISERS'
        },
        {
          img: './imgs/quick-easy-recipes.png',
          title: 'QUICK & EASY'
        },
      ],

      //Dati per mega sezione con card grande e righe di immagini
      mainarticle: {
        articles: [
          {
            img: './imgs/single-post-img3-800x527.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            data: 'By admin | March 25th, 2019',
            desc: '"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."'
          },
          {
            img: './imgs/fi-roundup-400x263.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            data: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-korean-food-400x263.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            data: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-toasts-400x263.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            data: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-street-food-400x263.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            data: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-organic-breakfast-400x263.jpg',
            title: 'Food Corner: Top Japanese Restaurants for Sushi',
            data: 'By admin | March 25th, 2019'
          },
          {
            img: './imgs/fi-water-side-rest-400x263.jpg',
            title: '5 Waterside Restaurants in Istanbul for Special Events',
            data: 'By admin | March 25th, 2019'
          },
        ]
      },
      //Dati per cityguide
      cityguide: {
        img: './imgs/singapore-featured-image-200x132.jpg',
        title: 'Singapore'
      },
      //Dati per followus
      followUs: [
        { img: '<i class="fa-brands fa-facebook-f"></i>', url: '#' },
        { img: '<i class="fa-brands fa-instagram"></i>', url: '#' },
        { img: '<i class="fa-brands fa-twitter"></i>', url: '#' },
        { img: '<i class="fa-brands fa-pinterest-p"></i>', url: '#' }
      ],
      //Dati per popular / recent messages
      isActive: 'popular', // Imposta il pulsante di default su "Popular"
      msgarray: [
        {
          img: './imgs/single-post-img3-66x66.jpg',
          message: 'Food Corner: Top Japanese Restaurants for Sushi',
          data: 'March 25th, 2019'
        },
        {
          img: './imgs/singapore-featured-image-66x66.jpg',
          message: 'City Guide: Singapore',
          data: 'February 27th, 2019'
        },
        {
          img: './imgs/slide1-bg-66x66.jpg',
          message: '6 Nutritional Tips to Help Burn Body Fat',
          data: 'February 28th, 2019'
        }
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
  }, methods: {
    setActive(button) {
      this.isActive = button; // Aggiorna il pulsante attivo
    },
  },
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
            <div class="mini-cont-jumbo py-2 px-4 rounded"><span class="text-white text-uppercase">{{ jumbocontent.desc
                }}</span>
            </div>
            <div>
              <h1>{{ jumbocontent.title }}</h1>
              <p>{{ jumbocontent.data }}</p>
            </div>
          </div>
        </div>
        <div class="sales-cont">
          <div class="bg-light border-0 rounded-1 my-1 py-1 text-center">
            <div><a href="#" class="text-black" @click.prevent ><i class="fa-solid fa-folder fs-2"></i></a></div>
            <div><span class="p-2">Demos</span></div>
          </div>
          <div class="bg-light py-1 text-center border-0 rounded-1">
            <div class="text-success"><span>$</span><span class="fs-3 fw-bold">{{saleslink}}</span></div>
            <div><span class="p-2">On Sale</span></div>
          </div>
        </div>
      </section>
      <section class="relative-cont py-5">
        <div class="container journal-cont">
          <div class="text-center mb-4">
            <h3 class="py-3 text-uppercase">{{ journalcontent.maintitle }}</h3>
          </div>

          <div class="row">
            <!-- Ciclo sui contenuti del journal -->
            <div v-for="(article, index) in journalcontent.articles" :key="index" class="col-md-4">
              <div class="card journal-card border-0 text-center my-2">
                <!-- Immagine con overlay e link -->
                <div class="card-img-wrapper position-relative">
                  <a :href="article.url" @click.prevent class="d-block">
                    <img :src="article.img" alt="Journal image" class="journal-img img-fluid">
                    <!-- Overlay arancione con link e titolo -->
                    <div class="hover-overlay d-flex justify-content-center align-items-center flex-column">
                      <div class="hover-icon mb-2">
                        <i class="fa fa-link"></i>
                      </div>
                      <h4 class="overlay-title text-white">{{ article.title }}</h4>
                    </div>
                  </a>
                </div>
                <!-- Titolo sempre visibile sotto l'immagine -->
                <h4 class="mt-3">{{ article.title }}</h4>
                <p>{{ article.desc }}</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section class="fixed-cont">
        <!-- Titolo e paragrafo -->
        <div class="container text-center">
          <h3>POPULAR RECIPES</h3>
          <p class="py-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, quae.</p>
        </div>

        <div class="container d-flex justify-content-between">
          <!-- Container di sinistra: mostra solo il primo articolo -->
          <div class="card recipes-cont col-6 border-0 rounded-0 position-relative">
            <div class="position-relative"> <!-- Aggiunto per il posizionamento dell'overlay -->
              <img :src="popularrecipes.articles[0].img" alt="Recipe Image" class="img-fluid">

              <!-- Overlay per l'immagine -->
              <div class="hover-overlay d-flex justify-content-center align-items-center flex-column">
                <a :href="popularrecipes.articles[0].url" @click.prevent class="hover-icon mb-2">
                  <!-- Rendi l'icona un link -->
                  <i class="fa fa-link"></i>
                </a>
                <h4 class="overlay-title">{{ popularrecipes.articles[0].title }}</h4> <!-- Titolo nell'overlay -->
              </div>
            </div>

            <h4 class="px-4 py-4">{{ popularrecipes.articles[0].title }}</h4>
            <p class="px-4">{{ popularrecipes.articles[0].type }}</p>
            <div class="px-4">
              <hr>
            </div>
            <p class="px-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam cupiditate quam, cum quaerat sed
              debitis qui aperiam maiores voluptas exercitationem quo. Optio maiores minima ipsa animi unde ab illo
              aliquam sit, qui eaque eum quasi corporis id, alias corrupti odit ea laboriosam dignissimos nostrum error!
              Fugiat adipisci ea dolorum maiores.
            </p>
            <div class="px-4 my-5">
              <button class="py-2 sub-button">LEARN MORE</button>
            </div>
          </div>

          <!-- Container di destra: mostra solo le immagini degli altri articoli -->
          <div class="col-6 px-3">
            <div class="row">
              <!-- Itera su tutti gli articoli tranne il primo e mostra 2 immagini per riga -->
              <div v-for="(article, index) in popularrecipes.articles.slice(1)" :key="index"
                class="col-6 mb-3 pm-3 d-flex justify-content-center position-relative card-img-wrapper">
                <img :src="article.img" alt="Recipe Image" class="img-articles img-fluid">
                <!-- Overlay hover per le immagini più piccole -->
                <div class="hover-overlay d-flex justify-content-center align-items-center flex-column">
                  <a :href="article.url" @click.prevent class="hover-icon mb-2"> <!-- Rendi l'icona un link -->
                    <i class="fa fa-link"></i>
                  </a>
                  <h4 class="overlay-title">{{ article.title }}</h4> <!-- Mostra il titolo qui -->
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>


      <section class="py-5">
        <div class="container text-center py-5">
          <h3 class="py-5">CULINARY COLLECTION</h3>
          <p class="py-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, quae.</p>
        </div>
        <div class="container">
          <div class="row">
            <div v-for="(item, index) in culinarycoll" :key="index" class="col-3 mb-4">
              <div class="card border-0 rounded-0 text-center hover-card">
                <img :src="item.img" alt="Culinary Image" class="img-fluid img-culinary">
                <div class="title-container mt-2"> <!-- Nuovo div per il titolo -->
                  <h5 class="title-hover">{{ item.title }}</h5>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>




      <section>
        <!--container con a sinistra titolo e paragrafo e a destra un buttone arancione-->
        <div class="container d-flex justify-content-between align-items-center">
          <div class="col-10">
            <div>FARM TO TABLE</div>
            <div>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quasi, quas.</div>
          </div>
          <div>
            <button class="py-2 sub-button">READ OUR BLOG <span><i class="fa-solid fa-book-open"></i></span></button>
          </div>
        </div>
      </section>
      <section>
        <!--mega section con un container diviso in due 80/20 a sinistra il container di 80% con una card principale enorme con sotto 6 cards da 2 per riga con  titolo/paragrafo/descrizione/ a sinistra readm more e a destra icona commenti e sotto una riga con load more posts
        la seconda parte a destra di 20% del container avrà a immagine con sotto un altra immagine-descrizione laterale e sotto una hr una search bar un div con "follow us" e icone FB/ISNT/X/YT/P , sotto ancora un altro div con tre righe di icone rotonde paragrafo , infine un div con simulazione di tweets-->
        <div class="container d-flex justify-content-between py-5">
          <div class="col-8">
            <div class="mb-4">
              <!-- Card più grande -->
              <div class="card border-0 rounded-0">
                <img :src="mainarticle.articles[0].img" class="card-img-top rounded-0" alt="Article Image">
                <div class="card-body">
                  <h5 class="card-title">{{ mainarticle.articles[0].title }}</h5>
                  <p class="card-text">{{ mainarticle.articles[0].data }}</p>
                  <div>
                    <hr class="style-hr">
                  </div>
                  <p>{{ mainarticle.articles[0].desc }}</p>
                  <div class="d-flex justify-content-between">
                    <div><a href="#" @click.prevent class="readlink-card">Read More ></a></div>
                    <div><span><i class="fa-regular fa-comments"></i></span></div>
                  </div>
                </div>
              </div>
            </div>

            <div>
              <div class="row">
                <!-- Righe di card più piccole -->
                <div class="col-6" v-for="(article, index) in mainarticle.articles.slice(1)" :key="index">
                  <div class="card border-0 rounded-0 mb-4">
                    <img :src="article.img" class="card-img-top rounded-0" alt="Article Image">
                    <div class="card-body">
                      <h5 class="card-title text-center">{{ article.title }}</h5>
                      <p class="card-text text-center">{{ article.data }}</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <div class="text-center mt-4">
              <button class="border-0 w-100 py-2 text-black">LOAD MORE POSTS</button>
            </div>
          </div>
          <div class="col-3">
            <div class="z d-flex justify-content-center align-items-center w-100">
              <div class="text-center w-50 h-50 py-5">
                <h4>VIEW OUR LATEST RECIPE</h4>
              </div>
            </div>
            <div class="w-100 city-guide py-4">
              <img class="w-100" :src="cityguide.img" alt="cityguide.title">
              <div class="city-desc p-1">City Guide: {{ cityguide.title }}</div>
              <div><button class="w-100 border-0 p-1 sub-button">VIEW ALL CITY GUIDES</button></div>
            </div>
            <div class="py-2">
              <hr>
            </div>
            <div class="py-2">
              <div class="search-container">
                <input type="search" name="search" id="searchbar" placeholder="Search..."
                  class="border-1 rounded-1 p-1 w-100">
              </div>

            </div>
            <div>
              <div class="py-5">
                <button :class="['border-1', isActive === 'popular' ? 'active-button' : '', 'tweet-button', 'w-50']"
                  @click="setActive('popular')">
                  Popular
                </button>
                <button :class="['border-1', isActive === 'recent' ? 'active-button' : '', 'tweet-button', 'w-50']"
                  @click="setActive('recent')">
                  Recent
                </button>
              </div>
              <div>
                <div v-for="(msg, index) in msgarray" :key="index" class="d-flex py-2">
                  <div class="rounded-circle">
                    <img :src="msg.img" alt="Message Image" class="rounded-circle" />
                  </div>
                  <div class="px-2">
                    <p>{{ msg.message }}</p>
                    <p>{{ msg.data }}</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="border-0 rounded-1 tweet-cont">
              <div class="container py-2">
                <div>
                  <h5>Tweets <span>By<a href="#" @click.prevent >@theme_fusion</a></span></h5>
                </div>
                <ul>
                  <li class="py-1">
                    <h6>ThemeFusion</h6>
                    <span>@theme_fusion</span>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi labore commodi sequi? Repellat
                      cupiditate blanditiis recusandae natus, aperiam sint numquam, in provident voluptatibus, voluptate
                      molestiae dolorum eaque doloribus commodi quidem!</p>
                    <div class="py-1"><img src="../public/imgs/En2TRxLW4AEiWUN.jpeg" alt="" class="img-tweet"></div>
                    <div class="d-flex justify-content-between py-2">
                      <div><span><i class="fa-regular fa-heart"></i></span><span class="px-3"><i
                            class="fa-solid fa-right-from-bracket"></i></span></div>
                      <div><span>21h</span></div>
                    </div>
                  </li>
                </ul>
              </div>
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
              <a class="text-secondary px-2" v-for="(icon, index) in headerrightLinks" :key="index" :href="icon.url" @click.prevent >
                <i :class="icon.iconClass"></i>
              </a>
            </div>
          </div>
          <div class="col-3 py-4 border-end">
            <ul>
              <li class="py-2" v-for="(link, index) in footerlink" :key="index">
                <a :href="link.url" class="footer-link" v-html="link.text" @click.prevent ></a>
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
  font-size: 18px;
  font-weight: 500;
  padding: 10px;
  transition: color 0.3s ease;

}


a.nav-link::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 50%;
  width: 0;
  height: 2px;
  background-color: #ff6347;
  transition: width 0.3s ease, left 0.3s ease;
}

a.nav-link:hover {
  color: #ff6347;

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
  position: relative;
}

.mini-cont-jumbo {
  background-color: #ff6347;
  position: absolute;
  top: -20px;
}

.sales-cont {
  position: absolute;
  top: 210px;
  right: 20px;
}

.relative-cont {
  position: relative;
}

.journal-cont {
  position: relative;
}

.journal-img {
  width: 100%;
  height: auto;
  display: block;
  transition: all 0.3s ease;
}


.card-img-wrapper {
  position: relative;
  overflow: hidden;
}

.readlink-card {
  text-decoration: none;
  color: #000;
}

.hover-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #ff6347b7;
  transition: opacity 0.3s ease;
  opacity: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.card:hover .hover-overlay {
  opacity: 1;
}


.hover-icon {
  width: 50px;
  height: 50px;
  background-color: white;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.hover-icon i {
  font-size: 20px;
  color: black;
}


.overlay-title {
  font-size: 1.2rem;
  margin-top: 10px;
  text-align: center;
  color: white;
}

h4 {
  margin: 0;
  font-size: 1.2rem;
}

p {
  font-size: 0.9rem;
  margin-top: 10px;
  margin-bottom: 0;
}

.card-img-wrapper {
  position: relative;
  overflow: hidden;
}

.img-articles {
  width: 100%;
  height: auto;
  transition: transform 0.3s ease;
}

.card-img-wrapper:hover .hover-overlay {
  opacity: 1;
}

/* Icona circolare */
.hover-icon {
  width: 50px;
  height: 50px;
  background-color: white;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.hover-icon i {
  font-size: 20px;
  color: black;
}

.journal-cont {
  position: absolute;
  left: 0;
  right: 0;
  top: -70px;
  background-color: white;
}

.recipes-cont img {
  width: 100%;
  height: auto;
  display: block;
}

.hover-icon {
  color: white;
  font-size: 24px;
}

.fixed-cont {
  padding-top: 500px;
}

.img-articles {
  width: 100%;
  height: 100%;
}

.title-container {
  transition: background-color 0.3s ease;
  padding: 10px;
}

.title-container:hover {
  background-color: #ff6347;
}

.title-hover {
  transition: color 0.3s ease;
  color: black;
}

.title-container:hover .title-hover {
  color: white;
}



.img-culinary {
  width: 50%;
  height: 50%;
  display: block;
  margin: 0 auto;
}

.z {
  height: 400px;
  background-image: url(../public/imgs/ad-bg.jpg);
  background-size: cover;
}

.city-guide {
  position: relative;
}

.city-desc {
  position: absolute;
  top: 170px;
  background-color: black;
  color: white;
}

.links-follow-us {
  margin-right: 10px;
  width: 40px;
  height: 40px;
  border: 1px solid #67615A;

}

.icon-link {
  text-decoration: none;
  font-size: 1.5rem;
  color: #67615A;
}

.tweet-button {
  height: 50px;
  background-color: #f5f5f1;
}

.tweet-cont {
  background-color: white;
}

.active-button {
  background-color: white;
}

.img-tweet {
  width: 80%;
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
