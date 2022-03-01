<template>
  <div class="cellComponent">
    <div class="logoBox">
      <img src="../../assets/anasayfa/gorusme.svg" alt="" class="logo" />
    </div>
    <div class="container">
      <div class="row colContainer">
        <!-- first box -->
        <div
          class="col-xs-12 col-sm-12 col-md-12 col-lg-12 col-xl-3 box firstBox d-flex flex-column justify-content-center align-items-start"
        >
          <div class="row colTitle redTitle">Görüşme Bekleniyor</div>
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
              src="../../assets/anasayfa/hospital.svg"
              alt=""
              class="greyLogo"
            />
          </div>
          <div>
            <div class="row colTitle">Ataşehir Tıp Merkezi</div>
            <div class="row colPara">Ataşehir Tıp Merkezi</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.cellComponent {
  display: flex;
  margin-left: 12px;
  background: #ffffff;
  /* Boxx Shadow */
  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  margin-bottom: 20px;
  margin-top: 20px;
  height: 110px;
}
.container {
  margin: 0 !important;
  padding: 0 !important;
}
.colContainer {
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
.redTitle {
  color: #ea5455;
}
.colPara {
  width: auto;
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
  height: 100px;
  background: #ffeeee;
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
@media (max-width: 1400px) {
  .doktorTitle {
    margin-bottom: 1.3rem;
  }
}
@media (max-width: 1200px) {
  .cellComponent {
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
}
@media (max-width: 1000px) {
}
</style>
