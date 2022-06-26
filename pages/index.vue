<template>


  <section>
    <div class="header p-2">
      <nav class="
            navbar navbar-expand-lg navbar-white
            shadow
            p-3
            mb-5
            bg-white
            rounded
          ">
        <div class="container-fluid">
          <a class="navbar-brand" href="#"> Imam Firmansyah </a>
          <button class="navbar-toggler bg-warning" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon align-middle">
              <h5>👽</h5>
            </span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link" aria-current="page" href="#home">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#about-us">About Us</a>
              </li>
              <li class="nav-item me-5">
                <a class="nav-link btn btn-warning" href="#contact">Contact Us</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </div>

    <div class="p-5" id="home">
      <div class="row">
        <div class="text-start px-5 pt-5 mt-5">
          <h2>
            <span class="bg-warning p-1"> Hallo</span>, Saya Imam
            <span class="text-warning"> Firmansyah ✌️ </span>
          </h2>
          <h4>Student & Techinical Support</h4>
        </div>
      </div>
    </div>

    <div class="container fluid">
      <div class="row">
        <div class="col col-12 col-md-4 col-lg-4">
          <div class="shadow bg-white">
            <img src="/images/ciremai.jpg" class="px-4 pt-3" width="100% " alt=" " />
            <div class="text-label px-4 py-2">
              <span> Haii </span>
              <h5>Ini Foto di Gunung Ciremai</h5>
            </div>
          </div>
        </div>

        <div class="col col-12 col-md-4 col-lg-4">
          <div class="shadow bg-white">
            <img src="/images/talaga biru.JPG" class="px-4 pt-3" width="100% " alt=" " />
            <div class="text-label px-4 py-2">
              <span> Haii </span>
              <h5>Ini Foto di Talaga Biru</h5>
            </div>
          </div>
        </div>

        <div class="col col-12 col-md-4 col-lg-4">
          <div class="shadow bg-white">
            <img src="/images/guntur.jpg" class="px-4 pt-3" width="100% " alt=" " />
            <div class="text-label px-4 py-2">
              <span> Haii </span>
              <h5>Ini Foto di Gunung Guntur</h5>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container mt-4">
      <client-only>
        <b-carousel id="carousel-1" v-model="slide" :interval="4000" controls indicators background="#ababab"
          img-width="1024" img-height="480" style="text-shadow: 1px 1px 2px #333;" @sliding-start="onSlideStart"
          @sliding-end="onSlideEnd">
          <!-- Text slides with image -->
          <b-carousel-slide caption="First slide" text="Nulla vitae elit libero, a pharetra augue mollis interdum."
            img-src="https://picsum.photos/1024/480/?image=52"></b-carousel-slide>

          <!-- Slides with custom text -->
          <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=54">
            <h1>Hello world!</h1>
          </b-carousel-slide>

          <!-- Slides with image only -->
          <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58"></b-carousel-slide>

          <!-- Slides with img slot -->
          <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->

          <!-- Slide with blank fluid image to maintain slide aspect ratio -->
        </b-carousel>
      </client-only>
    </div>


    <!-- about us -->
    <div class="container pt-5" id="about-us">
      <div class="shadow p-3 mb-5 bg-white rounded">
        <div class="row">
          <div class="col col-12 col-md-4 col-lg-3">
            <img src="/images/imam.jpg" class="py-2" width="100%" alt=" ">
          </div>
          <div class="col col-12 col-md-8 col-lg-9">
            <h3 class="mt-3">
              <span class="bg-warning rounded p-2"> Hai </span>
            </h3>
            <p> Perkenalkan nama saya Imam Firmansyah, saya seorang mahasiswa aktif semester 7 di perguruan tinggi STMIK
              LPKIA BANDUNG dan sekarang saya bekerja sebagai Techinical Support di perusahaan danAdaIde Indonesia,
              selain kesibukan saya kuliah
              dan bekerja, saya mengikuti kegiatan keorganisasian dikampus.</p>
            <p> Organisasi yang saya ikutin yaitu : </p>
            <ul>
              <li class="mb-3"> <span class="bg-warning rounded p-1 me-2"> 2019 - 2020 </span> Bascom ( Wakil
                Koordinator Animasi ) </li>
              <li class="mb-3"> <span class="bg-warning rounded p-1 me-2"> 2019 - 2020 </span> Futsal Lpkia ( Wakil
                Ketua ) </li>
              <li class="mb-3"> <span class="bg-warning rounded p-1 me-2"> 2019 - 2020 </span> Futsal Lpkia ( Ketua )
              </li>
              <li class="mb-3"> <span class="bg-warning rounded p-1 me-2"> 2021 - 2022 </span> Himpunan Mahasiswa STMIK
                ( Ketua ) </li>
            </ul>
            <p> Itulah biodata singkat saya </p>
            <p> Terima Kasih ✌️ </p>
          </div>
        </div>
      </div>
    </div>

    <!-- contact us -->
    <div class="container pt-5 " id="contact">
      <div class="shadow p-5 mb-5 bg-white rounded ">
        <form>
          <h1 class="text-center py-2 ">
            <span class="bg-warning p-2 rounded-3 ">
              CONTACT US
            </span>
          </h1>
          <div class="form-group py-2 ">
            <input type="text " class="form-control " placeholder="Your Name " />
          </div>
          <div class="form-group py-2 ">
            <input type="text " class="form-control " placeholder="Your Email " />
          </div>
          <div class="form-group py-2 ">
            <input type="text " class="form-control " placeholder="Subject " />
          </div>
          <div class="form-group py-2 ">
            <textarea name=" " id=" " cols="30 " rows="7 " class="form-control " placeholder="Message "></textarea>
          </div>
          <div class="form-group py-2 ">
            <input type="submit pt-2 " value="Send Message " class="btn btn-warning py-3 px-5 " />
          </div>
        </form>
      </div>
    </div>

    <!-- footer -->
    <div class="row ">
      <div class="col-md-12 pt-2 text-center ">
        <p>
          <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
          Copyright &copy;
          All rights reserved | Imam Firmansyah
          <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    }
  }
}
</script>