<template>
  <div class="sideBarTop">
    <div class="row">
      <div class="col-12 d-flex justify-content-center">
        <img src="../../assets/sidebar/foto.svg" alt="" class="foto" />
      </div>
    </div>
    <!-- row ends  -->

    <div class="d-flex justify-content-center">
      <!-- collapse button -->
      <button
        type="button"
        class="btn btn-secondary upperItem collapseButton para d-flex justify-content-center"
        data-bs-toggle="collapse"
        data-bs-target="#collapseExample"
        aria-expanded="false"
        aria-controls="collapseExample"
      >
        Akgül Yılmaz
      </button>
    </div>
    <!-- collapse content -->
    <div class="collapse" id="collapseExample">
      <!-- without this div, the collapse is not hidden initially -->
      <div class="row itemContainer">
        <div class="item d-flex justify-content-center">
          <!-- this itemfix class ensures all the items are aligned vertically -->
          <div class="itemfix">
            <img src="../../assets/sidebar/giris.svg" alt="" class="itemLogo" />
            <div class="itemPara">Giriş</div>
          </div>
        </div>
        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img
              src="../../assets/sidebar/randevularim.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Randevularım</div>
          </div>
        </div>

        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img
              src="../../assets/sidebar/kayitlar.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Tıbbi Kayıtlar</div>
            <img src="../../assets/sidebar/1.svg" alt="" class="notification" />
          </div>
        </div>
        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img
              src="../../assets/sidebar/gecmis.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Geçmiş Muayeneler</div>
          </div>
        </div>
        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img
              src="../../assets/sidebar/receteler.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Reçeteler</div>
          </div>
        </div>
        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img src="../../assets/sidebar/hesap.svg" alt="" class="itemLogo" />
            <div class="itemPara">Hesap Bilgileriniz</div>
          </div>
        </div>
        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img src="../../assets/sidebar/anket.svg" alt="" class="itemLogo" />
            <div class="itemPara">Anketimize Katılın</div>
          </div>
        </div>
        <div class="item d-flex justify-content-center">
          <div class="itemfix">
            <img src="../../assets/sidebar/cikis.svg" alt="" class="itemLogo" />
            <div class="itemPara">Çıkış Yap</div>
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
.sideBarTop {
  background: #f9fdff;
}
.row {
}
.col {
}
.foto {
  height: 116px;
  width: 116px;
  border-radius: 0px;
}
.collapseButton {
  margin-bottom: 1rem;
}
.itemContainer {
}
.item {
  height: auto;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  margin-bottom: 10px;
}
.itemfix {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  width: 200px;
}
.itemLogo {
  width: 30px;
  height: 40px;

  margin-right: 10px;
}
.itemPara {
  width: auto;
  height: 22px;

  /* menu */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 22px;
  /* identical to box height */

  /* Primary */

  color: #3c4e69;
  /* border: 1px solid red; */
}
.notification {
  width: 20px;
  height: 20px;
  margin-left: 5px;
}

/* @media only screen and (max-width: 768px) {
  .itemContainer {
    padding-left: 34%;
  }
}
@media only screen and (max-width: 576px) {
  .itemContainer {
    padding-left: 0;
  }
} */
</style>
