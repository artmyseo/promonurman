<template>
  <div class="section" id="carousel">
    <div class="container">
      <div class="title">
        <h4>Фото</h4>
      </div>
      <div class="row justify-content-center">
        <div class="col-8">
          <el-carousel height="250px">
            <el-carousel-item>
              <img class="d-block" src="img/gallery/10127-WA0007.jpg" alt="First slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Дробилка</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="img/gallery/20180817_110208.jpg" alt="Second slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Отжим</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="img/gallery/20181123_120150.jpg" alt="Third slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Универсальная мойка</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="img/gallery/20190805_180147.jpg" alt="4 slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Грохот</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="img/gallery/IMG_5346.jpg" alt="4 slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Мойка</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="img/gallery/IMG_5349.jpg" alt="4 slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Ванна флотации</h5>
              </div>
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="img/gallery/IMG_5353.jpg" alt="4 slide" />
              <div class="carousel-caption d-none d-md-block">
                <h5>Отжим</h5>
              </div>
            </el-carousel-item>
          </el-carousel>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Carousel, CarouselItem } from 'element-ui';

export default {
  components: {
    [Carousel.name]: Carousel,
    [CarouselItem.name]: CarouselItem
  }
};
</script>
<style></style>
