<template>
  <div id="app">
    <div class="title">
      <div class="left">
        <p>Sketch</p>
        <Icon type="ios-wifi" />
      </div>
      <div class="center">
        <span>9:00AM</span>
      </div>
      <div class="right">
        <p>100%</p>
        <Icon type="ios-battery-full" />
      </div>
    </div>
    <div class="list">
      <div class="header">
        <p>
          <span><a href="#"><</a></span>  
          <span>列表</span>
          <span>
            <Icon type="ios-cart-outline" />
          </span>
        </p>
      </div>
      <div class="content">
        <div class="nav">
          <div class="left">
            <Dropdown>          
                默认排序
                <Icon type="ios-arrow-down"></Icon>
              <DropdownMenu slot="list">
                <DropdownItem>驴打滚</DropdownItem>
                <DropdownItem>炸酱面</DropdownItem>
                <DropdownItem disabled>豆汁儿</DropdownItem>
                <DropdownItem>冰糖葫芦</DropdownItem>
                <DropdownItem divided>北京烤鸭</DropdownItem>
              </DropdownMenu>
            </Dropdown>
          </div>
           <div class="right">
            <Dropdown>          
                筛选
                <Icon type="ios-arrow-down"></Icon>
              <DropdownMenu slot="list">
                <DropdownItem>驴打滚</DropdownItem>
                <DropdownItem>炸酱面</DropdownItem>
                <DropdownItem disabled>豆汁儿</DropdownItem>
                <DropdownItem>冰糖葫芦</DropdownItem>
                <DropdownItem divided>北京烤鸭</DropdownItem>
              </DropdownMenu>
            </Dropdown>
            <Icon type="ios-list" style="fontSize:30px; color:#dc4150"/>
          </div>
        </div>
        <div class="content-list">
          <ul>
            <li>
              <div class="img">
                <!-- <img src="../images/列表大显_13.jpg" alt=""> -->
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app {
  padding: 10px;
}
a {
  list-style: none;
}
.title {
  overflow: hidden;
  padding-bottom: 10px;
}
.title p {
  font-size: 14px;
}
.title .left {
  float: left;
  width: 30%;
}
.title .left p {
  float: left;
  margin-right: 5px;
}
.title .center {
  width: 40%;
  text-align: center;
  float: left;
}
.title .right {
  float: right;
}
.title .right p {
  float: left;
}
.list .header {
  font-size: 16px;
  overflow: hidden;
  padding-bottom: 10px;
}
.list .header p {
  position: relative;
  height: 30px;
  line-height: 30px;
}
.list .header span:first-child {
  margin-left: 5px;
  float: left;
  width: 30%;
  font-size: 25px;
}
.list .header span:nth-of-type(2) {
  width: 40%;
  text-align: center;
  float: left;
}
.list .header span:last-child {
  float: right;
  margin-right: 7px;
  font-size: 20px;
}
.list .header p::after {
  content: "";
  display: block;
  width: 100%;
  border: 1px solid #f1f0f0;
  position: absolute;
  bottom: -10px;
}
.content .nav {
  padding: 10px 0 0 10px;
font-size: 16px;
}
.content .nav .left {
  float: left;
}
.content .nav .right {
  float: right;
}
/* .content .nav .right  */
.content .nav .right .ivu-dropdown {
  margin-right: 20px;
}
/* .content .nav i:last-child{
  font-size: 20px;
  color: red;
} */
</style>
