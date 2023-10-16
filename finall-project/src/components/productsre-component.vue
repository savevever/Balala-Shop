<template>
  <div class="products">
    <div class="products-container">
      <div v-for="product in products" :key="product.id" class="originalDiv">
        <div class="products-items">
          <img :src="require('@/assets/2.png')" />
          <div>
            <div class="products-items-bottom">
              <p class="products-items-bottom-title">{{ product.title }}</p>
              <div class="price-soldout">
                <p class="price">{{ product.price }}</p>
                <p class="sold-out">ขายแล้ว {{ product.soldCount }} ชิ้น</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="products-container">
      <div v-for="product in products" :key="product.id" class="originalDiv">
        <div class="products-items">
          <img :src="require('@/assets/2.png')" />
          <div>
            <div class="products-items-bottom">
              <p class="products-items-bottom-title">{{ product.title }}</p>
              <div class="price-soldout">
                <p class="price">{{ product.price }}</p>
                <p class="sold-out">ขายแล้ว {{ product.soldCount }} ชิ้น</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [],
      nextId: 1,
    };
  },
  created() {
    for (let i = 0; i < 5; i++) {
      this.products.push({
        id: this.nextId,
        imageSource: "2.png", // ใช้ชื่อไฟล์ "2.png"
        title: "Product Title",
        price: "245฿",
        soldCount: 2450,
      });
      this.nextId++;
    }
  },
};
</script>

<style scoped>
/* ------------------------------------------ */
/* ----------------------toptree-products---------------- */
.products {
  display: flex;
  flex-direction: column;
}
.products-container {
  width: 2000px;
  height: 400px;
  padding-right: 60px;
  background-color: #3d4380;
  display: flex;
  /* justify-content: center; */
  gap: 20px;
  justify-content: center;
}
.products-items {
  display: flex;
  flex-direction: column;
}
.products-items img {
  width: 286px;
  height: 235px;
}
.products-items p {
  width: 286px;
  height: 70px;
  /* background-color: white; */
  text-align: center;
}
.products-items-bottom-title {
  font-size: 20px;
}
.price {
  font-size: 20px;
  color: #b80d0d;
}
.sold-out {
  font-size: 15px;
}

.price-soldout {
  width: 286px;
  height: 40px;
  display: flex;
  /* background-color: white; */
  gap: 30px;
  overflow: hidden;
}
.price-soldout p {
  margin-top: 9px;
}
.products-items-bottom {
  background: #ffffff;
}
/* ------------------------------------------ */
/* ----------------------toptree-products-items---------------- */
</style>






