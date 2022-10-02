<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <router-link v-popover:popover1 class="navbar-brand" to="/">
        <img
                  src="img/logo.png"
                  alt="logo"
                  class="rounded img-fluid"
                />
      </router-link>
      <el-popover
        ref="popover1"
        popper-class="popover"
        placement="bottom"
        width="200"
        trigger="hover"
      >
        <div class="popover-body">
          Перейти на основной сайт компании <a href="https://nur-man.ru/" class="btn btn-primary btn-sm">Перейти</a>
        </div>
      </el-popover>
    </template>
    <template slot="navbar-menu">
      <li class="nav-item">
        <a
          class="nav-link"
          href="https://nur-man.ru/catalog/agregatyi/"
          target="_blank"
        >
          <i class="now-ui-icons arrows-1_cloud-download-93"></i>
          <p>Оборудование</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          href="https://nur-man.ru/linii-dlya-pererabotki/"
          target="_blank"
        >
          <i class="now-ui-icons arrows-1_cloud-download-93"></i>
          <p>Линии</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          href="https://nur-man.ru/biznes-plan/"
          target="_blank"
        >
          <i class="now-ui-icons arrows-1_cloud-download-93"></i>
          <p>Бизнес-план</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link btn btn-neutral"
          href="https://www.creative-tim.com/product/vue-now-ui-kit-pro"
          target="_blank"
        >
          <i class="now-ui-icons arrows-1_share-66"></i>
          <p>На основной сайт</p>
        </a>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Наш канал на Youtube"
          data-placement="bottom"
          href="https://www.youtube.com/channel/UCO8Sehs5YTrHTMypxa3AJhQ/videos"
          target="_blank"
        >
          <i class="fab fa-youtube"></i>
          <p class="d-lg-none d-xl-none">Youtube</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Наша группа Вконтакте"
          data-placement="bottom"
          href="https://vk.com/nurmanplastik"
          target="_blank"
        >
          <i class="fab fa-vk"></i>
          <p class="d-lg-none d-xl-none">VK</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Наша страница в Instagram"
          data-placement="bottom"
          href="https://www.instagram.com/nurman_equipment/"
          target="_blank"
        >
          <i class="fab fa-instagram"></i>
          <p class="d-lg-none d-xl-none">Instagram</p>
        </a>
      </li>
    </template>
  </navbar>
</template>

<script>
import { DropDown, Navbar, NavLink } from '@/components';
import { Popover } from 'element-ui';
export default {
  name: 'main-navbar',
  props: {
    transparent: Boolean,
    colorOnScroll: Number
  },
  components: {
    Navbar,
    [Popover.name]: Popover
  }
};
</script>

<style scoped></style>
