<template>
  <div class="randevuDetay">
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
          <!-- start here -->
          <div class="container">
            <div class="row topPart">
              <div class="col bigTitle">Randevu Detayı</div>
              <div
                class="col geri d-flex justify-content-end align-items-center"
              >
                <span class="sign">
                  <!-- &lt; -->
                  <img
                    class="sign"
                    src="../assets/randevular/sign.svg"
                    alt=""
                  />
                </span>

                Geri Dön
              </div>
            </div>
            <!-- row ends -->
            <div class="row">
              <div class="greyLine"></div>
            </div>
            <div class="row whiteSpace">
              <div class="container">
                <div class="row">
                  <div
                    class="col-12 d-flex justify-content-start align-items-center informativeCard"
                  >
                    <img
                      src="../assets/randevular/calendar.svg"
                      alt=""
                      class="logo"
                    />
                    <div class="redTitle">Görüşme Bekleniyor...</div>
                  </div>
                  <!-- col -->
                  <div
                    class="col-12 doktorCard d-flex align-items-center justify-content-start"
                  >
                    <img
                      src="../assets/randevular/doktor.svg"
                      alt=""
                      class="doktor"
                    />
                    <div
                      class="d-flex flex-column align-items-start justify-content-center"
                    >
                      <div class="doktorTitle">
                        Prof. Dr. Mehmet Ali Tahaoğlu
                      </div>
                      <div class="para">Göğüs Hastalıkları</div>
                    </div>
                  </div>
                  <!-- col -->
                  <div
                    class="col-12 greyCard d-flex flex-column flex-sm-column flex-md-row align-items-sm-start align-items-md-center"
                  >
                    <div
                      class="redDoktorContainer col col-sm-12 col-md-3 d-flex align-items-center"
                    >
                      <img
                        src="../assets/randevular/note.svg"
                        alt=""
                        class="logo"
                      />
                      <div class="doktorNote">Doktorun Notu</div>
                    </div>

                    <div class="col col-sm-12 col-md-3 para">
                      Lütfen muayeneye aç karnına gelin.
                    </div>
                  </div>
                  <div class="greyLine"></div>

                  <!-- col -->
                  <div
                    class="col cards d-flex flex-row align-items-center justify-content-start"
                  >
                    <img
                      src="../assets/randevular/kim.svg"
                      alt=""
                      class="cardLogo"
                    />
                    <div
                      class="cardTexts d-flex flex-column justify-content-center"
                    >
                      <div class="cardTitle">Kim için</div>
                      <div class="cardPara">Mehmet Balkan</div>
                    </div>
                  </div>
                  <div class="greyLine"></div>
                  <!-- col -->
                  <div
                    class="col cards d-flex flex-row align-items-center justify-content-start"
                  >
                    <img
                      src="../assets/randevular/tarih.svg"
                      alt=""
                      class="cardLogo"
                    />
                    <div
                      class="cardTexts d-flex flex-column justify-content-center"
                    >
                      <div class="cardTitle">Tarih</div>
                      <div class="cardPara">
                        14 Ağustos 2020 - Pazartesi 15:30
                      </div>
                    </div>
                  </div>
                  <div class="greyLine"></div>
                  <!-- col -->
                  <div
                    class="col cards d-flex flex-row align-items-center justify-content-start"
                  >
                    <img
                      src="../assets/randevular/randevu.svg"
                      alt=""
                      class="cardLogo"
                    />
                    <div
                      class="cardTexts d-flex flex-column justify-content-center"
                    >
                      <div class="cardTitle">Randevu Türü</div>
                      <div class="cardPara">Ataşehir Tıp Merkezi</div>
                    </div>
                  </div>
                  <div class="greyLine"></div>
                  <!-- col -->
                  <div
                    class="col cards d-flex flex-row align-items-center justify-content-start"
                  >
                    <img
                      src="../assets/randevular/sikayet.svg"
                      alt=""
                      class="cardLogo"
                    />
                    <div
                      class="cardTexts d-flex flex-column justify-content-center"
                    >
                      <div class="cardTitle">Şikayet</div>
                      <div class="cardPara">
                        Gögüs boşlugumda ara ara ağrılar hissediyorum. Lorem
                        ipsum dolor sit amet, consectetur adipiscing elit, sed
                        do eiusmod tempor incididunt ut labore et dolore magna
                        aliqua. Ut enim ad minim veniam, quis nostrud
                        exercitation ullamco laboris nisi ut aliquip ex ea
                        commodo
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- right part col ends -->
      </div>
      <div class="row footer">
        <Footer />
      </div>
    </div>
  </div>
</template>

<script>
/* eslint-disable vue/no-unused-components */
import Header from "../components/anasayfa/Header.vue";
import SideBar from "../components/anasayfa/SideBar.vue";
import SideBarTop from "../components/anasayfa/SideBarTop.vue";
import Top from "../components/randevularim/Top.vue";

import Footer from "../components/shared/Footer.vue";

export default {
  components: {
    Header,
    SideBar,
    SideBarTop,
    Top,
    Footer,
  },
};
</script>

<style scoped>
.col {
  /* border: solid; */
}
.randevuDetay {
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
/* page specific styling starts here */
.topPart {
  margin-top: 1.5rem;
}
.bigTitle {
  width: 162px;
  height: 29px;
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 130%;
  /* identical to box height, or 29px */
  /* Primary */
  color: #3c4e69;
}
.geri {
  width: 59px;
  height: 21px;
  /* text3 */
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 140%;
  /* identical to box height, or 21px */
  letter-spacing: -0.01em;
  /* Gri */
  color: #818b9a;
}
.sign {
  width: auto;
  height: auto;
  /* font-size: 1.5rem;
  font-weight: 900;
  color: #818b9a; */
  margin-right: 5px;
  padding-bottom: 1px;
}
.greyLine {
  height: 1px;
  width: 100%;
  background: #dae9f1;
  margin: 1.5rem 0 1rem 0;
}
.whiteSpace {
  width: auto;
  height: auto;
  background: white;
  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  padding: 1rem;
}

.informativeCard {
  width: 100%;
  height: 50px;
  background: #ffeeee;
  border-radius: 5px;
}
.redTitle {
  margin-left: 12px;
  width: 159px;
  height: 24px;
  /* baslik4 */
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */
  /* Kırmızı */
  color: #ea5455;
}
.doktorCard {
  margin-top: 22px;
}
.doktor {
  margin-right: 17px;
}
.doktorTitle {
  width: 225px;
  height: 24px;

  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */

  /* Primary */

  color: #3c4e69;
}
.para {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */
  letter-spacing: -0.01em;

  /* Primary */

  color: #3c4e69;
}
.greyCard {
  background: #fafafa;
  border-radius: 5px;
  min-height: 50px;
  height: auto;
  margin-top: 1rem;
}
.doktorNote {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;

  /* Kırmızı */

  color: #ea5455;
  margin-left: 8px;
}
.redDoktorContainer {
  width: auto;
  margin-right: 20px;
}
.cardLogo {
  margin-right: 1rem;
}
.cardTitle {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
.cardPara {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */

  /* Primary */

  color: #3c4e69;
}
/* page specific styling ends here */
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

.footer {
  height: 200px;
  width: auto;
}

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
/* @media (min-width: 576px) {
  .para {
    text-align: right;
  }
} */
</style>
