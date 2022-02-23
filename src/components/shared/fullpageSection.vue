<template>
  <div class="fullpage-section">
    <img src="../../assets/images/lenovo_logo.svg" class="lenovo-logo">
    <div class="container-flex">
      <div class="row">
        <div class="col leftCol">
          <h1 class="header">Yoga S740 (14)</h1>
          <h1 class="sub-header">Wyrozniajaca inteligencja</h1>
          <p class="description">
            Z komputerem Yoga S740 możesz pracować i korzystać z rozrywki w eleganckim stylu.
            Ten imponujący laptop w całkowicie metalowej obudowie działa z pełną mocą procesora Intel® Core™ 10.
            generacji i oferuje inteligentne, przydatne na co dzień funkcje. Lekki, ale wydajny, zapewnia wysokiej
            klasy funkcje rozrywkowe dzięki baterii wystarczającej na nawet 15 godzin, efektownemu wyświetlaczowi 4K
            VESA400 HDR oraz fantastycznemu dźwiękowi z technologią Dolby Atmos®.
          </p>
        </div>
        <div class="col rightCol">
          <img src="../../assets/images/laptop_1.png">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "fullpageSection.vue"
}
</script>

<style scoped>
  @font-face {
    font-family: 'Gotham-Book';
    src: url(../../assets/fonts/Gotham-Book.ttf);
  }
  .fullpage-section {
    height: 796px;
    width: 100%;
    background-color: #408DDC;
    position: relative;
  }
  .lenovo-logo {
    position: absolute;
    top: 0;
    left: 0;
  }
  .container-flex .row {
    display: flex;
    max-width: 1321px;
    width: 100%;
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    transform: translateY(25%);
  }
  .header {
    font-family: 'Gotham-Book';
    color: white;
    font-size: 50px;
    line-height: 56px;
    text-align: left;
    margin-bottom: 0;
  }
  .sub-header {
    color: white;
    font-family: 'Gotham-Book';
    margin-top: 0;
  }
  .description {
    color: white;
    font-family: 'Gotham-Book';
  }
  @media (max-width: 688px) {
    .lenovo-logo {
      display: none;
    }
    .container-flex .row {
      display: block;
      max-width: 90%;
      transform: translateY(9vw);
    }
    .header {
      margin-top: 0;
      font-size: 8vw;
    }
    .sub-header {
      margin-top: 0;
      font-size: 6vw;
    }
    .col img {
      display: block;
      width: 90%;
      margin: 0 auto;
    }
  }
  @media (min-width: 689px) and (max-width: 992px) {
    .container-flex .row {
      display: block;
      max-width: 60%;
      transform: translateY(9vw);
    }
    .header {
      margin-top: 0;
      font-size: 6vw;
    }
    .sub-header {
      margin-top: 0;
      font-size: 3vw;
    }
    .col img {
      display: block;
      width: 90%;
      margin: 0 auto;
    }
  }
  @media (min-width: 993px) and (max-width: 1320px) {
    .container-flex .row {
      max-width: 90%;
      transform: translateY(23vw);
    }
    .col img {
      display: block;
      width: 90%;
      margin: 0 auto;
    }
    .col.leftCol {
      width: 50%;
    }
    .col.rightCol {
      width: 50%;
    }
  }
</style>
