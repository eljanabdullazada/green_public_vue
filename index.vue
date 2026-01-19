<template>
  <div class="frame">
    <div class="group">
      <div class="sirvan-salyan">
        <img
          class="sirvan-salyan-2"
          alt="Sirvan salyan"
          :src="sirvanSalyan"
        />
      </div>
    </div>

    <RegionQazaxTovuz
      class="region-qazax-tovuz-state-default"
      img="vector-18-2.svg"
      mapClassName="region-qazax-tovuz-instance"
      qazaxTovuz="image.svg"
      qazaxTovuzClassName="region-qazax-tovuz-state-default-instance"
      vector="vector-17-2.svg"
    />
    <RegionGNcDaKSN
      class="region-g-nc-da-k-s-n-state-default"
      gNcDaKSNClassName="region-g-nc-da-k-s-n-state-default-instance"
      gNcDashkSN="g-nc-dashk-s-n-2.svg"
      gNcDashkSNClassName="region-g-nc-da-k-s-n-instance"
    />
    <RegionQarabaState
      class="region-qaraba-state-default"
      divClassName="region-qaraba-state-default-instance"
      qarabag="qarabag-2.svg"
      qarabagClassName="region-qaraba-state-instance"
    />
    <RegionQubaXaMaz
      class="region-quba-xa-maz-state-default"
      divClassName="region-quba-xa-maz-state-default-instance"
      qubaXachmaz="quba-xachmaz-2.svg"
      qubaXachmazClassName="region-quba-xa-maz-instance"
    />
    <RegionAbEronXZ
      aBsheron="a-bsheron-2.svg"
      aBsheronClassName="region-ab-eron-x-z-instance"
      abEronXZClassName="region-ab-eron-x-z-state-default-instance"
      class="region-ab-eron-x-z-state-default"
    />
    <div class="map-2">
      <div class="baki-wrapper">
        <img class="img-2" alt="Baki" :src="baki" />
      </div>

      <div class="div-wrapper">
        <div class="text-wrapper-4">Bakı</div>
      </div>
    </div>

    <div class="map-3">
      <img
        class="sirvan-salyan-3"
        alt="Sirvan salyan"
        :src="sirvanSalyan2"
      />

      <img
        class="sirvan-salyan-4"
        alt="Sirvan salyan"
        :src="sirvanSalyan3"
      />

      <div class="text-wrapper-5">Şirvan - Salyan</div>
    </div>

    <RegionRqiZNgZur
      class="region-rqi-z-ng-zur-state-default"
      rqiZNgZurClassName="region-rqi-z-ng-zur-state-default-instance"
      zengezur="zengezur-2.svg"
      zengezurClassName="region-rqi-z-ng-zur-instance"
    />
    <div class="map-4">
      <div class="m-aran-wrapper">
        <img class="m-aran" alt="M aran" :src="mAran" />
      </div>

      <div class="map-5">
        <div class="text-wrapper-6">Mərkəzi Aran</div>
      </div>
    </div>

    <div class="map-6">
      <img class="mil-m" alt="Mil m" :src="milM" />

      <div class="text-wrapper-7">Mil - Muğan</div>
    </div>

    <div class="map-7">
      <div class="daglig-shirvan-wrapper">
        <img class="img-2" alt="Daglig shirvan" :src="dagligShirvan" />
      </div>

      <div class="map-8">
        <div class="text-wrapper-8">Dağlıq Şirvan</div>
      </div>
    </div>

    <RegionKiZaqatala
      class="region-ki-zaqatala-state-default"
      divClassName="region-ki-zaqatala-state-default-instance"
      shekiZaqatala="sheki-zaqatala-2.svg"
      shekiZaqatalaClassName="region-ki-zaqatala-instance"
    />
    <div class="map-9">
      <div class="l-nk-ran-astara">
        Lənkəran - <br />
        Astara
      </div>

      <img class="lenkaran" alt="Lenkaran" :src="lenkaran" />

      <div class="l-nk-ran-astara">
        Lənkəran - <br />
        Astara
      </div>

      <img class="lenkeran" alt="Lenkeran" :src="lenkeran" />
    </div>

    <div class="map-10">
      <img class="vector-2" alt="Vector" :src="vector26" />

      <div class="text-wrapper-9">Naxçıvan</div>
    </div>
  </div>
</template>

<script>
import RegionAbEronXZ from "./RegionAbEronXZ";
import RegionGNcDaKSN from "./RegionGNcDaKSN";
import RegionKiZaqatala from "./RegionKiZaqatala";
import RegionQarabaState from "./RegionQarabaState";
import RegionQazaxTovuz from "./RegionQazaxTovuz";
import RegionQubaXaMaz from "./RegionQubaXaMaz";
import RegionRqiZNgZur from "./RegionRqiZNgZur";
import baki from "./baki.svg";
import dagligShirvan from "./daglig-shirvan.svg";
import lenkaran from "./lenkaran.svg";
import lenkeran from "./lenkeran.svg";
import mAran from "./m-aran.svg";
import milM from "./mil-m.svg";
import sirvanSalyan2 from "./sirvan-salyan-2.svg";
import sirvanSalyan3 from "./sirvan-salyan-3.svg";
import sirvanSalyan from "./sirvan-salyan.svg";
import vector26 from "./vector-26.svg";

export default {
  name: "Frame",
  components: {
    RegionAbEronXZ,
    RegionGNcDaKSN,
    RegionKiZaqatala,
    RegionQarabaState,
    RegionQazaxTovuz,
    RegionQubaXaMaz,
    RegionRqiZNgZur,
  },
  data() {
    return {
      baki,
      dagligShirvan,
      lenkaran,
      lenkeran,
      mAran,
      milM,
      sirvanSalyan2,
      sirvanSalyan3,
      sirvanSalyan,
      vector26,
    };
  },
};
</script>

<style>
.frame {
  height: 473px;
  position: relative;
  width: 580px;
}

.frame .group {
  display: flex;
  height: 184px;
  left: 330px;
  position: absolute;
  top: 208px;
  width: 149px;
}

.frame .sirvan-salyan {
  display: flex;
  height: 183.99px;
  margin-left: 0;
  margin-top: 0;
  width: 148.74px;
}

.frame .sirvan-salyan-2 {
  height: 9.1px;
  margin-left: 119.1px;
  margin-top: 175.0px;
  width: 6.8px;
}

.frame .region-qazax-tovuz-state-default {
  height: 214px !important;
  left: -181px !important;
  position: absolute !important;
  top: 1px !important;
  width: 341px !important;
}

.frame .region-qazax-tovuz-instance {
  margin-left: 58.84% !important;
  margin-right: -0.0% !important;
  width: 140.19px !important;
}

.frame .region-qazax-tovuz-state-default-instance {
  font-size: 13px !important;
  height: 25.69% !important;
  left: 50.42% !important;
  line-height: 19.6px !important;
  top: 41.98% !important;
  width: 35.67% !important;
}

.frame .region-g-nc-da-k-s-n-state-default {
  height: 233px !important;
  left: -156px !important;
  position: absolute !important;
  top: -12px !important;
  width: 382px !important;
}

.frame .region-g-nc-da-k-s-n-instance {
  height: 131px !important;
  left: 263px !important;
  top: 103px !important;
  width: 119px !important;
}

.frame .region-g-nc-da-k-s-n-state-default-instance {
  font-size: 13px !important;
  height: 17.16% !important;
  left: 75.92% !important;
  line-height: 19.6px !important;
  top: 75.05% !important;
  width: 16.77% !important;
}

.frame .region-qaraba-state-default {
  height: 313px !important;
  left: 173px !important;
  position: absolute !important;
  top: 179px !important;
  width: 142px !important;
}

.frame .region-qaraba-state-instance {
  height: 162px !important;
  width: 137px !important;
}

.frame .region-qaraba-state-default-instance {
  font-size: 13px !important;
  height: 6.38% !important;
  line-height: 19.6px !important;
  top: 25.17% !important;
  width: 38.10% !important;
}

.frame .region-quba-xa-maz-state-default {
  height: 133px !important;
  left: 311px !important;
  position: absolute !important;
  top: 6px !important;
  width: 429px !important;
}

.frame .region-quba-xa-maz-instance {
  height: 134px !important;
  top: 0 !important;
  width: 164px !important;
}

.frame .region-quba-xa-maz-state-default-instance {
  font-size: 13px !important;
  height: 15.01% !important;
  left: 6.61% !important;
  line-height: 19.6px !important;
  top: 52.45% !important;
  width: 22.86% !important;
}

.frame .region-ab-eron-x-z-state-default {
  height: 147px !important;
  left: 413px !important;
  position: absolute !important;
  top: 114px !important;
  width: 327px !important;
}

.frame .region-ab-eron-x-z-instance {
  height: 137px !important;
  top: 10px !important;
  width: 116px !important;
}

.frame .region-ab-eron-x-z-state-default-instance {
  font-size: 13px !important;
  height: 27.25% !important;
  line-height: 19.6px !important;
  top: 15.41% !important;
  width: 20.51% !important;
}

.frame .map-2 {
  height: 186px;
  left: 467px;
  position: absolute;
  top: 114px;
  width: 273px;
}

.frame .baki-wrapper {
  height: 125px;
  left: 0;
  position: absolute;
  top: 61px;
  width: 113px;
}

.frame .img-2 {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}

.frame .div-wrapper {
  height: 20px;
  left: 58px;
  position: absolute;
  top: 72px;
  width: 28px;
}

.frame .text-wrapper-4 {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 102.30%;
  justify-content: center;
  left: 2.94%;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: -5.11%;
  white-space: nowrap;
  width: 97.48%;
}

.frame .map-3 {
  height: 184px;
  left: 331px;
  position: absolute;
  top: 209px;
  width: 409px;
}

.frame .sirvan-salyan-3 {
  height: 9px;
  left: 119px;
  position: absolute;
  top: 175px;
  width: 7px;
}

.frame .sirvan-salyan-4 {
  height: 166px;
  left: -1px;
  position: absolute;
  top: -1px;
  width: 150px;
}

.frame .text-wrapper-5 {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 10.86%;
  justify-content: center;
  left: 8.92%;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: 56.54%;
  white-space: nowrap;
  width: 22.99%;
}

.frame .region-rqi-z-ng-zur-state-default {
  height: 192px !important;
  left: -160px !important;
  position: absolute !important;
  top: 213px !important;
  width: 416px !important;
}

.frame .region-rqi-z-ng-zur-instance {
  height: 193px !important;
  left: 243px !important;
  width: 173px !important;
}

.frame .region-rqi-z-ng-zur-state-default-instance {
  font-size: 13px !important;
  height: 20.85% !important;
  left: 65.71% !important;
  line-height: 19.6px !important;
  top: 13.49% !important;
  width: 13.93% !important;
}

.frame .map-4 {
  height: 204px;
  left: 203px;
  position: absolute;
  top: 46px;
  width: 462px;
}

.frame .m-aran-wrapper {
  height: 125px;
  left: 0;
  position: absolute;
  top: 79px;
  width: 178px;
}

.frame .m-aran {
  height: 100.00%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}

.frame .map-5 {
  height: 20px;
  left: 86px;
  position: absolute;
  top: 160px;
  width: 81px;
}

.frame .text-wrapper-6 {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 102.30%;
  justify-content: center;
  left: 0;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: -5.11%;
  white-space: nowrap;
  width: 100.66%;
}

.frame .map-6 {
  height: 260px;
  left: 182px;
  position: absolute;
  top: 234px;
  width: 253px;
}

.frame .mil-m {
  height: 82px;
  left: 93px;
  position: absolute;
  top: -1px;
  width: 160px;
}

.frame .text-wrapper-7 {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 7.70%;
  justify-content: center;
  left: 55.81%;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: 11.22%;
  white-space: nowrap;
  width: 29.70%;
}

.frame .map-7 {
  height: 172px;
  left: 305px;
  position: absolute;
  top: 46px;
  width: 360px;
}

.frame .daglig-shirvan-wrapper {
  height: 107px;
  left: 0;
  position: absolute;
  top: 65px;
  width: 157px;
}

.frame .map-8 {
  height: 20px;
  left: 38px;
  position: absolute;
  top: 115px;
  width: 84px;
}

.frame .text-wrapper-8 {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 102.30%;
  justify-content: center;
  left: 0;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: -5.11%;
  white-space: nowrap;
  width: 97.73%;
}

.frame .region-ki-zaqatala-state-default {
  height: 174px !important;
  left: -174px !important;
  position: absolute !important;
  top: -7px !important;
  width: 510px !important;
}

.frame .region-ki-zaqatala-instance {
  height: 169px !important;
  left: 318px !important;
  top: 6px !important;
  width: 193px !important;
}

.frame .region-ki-zaqatala-state-default-instance {
  font-size: 13px !important;
  height: 11.50% !important;
  line-height: 19.6px !important;
  top: 64.08% !important;
  width: 18.62% !important;
}

.frame .map-9 {
  height: 140px;
  left: 332px;
  position: absolute;
  top: 333px;
  width: 350px;
}

.frame .l-nk-ran-astara {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 28.65%;
  justify-content: center;
  left: 4.60%;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: 44.80%;
  width: 20.57%;
}

.frame .lenkaran {
  height: 141px;
  left: -1px;
  position: absolute;
  top: -1px;
  width: 130px;
}

.frame .lenkeran {
  height: 9px;
  left: 110px;
  position: absolute;
  top: 53px;
  width: 11px;
}

.frame .map-10 {
  height: 151px;
  left: -196px;
  position: absolute;
  top: 259px;
  width: 337px;
}

.frame .vector-2 {
  height: 125px;
  left: 196px;
  position: absolute;
  top: 27px;
  width: 142px;
}

.frame .text-wrapper-9 {
  align-items: center;
  color: var(--gray-200);
  display: flex;
  font-family: "DM Sans-SemiBold", Helvetica;
  font-size: 13px;
  font-weight: 600;
  height: 13.28%;
  justify-content: center;
  left: 71.91%;
  letter-spacing: 0;
  line-height: 19.6px;
  position: absolute;
  text-align: center;
  top: 53.96%;
  white-space: nowrap;
  width: 17.19%;
}
</style>