<template>
  <div class="q-pa-md">
    <q-carousel animated v-model="slide" arrows navigation infinite>
      <q-carousel-slide
        :name="1"
        img-src="https://images-na.ssl-images-amazon.com/images/I/91kXZN089WL.jpg"
      />
      <q-carousel-slide
        :name="2"
        img-src="https://www.notebookcheck.net/fileadmin/Notebooks/News/_nc3/ROG_Swift_OLED_PG48UQ___L.jpg"
      />
      <q-carousel-slide
        :name="3"
        img-src="https://luckyretail.com/Uploadfile/202003202/358168/358168-2.jpg"
      />
    </q-carousel>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      slide: ref(1),
    };
  },
};
</script>
