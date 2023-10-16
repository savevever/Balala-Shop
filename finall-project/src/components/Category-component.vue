<template >
  <div id="Category">
    <div id="Category-container">
      <div class="Category-title">
        <button @click="showCommunityButtons" >
          ชุมชน
        </button>
        <button @click="showCategoryButtons" >
          หมวดหมู่
        </button>
      </div>
      <div
        style="
          width: 1505px;
          height: 3px;
          background-color: rgba(2, 0, 121, 0.7);
          margin-top: 20px;
          margin-right: 60px;
        "
      ></div>
      <div id="Category-item">
        <div v-if="showButtons">
          <button v-for="button in buttons" :key="button.id">
            {{ button.name }}
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showButtons: false,
      buttons: [],
    };
  },
  methods: {
    showCommunityButtons() {
      this.showButtons = true;
      this.buttons = [
        { id: 1, name: "ชุมชน 1" },
        { id: 2, name: "ชุมชน 2" },
        { id: 3, name: "ชุมชน 3" },
        { id: 4, name: "ชุมชน 4" },
        { id: 5, name: "ชุมชน 5" },
      ];
    },
    showCategoryButtons() {
      this.showButtons = true;
      this.buttons = [
        { id: 1, name: "หมวดหมู่ 1" },
        { id: 2, name: "หมวดหมู่ 2" },
        { id: 3, name: "หมวดหมู่ 3" },
        { id: 4, name: "หมวดหมู่ 4" },
        { id: 5, name: "หมวดหมู่ 5" },
      ];
    },
  },
  created() {
    // เริ่มต้นแสดง "ชุมชน" เมื่อคอมโพเนนต์ถูกสร้าง
    this.showCommunityButtons();
  },
};
</script>
<style >
/* ------------------------------------------ */
/* ----------------------Category---------------- */
#Category {
  width: 2000px;
  margin: 50px 0 50px 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
.Category-title button{
  color: #fff;
  text-align: center;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  text-decoration-line: underline;
  margin-left: 40px;
  background-color: #3d4380;
  border: none;
  cursor: pointer;
}

#Category-item {
  display: flex;
  flex-direction: column;
}
#Category-item button {
  border-radius: 125.5px;
  background: #d3bfff;
  box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  width: 121px;
  height: 36px;
  margin-right: 20px;
  margin-top: 20px;
  border: 0px;
}
</style>
