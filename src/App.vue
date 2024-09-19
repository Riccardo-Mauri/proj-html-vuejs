<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  data() {
    return {

    }
  },
  //2- Dichiarazione del componente 
  components: {

  },
  methods: {

  }
}
</script>

<template>
  <div>
    <!--3- Utilizzo del componenete -->
    <header>
      <div class="container d-flex justify-content-between">
        <!--link a sinistra Download APP/ ADS    a destra link con icone di FB/INST/X/YT-->
        <div>
          <a href="#">download-app</a>
          <a href="#">ads</a>
        </div>
        <div>
          <a href="#">FB</a>
          <a href="#">INST</a>
          <a href="#">X</a>
          <a href="#">YT</a>
        </div>
      </div>
      <div class="container d-flex justify-content-center"><!--logo al centro della pagina/container avada food-->
        LOGO
      </div>
      <div class="container d-flex justify-content-center">
        <!-- al centro della pagina/container link con pseudo elemento quando in hover di home/recipes/places/blog/about/contact/search-->
        <ul class="d-flex justify-content-center">
          <li>Home</li>
          <li>Recipes</li>
          <li>Places</li>
          <li>Blog</li>
          <li>About</li>
          <li>Contact</li>
          <li>search</li>
        </ul>
      </div>
    </header>
    <main>
      <section>
        <!--jumbotron con sfondo e container all'interno con scritte  -->
        <div class="jumbotron text-center p-5 bg-light">
          <div class="rounded-div mx-auto">
            <p>div al centro del jumbotron</p>
          </div>
        </div>

      </section>
      <section>
        <!--container con titolo e tre carte con immagine titolo e titoletto e alzato leggemente sopra all'altro container-->
        <div class="container">
          <div class="d-flex justify-content-center">
            <h3>FOODIE JOURNAL</h3>
          </div>
          <div class="d-flex justify-content-center">
            <div><div>img</div><h4>titolo</h4><p>desc</p></div>
            <div><div>img</div><h4>titolo</h4><p>desc</p></div>
            <div><div>img</div><h4>titolo</h4><p>desc</p></div>
          </div>
        </div>
      </section>
      <section>
        <!--container titolo paragrafo e due container divisi uno a sinistra e l'altro a destra-->
        <div class="container text-center">
          <h3>TITOLO</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, quae.</p>
        </div>
        <div class="container d-flex justify-content-between">
          <div>CONTENUTO DI SINISTRA</div>
          <div>CONTENUTO DI DESTRA</div>
        </div>
      </section>
      <section>
        <!--container con titolo paragrafo e un altro container con dentro 8 immagini con sfondo e titolo-->
        <div class="container text-center">
          <h3>TITOLO</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius, quae.</p>
        </div>
        <div class="container d-flex justify-content-between">
          <div>img</div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
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
        <div class="jumbotron text-center p-5 bg-light">
          <div class="rounded-div mx-auto">
            <h1>titolo footer</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore, aspernatur.</p>
            <div>searchbar <button>SUBSCRIBE</button></div>
            <p>Lorem ipsum dolor sit amet.</p>
          </div>
        </div>
      </section>
      <section>
        <!--sezione di mezzo con solo 4 immagini tutta la width-->
        <div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
          <div>img</div>
        </div>
      </section>
      <section>
        <!--sezione inferiore diviso in 4 container il primo con logo/icone FB/INST/X/YT  il secondo con una lista di link Recipes/places/blog/about/contact il terzo con titolo e una lista con info non link il quarto con titolo e due bottoni-->
        <div class="container">
          <div>LOGO
            <div>FB INST X YT</div>
          </div>
          <div>
            <ul>
              <li>Recipes</li>
              <li>Places</li>
              <li>Blog</li>
              <li>About</li>
              <li>Contact</li>
            </ul>
          </div>
          <div>
            <h4>Contact</h4>
            <ul>
              <li>info-icon</li>
              <li>info-icon</li>
              <li>info-icon</li>
            </ul>
          </div>
          <div>
            <h4>GET OUR APP!</h4>
            <button>google play</button>
            <button>app store</button>
          </div>
        </div>
      </section>
      <section>
        <!--sezione ultima inferiore con colore di sfondo diverso e solo una scritta copyright centrale-->
        <p>copyright</p>
      </section>
    </footer>
  </div>
</template>

<style lang="scss">
@import 'bootstrap/scss/bootstrap';

header {
  background-color: black;

}

ul>li {
  list-style: none;

}
.rounded-div {
  width: 300px;
  height: 200px;
  background-color: #f8f9fa;
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
