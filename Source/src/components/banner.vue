<template>
  <div class="shadow-lg ">
  <swiper
    :slidesPerView="'auto'"
    :spaceBetween="30"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    :autoplay="{
      delay: 5000, // Delay between transitions in milliseconds
      disableOnInteraction: false, // Prevents autoplay from stopping when user interacts with swiper
    }"
    class="mySwiper"
  >
    <swiper-slide>
      <section
        class="relative bg-[url('./assets/anh.png')] bg-cover bg-center bg-no-repeat "
      >
        <div
          class="absolute inset-0 bg-white/20"
        ></div>

        <div
          class="relative mx-auto max-w-screen-xl px-4 py-32 sm:px-6 lg:flex lg:h-screen lg:items-center lg:px-8"
        >
          <div class="max-w-xl  ltr:sm:text-left rtl:sm:text-right text-white">
            <h1 class="text-3xl font-extrabold sm:text-5xl">
              MODS BÀN PHÍM CƠ

              <strong class="block font-extrabold ">
                AnhPhimCo
              </strong>
            </h1>

            <p class="mt-4 max-w-lg sm:text-xl/relaxed">
              AnhPhimCo với đội ngũ mods chuyên nghiệp luôn mong muốn mang đến trải nghiệm mods phím tuyệt vời và đúng gu của khách hàng nhất có thể !!!
            </p>

            <div class="mt-8 flex flex-wrap gap-4 ">
              <a
                href="https://www.facebook.com/profile.php?id=100004474787150"
                class="block w-full rounded bg-gray-600 px-12 py-3 text-sm font-medium text-white shadow hover:bg-gray-700 focus:outline-none focus:ring active:bg-rose-500 sm:w-auto"
              >
                Liên hệ ngay
              </a>
            </div>
          </div>
        </div>
      </section>
    </swiper-slide>

    <swiper-slide>
      <section
        class="relative  bg-[url('./assets/anh2.png')] bg-cover bg-center bg-no-repeat "
      >
        <div
          class="absolute inset-0 bg-white/20 "
        ></div>

        <div
          class="relative mx-auto max-w-screen-xl px-4 py-32 sm:px-6 lg:flex lg:h-screen lg:items-center lg:px-8"
        >
          <div class="max-w-xl  ltr:sm:text-left rtl:sm:text-right text-white">
            <h1 class="text-3xl font-extrabold sm:text-5xl">
              MODS BÀN PHÍM CƠ

              <strong class="block font-extrabold ">
                AnhPhimCo
              </strong>
            </h1>

            <p class="mt-4 max-w-lg sm:text-xl/relaxed">
              Mang đến trải nghiệm tuyệt vời, tận tâm vì nghề. Bạn hài lòng là niểm vui của chúng tôi.
            </p>

            <div class="mt-8 flex flex-wrap gap-4 ">
              <a
                href="https://www.facebook.com/profile.php?id=100004474787150"
                class="block w-full rounded bg-gray-600 px-12 py-3 text-sm font-medium text-white shadow hover:bg-gray-700 focus:outline-none focus:ring active:bg-gray-500 sm:w-auto"
              >
                Liên hệ ngay
              </a>
            </div>
          </div>
        </div>
      </section>
    </swiper-slide>

  </swiper>
</div>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";
// Import Swiper styles
import "swiper/css";
import "swiper/css/pagination";

import { Pagination, Autoplay } from "swiper/modules";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination, Autoplay], // Import Autoplay module
    };
  },
};
</script>
