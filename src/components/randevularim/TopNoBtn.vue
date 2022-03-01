<template>
  <div class="randevularimTop">
    <div class="row container">
      <!-- column -->
      <div
        class="col-12 columns col-sm-6 col-md-3 randevularimContainer justify-content-center justify-content-xl-start d-flex align-items-center"
      >
        <div class="randevularimText">Randevularım</div>
      </div>
      <!-- column -->

      <div
        class="col-12 columns col-sm-6 col-md-3 yerindeContainer d-flex flex-column justify-content-center align-items-center"
      >
        <div class="yerindeRandevular">Yerinde Randevular</div>
        <div class="selectedTab"></div>
      </div>
      <!-- column -->

      <div
        class="col-12 columns col-sm-6 col-md-3 goruntuluContainer d-flex justify-content-center justify-content-xl-start align-items-center"
      >
        <div class="goruntulu">Görüntülü Görüşme</div>
      </div>
      <!-- column -->

      <div class="buttonContainer">
        <button class="button">
          <div class="buttonText">Yeni Randevu Alın</div>
        </button>
      </div>
    </div>
    <!-- row ends -->
    <div class="row d-flex justify-content-center">
      <div class="greyLine"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.columns {
  margin-bottom: 10px;
}
.randevularimTop {
  padding-top: 15px;
}
.randevularimContainer {
}
.randevularimText {
  width: auto;
  height: auto;

  /* baslik3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 130%;
  /* identical to box height, or 29px */

  /* Primary */

  color: #3c4e69;
  margin-left: 1rem;
}
.yerindeContainer {
}
.yerindeRandevular {
  width: auto;

  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */

  /* Secondary */

  color: #32a5df;
}
.goruntuluContainer {
}
.goruntulu {
  width: auto;

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
.button {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 167px;
  height: 40px;

  /* Button Primary */

  background: #ff7c32;
  border: none;
  border-radius: 6px;
}
.buttonText {
  width: 127px;
  height: 17px;

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
.selectedTab {
  position: relative;
  top: 1rem;
  width: 25px;
  height: 5px;
  background: #32a5df;
  border-radius: 4px 4px 0px 0px;
}
.greyLine {
  border: 1px solid #dae9f1;
  width: 90%;
}
.buttonContainer {
  display: none;
  border: solid;
}
@media only screen and (max-width: 1200px) {
  .selectedTab {
    display: none;
  }
}
</style>
