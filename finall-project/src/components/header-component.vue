<template >
  <div id="home">
    <div id="header">
      <div id="menu">
        <h1>balala Shop</h1>
        <button>หน้าหลัก</button>
        <button>เริ่มขายของ</button>
        <button>ติดต่อ</button>
        <button>เข้าสู่ระบบ</button>
        <button>สมัคร</button>
      </div>
      <div id="serach">
        <input type="text" />
        <img src="../assets/1.png" width="38" height="37" />
        <img
          src="../assets/2.png"
          width="38"
          height="37"
          style="margin-left: 25px"
        />
      </div>
    </div>
    
  </div>
</template>

<script>

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
/* ----------------------All---------------- */
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
  overflow-x: hidden;
}
/* ------------------------------------------ */
/* ----------------------MENU---------------- */
#header {
  
  border-radius: 30px;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 100%),
    rgba(27, 0, 85, 0.75);
  width: 1505px;
  height: 150px;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  padding: 23px 60px 23px 60px;
  margin-top: 20px;
  margin-right: 60px;
}
#menu {
  display: flex;
  overflow: hidden;
  gap: 63px;
}
#menu button {
  border-radius: 125.5px;
  width: 144px;
  height: 45px;
  border: 2px solid #fff;
  background: rgba(255, 248, 248, 0);
  box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  color: #fff;
  text-align: center;
  font-family: Inter;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  text-decoration-line: underline;
  cursor: pointer;
}
#menu h1 {
  width: 360px;
  height: 68px;
  color: #fff;
  font-family: Holtwood One SC;
  font-size: 45px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  cursor: pointer;
}
#serach {
  display: flex;
}
#serach input {
  width: 570px;
  height: 37px;
}
/* ----------------------HOME---------------- */
/* ------------------------------------------ */
#home {
  width: 2000px;
  /* 1440 */
  height: auto;
  background: #3d4380;
  /* box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25); */
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
}

</style>
