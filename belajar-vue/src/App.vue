<script>
export default {
  data() {
    return {};
  },
  // untuk file vanila javascript
  mounted() {
    var menuBtn = document.getElementById("menuBtn");

    // nav
    var sideNav = document.getElementById("sideNav");
    sideNav.style.right = "-250px";
    menuBtn.onclick = function () {
      if (sideNav.style.right == "-250px") {
        sideNav.style.right = "0";
      } else {
        sideNav.style.right = "-250px";
      }
    };

    // scroll animation
    var scroll = new SmoothScroll('a[href*="#"', {
      speed: 1000,
      speedAsDuration: true,
    });
  },
};
</script>

<template>
  <header>
    <nav id="sideNav">
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#tools">Services</a></li>
        <li><a href="#ourwork">Our Works</a></li>
        <li><a href="#testi">Testimonial</a></li>
        <li><a href="#about">About</a></li>
      </ul>
    </nav>
    <img src="../src/assets/img/menu-icon.png" id="menuBtn" />
  </header>

  <main>
    <!-- Home -->
    <article id="home">
      <div class="container">
        <img src="../src/assets/img/logo-piandtech.png" class="logo" />
        <div class="home-text">
          <h1>Bingung Cara Edit konten Produk Mu ?</h1>
          <span class="square"></span>
          <p>Disini kami hadir membatu kamu agar dapat mengedit konten produkmu dengan mudah tanpa ribet otak-atik desain</p>
          <a href="#detail1">
            <button id="homeBtn">Lihat Lebih Detail</button>
          </a>
        </div>
      </div>
    </article>

    <!-- Detail1 -->
    <article id="detail1">
      <div class="detail1-left-col">
        <img src="../src/assets/img/detail1.png" />
      </div>
      <div class="detail1-right-col">
        <div class="detail1-text">
          <h1>Mengapa Konten<br />Produk Penting</h1>
          <span class="square"></span>
          <p>
            Konten produk berkualitas merupakan hal penting untuk mendapatkan perhatian dari calon pelanggan potensial anda. Apalagi didukung dengan menggabungkan kualitas gambar menggunakan media yang menarik akan sangat menguntungkan
            seller. Tingkatin marketing promosi Anda dengan Desain Promosi yang menarik, kreatif, profesional.
          </p>
        </div>
      </div>
    </article>

    <!-- detail2 -->
    <article id="detail2">
      <div class="container detail2-row">
        <div class="detail2-left-col">
          <div class="detail2-text">
            <h1>Gak ada waktu buat ngedit ?</h1>
            <span class="square"></span>
            <p>Membuat konten yang menarik dan berkualitas memang membutuhkan waktu yang tidak sedikit, oleh karena itu kami hadir untuk membantu kamu membuat konten dengan biaya yang sangat terjangkau</p>
          </div>
        </div>
        <div class="detail2-right-col">
          <img src="../src/assets/img/detail2.jpg" />
        </div>
      </div>
    </article>

    <!-- Tools Container -->
    <article id="tools">
      <div class="tools-text">
        <h1>Services</h1>
        <p>Tools atau Software desain yang kami gunakan :)</p>
      </div>
      <div class="tools-row">
        <div class="tools-col card">
          <img src="../src/assets/img/ai-logo.png" alt="3D Modeling" />
          <h4>Illustrator</h4>

          <p>Software Desain Grafis berbasis Vektor, untuk Desain ilustrasi dan visual</p>
        </div>
        <div class="tools-col card">
          <img src="../src/assets/img/ps-logo.png" />
          <h4>Photoshop</h4>
          <p>Software Desain Grafis berbasis Bitmap, untuk pengeditan foto/gambar</p>
        </div>
        <div class="tools-col card">
          <img src="../src/assets/img/corel-logo.png" />
          <h4>Corel Draw</h4>
          <p>Software Desain Grafis berbasis Vektor, untuk Desain ilustrasi dan visual</p>
        </div>
      </div>
    </article>

    <!-- OurWorks -->
    <article id="ourwork">
      <div class="ourwork-text">
        <h1>Our Works</h1>
      </div>
      <div class="tools-row">
        <figure class="ourwork-card">
          <div class="image"><img src="../src/assets/img/sesi1.jpg" alt="obj1" /></div>
          <figcaption>
            <div class="date"><span class="day">23</span><span class="month">Juli</span></div>
            <h3>3D Object Text</h3>
            <p>Dibuat dengan blender 3D text agar tampak timbul.</p>
          </figcaption>
        </figure>
        <figure class="ourwork-card">
          <div class="image"><img src="../src/assets/img/sesi3.jpg" alt="obj2" /></div>
          <figcaption>
            <div class="date"><span class="day">30</span><span class="month">Juli</span></div>
            <h3>3D Lowpoly Computer</h3>
            <p>Dibuat dengan blender 3D simple lowpoly computer</p>
          </figcaption>
        </figure>
        <figure class="ourwork-card">
          <div class="image"><img src="../src/assets/img/sesi2.jpg" alt="cdr1" /></div>
          <figcaption>
            <div class="date"><span class="day">01</span><span class="month">Juli</span></div>
            <h3>Digital Imaging</h3>
            <p>Dibuat dengan Photoshop simple digital imaging</p>
          </figcaption>
        </figure>
      </div>
    </article>

    <!-- testi -->
    <article id="testi">
      <div class="testi-text">
        <h1>Testimoni</h1>
        <p>Dari Mereka yang menggunakan jasa kami</p>
      </div>
      <div class="tools-row">
        <div class="tools-col">
          <figure class="testi-card">
            <blockquote>Calvin: Sometimes when I'm talking with others, my words can't keep up with my thoughts. I wonder why we think faster than we speak. Hobbes: Probably so we can think twice.</blockquote>
            <div class="author">
              <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/331810/sq-sample1.jpg" alt="sq-sample1" />
              <h5>Pelican Steve <span> LittleSnippets</span></h5>
            </div>
          </figure>
        </div>
        <div class="tools-col">
          <figure class="testi-card hover">
            <blockquote>
              Thank you. before I begin, I'd like everyone to notice that my report is in a professional, clear plastic binder...When a report looks this good, you know it'll get an A. That's a tip kids. Write it down.
            </blockquote>
            <div class="author">
              <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/331810/sq-sample24.jpg" alt="sq-sample24" />
              <h5>Max Conversion<span> LittleSnippets</span></h5>
            </div>
          </figure>
        </div>
        <div class="tools-col">
          <figure class="testi-card">
            <blockquote>My behaviour is addictive functioning in a disease process of toxic co-dependency. I need holistic healing and wellness before I'll accept any responsibility for my actions.</blockquote>
            <div class="author">
              <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/331810/sq-sample29.jpg" alt="sq-sample29" />
              <h5>Eleanor Faint<span> LittleSnippets</span></h5>
            </div>
          </figure>
        </div>
      </div>
    </article>

    <!-- about -->
    <article class="about-dev container detail2-row">
      <section id="about">
        <div class="detail2-left-col">
          <div class="detail2-text">
            <h1>About us</h1>
            <span class="square"></span>
            <p>Phi.and.Tech bergerak dalam bidang desain graphic dan tecnologi, termasuk dokumentasi pribadi, karya gabut, orderan dari anda anda orang random yang ada di dunia maya</p>
            <br />
            <q>Makan Kupat Campur Pepaya, Yo ndak tau kok tanya saya</q>
            <small>--bukan saya</small>
          </div>
        </div>
      </section>

      <!-- Created by -->
      <aside id="creator">
        <article class="profile cardProfile">
          <header>
            <h3>Created by</h3>
            <br />
            <figure>
              <img src="../src/assets/img/profile.jpg" />
            </figure>
            <br />
            <h3>Digdaya R</h3>
          </header>
          <section>
            <br />
            <h5>Desain Grafis & Illustrator</h5>
            <p>Rdigdaya84@gmail.com</p>
            <p>Nganjuk</p>
          </section>
        </article>
      </aside>
    </article>
  </main>

  <!-- Footer -->
  <footer>
    <section id="footer">
      <div class="container footer-row">
        <hr />
        <div class="footer-left-col">
          <div class="footer-links">
            <div class="link-title">
              <h4>Project</h4>
              <small
                ><a
                  href="https://www.adobe.com/id_en/products/photoshop/landpa.html?gclid=CjwKCAjww8mWBhABEiwAl6-2RbvRXc_yAigCnLQDKOz87atCrSsw1PFQs0ZXOXWPPr_A20Ro9AfJ1BoC8kgQAvD_BwE&sdid=85665QDS&mv=search&ef_id=CjwKCAjww8mWBhABEiwAl6-2RbvRXc_yAigCnLQDKOz87atCrSsw1PFQs0ZXOXWPPr_A20Ro9AfJ1BoC8kgQAvD_BwE:G:s&s_kwcid=AL!3085!3!444512448900!e!!g!!adobe%20photoshop!703952628!38400836578"
                  target="_blank"
                  >Photoshop</a
                ></small
              >
              <br />
              <small
                ><a
                  href="https://www.adobe.com/id_en/products/illustrator.html?gclid=CjwKCAjww8mWBhABEiwAl6-2RQWImRykutZz-_XX5Y0AjNGYf8b35Vw2VPiwE_PjOFejj0QpHnwj3xoCLrQQAvD_BwE&sdid=81G55V4T&mv=search&ef_id=CjwKCAjww8mWBhABEiwAl6-2RQWImRykutZz-_XX5Y0AjNGYf8b35Vw2VPiwE_PjOFejj0QpHnwj3xoCLrQQAvD_BwE:G:s&s_kwcid=AL!3085!3!472466910439!e!!g!!adobe%20illustrator!11350284429!111298123836"
                  target="_blank"
                  >Illustrator</a
                ></small
              >
              <br />
              <small><a href="https://www.coreldraw.com/en/" target="_blank">Coreldraw</a></small>
            </div>
            <div class="link-title">
              <h4>Find Us</h4>
              <small><a href="https://www.facebook.com/PiandTech-107452205198144"> Facebook </a></small>
              <br />
              <small><a href="https://www.instagram.com/phi.and.tech/">Instagram</a></small>
            </div>
            <div class="link-title">
              <h4>Free Asset</h4>
              <small><a href="https://www.freepik.com/">Freepik</a></small
              ><br />
              <small><a href="https://www.flaticon.com/">Flaticon</a></small>
            </div>
          </div>
        </div>
        <div class="footer-right-col">
          <div class="footer-logo">
            <img src="../src/assets/img/logo-piandtech.png" />
          </div>
        </div>
      </div>
    </section>
  </footer>
</template>

<!-- <style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style> -->
