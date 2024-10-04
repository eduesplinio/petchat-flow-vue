<template>
  <div class="carrossel">
    <swiper
      :modules="modules"
      :slides-per-view="1"
      :space-between="50"
      navigation
      :pagination="{ clickable: true }"
      :autoplay="{ delay: 3000, disableOnInteraction: false }"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide v-for="slide in slides" :key="slide.id">
        <img :src="slide.imagem" :alt="slide.titulo" />
        <div class="slide-content">
          <h2>{{ slide.titulo }}</h2>
          <p>{{ slide.descricao }}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, Pagination, Autoplay } from "swiper/modules";

// Importação das imagens
import carrossel1 from "@/assets/carrossel1.png";
import carrossel2 from "@/assets/carrossel2.png";
import carrossel3 from "@/assets/carrossel3.png";

import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";

export default {
  name: "CarrosselView",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      modules: [Navigation, Pagination, Autoplay],
      slides: [
        {
          id: 1,
          imagem: carrossel1,
          titulo: "Bem-vindo ao Petshop!",
          descricao: "Encontre os melhores cuidados e produtos para o seu pet",
        },
        {
          id: 2,
          titulo: "Promoção de Rações",
          descricao: "Até 30% de desconto em rações premium",
          imagem: carrossel2,
        },
        {
          id: 3,
          titulo: "Serviço de Banho e Tosa",
          descricao: "Agende agora e ganhe 10% de desconto",
          imagem: carrossel3,
        },
      ],
    };
  },
  methods: {
    onSwiper(swiper) {
      console.log(swiper);
    },
    onSlideChange() {
      console.log("slide change");
    },
  },
};
</script>

<style>
.carrossel {
  margin-bottom: 1rem;
  width: 100vw;
  position: relative;
  left: 50%;
  transform: translateX(-50%);
}

.swiper {
  width: 100%;
  height: 450px;
}

.swiper-slide {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 100%;
  height: 100%;
}

.swiper-slide img {
  width: 100%;
  height: 100%;
}

.slide-content {
  position: absolute;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  width: 80%;
}
</style>
