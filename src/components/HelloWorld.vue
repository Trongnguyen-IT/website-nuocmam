<template>
  <div class="wrapper">
    <div class="header">
      <!-- Just an image -->
      <nav class="bg-light">
        <a class href="#">
          <img class="logo" src="../assets/logo.png" alt="nuocmamthuongnguon" />
        </a>
      </nav>
    </div>
    <div class="introduce">
      <div class="row">
        <div class="col-4">
          <img class="image-introduce" alt="nuocmamthuongnguon" src="../assets/image-intro.png" />
        </div>
        <div class="col-6">
          <h1 class="title color-title">Giới thiệu chung</h1>
          <p class="text-content">
            Nhận thấy Cá Linh là một trong những đặc sản không thể bỏ qua của miền Tây Nam Bộ vào mùa nước nổi. Thời điểm lũ về cũng là lúc thiên nhiên hào phóng gửi tặng người dân sản vật quí. Trong số đó, Cá Linh là một đặc sản được đặc biệt trông chờ nhất. Hồng ngự là một huyện biên giới của tỉnh Đồng tháp, với nguồn nhiên liệu dồi giàu của thiên nhiên. Cá Linh được người dân vùng sông nước chế biến ra nhiều món ăn hấp dẫn, trong đó có Nước mắm Cá Linh truyền thống, đây là món gia vị không thể thiếu trong buổi cơm hàng ngày của chúng ta.
            Việc thực hiện Dự án sản xuất nước mắm Cá Linh nhằm duy trì nghề làm nước mắm truyền thống của gia đình, cũng như đáp ứng nhu cầu thị trường. Việc sản xuất từ các nguyên liệu sẳn có trong tự nhiên, không sử dụng phẩm màu hay chất bảo quản gây ảnh hưởng sức khỏe người tiêu dùng.
            Để làm được một sản phẩm nước mắm Cá Linh Thơm ngon, an toàn bản thân đã giành nhiều thời gian để học cách làm từ ông bà, cha mẹ, từ các cô chú lớn tuổi đến các cơ sở hiện tại, nhằm tạo ra một sản phẩm ngon, an toàn phù hợp với hương vị quê hương.
          </p>
        </div>
        <div></div>
      </div>
    </div>
    <div class="body">
      <VueSlickCarousel v-bind="settings">
        <div class="column">
          <img class="image-product" alt="Vue logo" src="../assets/image1.jpg" />
        </div>
        <div class="column">
          <img class="image-product" alt="Vue logo" src="../assets/image3.jpg" />
        </div>
        <div class="column">
          <img class="image-product" alt="Vue logo" src="../assets/image2.jpg" />
        </div>
        <div class="column">
          <img class="image-product" alt="Vue logo" src="../assets/image4.jpg" />
        </div>
      </VueSlickCarousel>
    </div>
    <!-- <h1>{{ msg }}</h1> -->
    <!-- <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">babel</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">eslint</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul>-->
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  data: function() {
    return {
      settings: {
        dots: true,
        dotsClass: "slick-dots custom-dot-class",
        edgeFriction: 0.35,
        infinite: false,
        speed: 500,
        slidesToShow: 4,
        slidesToScroll: 1
      }
    };
  },
  components: { VueSlickCarousel },
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.title {
  font-size: 50px;
  color: #b01f24;
  text-align: left;
  margin-bottom: 3rem;
}
.introduce {
  padding: 2rem 6rem;
}
.bg-light {
  padding: 10px 0;
  background-color: rgba(0, 0, 0, 0.6) !important;
}
.wrapper {
  background-image: url("../assets/background.jpg");
}
.column {
  height: 600px;
}
.introduce .text-content {
  color: #000;
  font-size: 1rem;
  text-align: left;
}
.introduce .image-introduce {
  object-fit: contain;
  width: 100%;
  height: auto;
}
.logo {
  max-width: 100px;
}
.body .image-wrap .column {
}
.image-product {
  width: 100%;
  object-fit: contain;
}
</style>
