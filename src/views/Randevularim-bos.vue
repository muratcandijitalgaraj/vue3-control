<template>
  <div class="randevularimBos">
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
          <div class="row cards">
            <div class="col">
              <Top />
            </div>
          </div>
          <div class="col d-flex justify-content-center aling-items-center">
            <img
              src="../assets/randevular/randevularim-bos/bulutlar.svg"
              alt=""
              class="bulutlarBos"
            />
            <div
              class="flexContainer d-flex flex-column justify-content-center aling-items-center"
            >
              <img
                src="../assets/randevular/randevularim-bos/calendar.svg"
                alt=""
                class="bigLogo"
              />
              <div class="bigTitle d-flex justify-content-center">
                Randevunuz bulunmuyor.
              </div>
              <div class="titleBlue d-flex justify-content-center">
                Randevu almak için aşağıdaki butonu kullabilirsiniz
              </div>
              <div class="d-flex justify-content-center">
                <button class="button">
                  <div class="buttonText">Yeni Randevu Alın</div>
                </button>
              </div>
            </div>
          </div>
        </div>
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
import Top from "../components/randevularim/TopNoBtn.vue";

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
.randevularimBos {
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
/* component specific style starts */
.bigLogo {
  width: auto;
  height: 120px;
  margin-bottom: 30px;
}
.bulutlarBos {
  position: absolute;
  top: 15rem;

  z-index: 0;
}
.flexContainer {
  z-index: 1;
  height: auto !important;
  margin-top: 15%;
  margin-bottom: 15%;
}
.bigTitle {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 26px;
  line-height: 130%;
  /* identical to box height, or 34px */

  letter-spacing: -0.01em;

  /* Primary */

  color: #3c4e69;
  margin-bottom: 13px;
}
.titleBlue {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 130%;
  /* or 26px */

  text-align: center;
  letter-spacing: -0.01em;

  /* Secondary */

  color: #32a5df;
  margin-bottom: 23px;
}

.button {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 20px 40px;

  width: 235px;
  height: 60px;

  /* Button Primary */

  background: #ff7c32;
  border: none;
  border-radius: 6px;
}
.buttonText {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 18px;
  line-height: 110%;
  /* identical to box height, or 20px */

  display: flex;
  align-items: center;
  text-align: center;

  /* Beyaz */

  color: #ffffff;

  /* Inside auto layout */

  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 10px;
}

/* component ends */
.bulutlar {
  position: fixed;
  width: 100%;
  height: auto;
  top: 7rem;
  z-index: 0;
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
  height: auto;
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
@media only screen and (max-width: 1200px) {
  .bulutlarBos {
    top: 15.5rem;
    width: 700px;
  }
}

@media screen and (max-width: 992px) {
  /* do this so that there won't be a white space at the bottom of the page */
  .greyPart {
    min-height: 418px;
    height: 100%;
  }
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
  .bulutlarBos {
    top: 26rem;
    width: 600px;
  }
}
@media (max-width: 900px) {
  .bulutlarBos {
    top: 32rem;
    width: 500px;
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
