<template>
  <div id="footerBackGorund">
    <div id="footer">
      <h1>balala shop</h1>
      <p>
        เว็บไซต์นี้จัดทำขึ้นเพื่อเป็นโครงการจบสำหรับนิสิตปริญญาตรีเพื่อที่จะสนับสนุนชุมชนในการขายสินค้าหรือซื้อสินค้าของชุมชนออนไลน์
      </p>
      <div id="footer-icon">
        <font-awesome-icon class="icongoogle" :icon="['fab', 'google']" />
        <font-awesome-icon class="iconfacebook" :icon="['fab', 'facebook']" />
      </div>
    </div>
  </div>
</template>

<script>
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { library } from "@fortawesome/fontawesome-svg-core";
import { faGoogle, faFacebook } from "@fortawesome/free-brands-svg-icons";

library.add(faGoogle, faFacebook);

export default {
  components: {
    FontAwesomeIcon,
  },
};
</script>

<style>
#footerBackGorund {
  height: 180px;
  display: flex;
  width: 2000px;
  flex-direction: column;
  align-items: center;
  background-color: #3d4380;
  /* background-color: #168f20; */
  padding-right: 60px;
}
#footer {
  height: 180px;
  display: flex;
  width: 1505px;
  flex-direction: column;
  align-items: center;
  background-color: rgb(255, 255, 255);
  gap: 20px;
  padding-top: 20px;
}

#footer-icon {
  display: flex;
  gap: 20px;
}
.icongoogle {
  width: 35px;
  height: 35px;
  color: rgb(233, 18, 18);
}
.iconfacebook {
  width: 35px;
  height: 35px;
  color: rgb(28, 53, 165);
}
</style>