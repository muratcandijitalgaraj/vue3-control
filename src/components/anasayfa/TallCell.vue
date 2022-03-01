<template>
  <div class="tallCell">
    <div class="logoBox">
      <img src="../../assets/anasayfa/odeme.svg" alt="" class="logo" />
    </div>
    <div class="container d-flex flex-column justify-content-center">
      <div class="row colContainer">
        <!-- first box -->
        <div
          class="col-xs-12 col-sm-12 col-md-12 col-lg-12 col-xl-3 box firstBox d-flex flex-column justify-content-center align-items-start"
        >
          <div class="row colTitle orangeTitle">Ödeme Bekleniyor</div>
          <div class="row colPara">20 Ocak Pazartesi - 12:30</div>
        </div>

        <!-- second box -->
        <div
          class="col-xs-12 col-sm-12 col-md-12 col-lg-12 col-xl-4 box secondBox d-flex flex-row justify-content-start align-items-center"
        >
          <img src="../../assets/anasayfa/doktor.svg" alt="" class="doktor" />
          <div>
            <div class="row doktorTitle colTitle">
              Prof. Dr. Mehmet Ali Tahaoğlu
            </div>
            <div class="row colPara">Gögüs Hastalıkları</div>
          </div>
        </div>
        <!-- third box -->
        <div
          class="col-xs-12 col-sm-12 col-md-12 col-lg-12 col-xl-5 box thirdBox d-flex flex-row justify-content-xl-center justify-content-start align-items-center"
        >
          <div class="greyBox">
            <img
              src="../../assets/anasayfa/video.svg"
              alt=""
              class="greyLogo"
            />
          </div>
          <div>
            <div class="row thirdBoxTitle colTitle">
              Görüntülü Görüşme Randevusu
            </div>
          </div>
        </div>
        <!-- third box ends -->
      </div>
      <!-- first row ends -->
      <div class="row greyLineRow">
        <div class="greyLine col-12"></div>
      </div>
      <!-- grey line row ends -->

      <div class="row bottomPartRow">
        <div class="col-12 col-md-6 bottomPara d-flex align-items-center">
          Ödemenizi yaptığınızda randevunuz aktif hale gelecektir.
        </div>
        <div
          class="col-12 col-md-6 buttonContainer d-flex justify-content-md-end justify-content-start"
        >
          <button class="bottomButton">
            <div class="buttonPara">241 TL Ödeme Yapın</div>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tallCell {
  display: flex;
  margin-left: 12px;
  background: #ffffff;
  /* Boxx Shadow */
  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  margin-bottom: 20px;
  margin-top: 20px;
  height: 180px;
}

.container {
  margin: 0 !important;
  padding: 0 !important;
  height: auto;
}
.colContainer {
  height: auto !important;
}
.row {
  height: 100%;
}
.col-xs-12 {
  height: 100% !important;
}
.box {
  height: 100%;
}
.firstBox {
  padding-left: 2rem;
}
.colTitle {
  width: auto;
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
.orangeTitle {
  color: #ff8038;
}
.thirdBox {
}
.thirdBoxTitle {
  width: 148px;
  height: auto;
}
.colPara {
  width: 171px;
  height: 21px;
  /* text3 */
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
.doktor {
  width: 50px;
  height: 50px;
  margin-right: 1.5rem;
}
.logoBox {
  width: 40px;
  height: 170px;
  background: #fff9f0;
  border-radius: 5px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin-right: 20px;
  align-self: center;
  margin-left: 5px;
}
.logo {
  height: 20px;
  width: 20px;
  /* margin-left: 1rem; */
  border-radius: 0px;
  margin: 0;
}
.greyBox {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f2f8fb;
  border-radius: 5px;
  margin-right: 1.5rem;
  /* this padding makes sure that the logo fits well */
  padding: 10px;
}
.greyLogo {
  width: 22px;
  height: 22px;
  margin-right: 1rem;
}
.greyLineRow {
  /* align-items: center; */
  height: auto !important;
  display: flex;
  justify-content: center;
  margin: 0 !important;
  padding: 0 !important;
  margin-right: 2% !important;
}
.greyLine {
  height: 1px !important;
  width: 95% !important;
  background: #dae9f1;
  margin-top: 20px;
  margin-bottom: 15px;
}
.bottomPartRow {
  height: auto;
}

.bottomButton {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 250px !important;
  height: 40px !important;

  /* Button Primary */

  background: #ff7c32;
  border: none;

  border-radius: 6px;
}
.bottomPara {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */
  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
  padding-left: 1.2rem;
}
.buttonPara {
  /* buton-text-kucuk */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 110%;
  /* identical to box height, or 17px */

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
.buttonContainer {
  height: 43px !important;
  padding-right: 5%;
}
@media (max-width: 1400px) {
  .doktorTitle {
    margin-bottom: 1.3rem;
  }
}
@media (max-width: 1200px) {
  .tallCell {
    flex-direction: column;
    height: 100%;
  }
  .logoBox {
    width: 100%;
    height: auto;
    padding: 10px;
    margin: 0;
  }
  .box {
    margin-left: 2rem;
    margin-bottom: 2rem;
  }
  .doktorTitle {
    margin-bottom: 0;
  }
  .firstBox {
    /* margin-left: 5.5rem; */
  }
  .bottomPartRow {
    padding-left: 2rem;
  }
  .bottomPara,
  .buttonContainer {
    margin-bottom: 2rem;
  }
}
@media (max-width: 1000px) {
}

/* @media (max-width: 768px) {
  .buttonContainer {
    display: flex;
    justify-content: center;
    border: solid;
  }
} */
</style>
