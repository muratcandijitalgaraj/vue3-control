<template>
  <div class="anasayfaComponent">
    <img src="../assets/anasayfa/bulutlar.svg" alt="" class="bulutlar" />

    <div class="container">
      <div class="row header">
        <Header />
      </div>

      <div class="row sideBarTopRow">
        <div class="col sideBarTop">
          <SideBarTop class="sideBarTop" />
        </div>
      </div>

      <div class="row greyPart">
        <div class="col-3 sideBar">
          <SideBar />
        </div>

        <div class="col rightPart">
          <div class="row cards">
            <div class="col">
              <Cards />
            </div>
          </div>

          <div class="row texts">
            <div class="col title">Randevularınız</div>
            <div class="col para">Hepsini Göster</div>
          </div>

          <div class="row randevular">
            <div class="col">
              <Randevulariniz />
            </div>
          </div>

          <div class="row texts">
            <div class="col title">Son Muayeneler</div>
            <div class="col para">Hepsini Göster</div>
          </div>

          <div class="row muayeneler">
            <div class="col">
              <Muayeneler />
            </div>
          </div>
        </div>
        <div class="row footer">
          <Footer />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/* eslint-disable vue/no-unused-components */
import Header from "../components/anasayfa/Header.vue";
import SideBar from "../components/anasayfa/SideBar.vue";
import SideBarTop from "../components/anasayfa/SideBarTop.vue";

import Cards from "../components/anasayfa/Cards.vue";
import Randevulariniz from "../components/anasayfa/Randevulariniz.vue";
import Muayeneler from "../components/anasayfa/Muayeneler.vue";
import Footer from "../components/shared/Footer.vue";

export default {
  components: {
    Header,
    SideBar,
    SideBarTop,
    Cards,
    Randevulariniz,
    Muayeneler,
    Footer,
  },
};
</script>

<style scoped>
.anasayfaComponent {
  width: 100%;
  height: auto;
  /* Secondary */

  background: #32a5df;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  display: flex;
  flex-direction: column;
  margin: 0;
  padding: 0;
}
.container {
  z-index: 1;
}
.bulutlar {
  position: fixed;
  width: 100%;
  height: auto;
  top: 7rem;
  z-index: 0;
}
.anasayfa {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  z-index: 60;
}
.header {
  width: auto;
  height: auto;
  background: #32a5df;
  margin-bottom: 25px;
}
.cards {
  min-height: 140px;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
}
.randevular {
  height: auto;
}
.muayeneler {
  height: auto;
}
.texts {
  height: auto;
  width: auto;
  display: flex;
  justify-content: space-between;
  /* padding-left: 1rem;
  padding-right: 2rem; */
  margin-left: 10px;
  margin-right: 10px;
}
.title {
  width: auto;
  height: auto;

  /* baslik3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 130%;
  /* identical to box height, or 29px */

  /* Secondary */

  color: #32a5df;
}
.para {
  width: auto;
  height: auto;

  /* text4-bold */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 130%;
  /* identical to box height, or 17px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
.footer {
  height: 200px;
  width: auto;
}

/* .bulutlar {
  margin-top: 10rem;
  position: absolute;

  height: auto;
  width: 100%;
} */
.container {
}
.greyPart {
  min-height: 1018px;
  height: 100%;
  width: auto;
  background: #f2f8fb;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.15);
  border-radius: 18px;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
}
.sideBar {
  background: #f9fdff;
  border-radius: 18px 0px 0px 18px;
  height: auto;
}
.rightPart {
  height: auto;
}

.sideBarTopRow {
  display: none;
  width: auto;
}
.sideBarTop {
}
@media screen and (max-width: 992px) {
  .sideBar {
    display: none;
  }
  .sideBarTopRow {
    display: block !important;
    width: auto;
    padding: 0;
  }
  .sideBarTop {
    display: block !important;
    width: auto;
    padding: 0;
    border-bottom-left-radius: 0;
    border-top-left-radius: 18px;
    border-top-right-radius: 18px;
  }
  .greyPart {
    border-radius: 0px;
  }
  .bulutlar {
    top: 12rem;
  }
}
@media (max-width: 576px) {
  .texts {
    flex-direction: column;
    align-items: center;
  }
  .title {
    margin-bottom: 1rem;
  }
}
@media (min-width: 576px) {
  .para {
    text-align: right;
  }
}
</style>
