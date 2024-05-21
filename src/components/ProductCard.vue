<template>
  <q-page-container>
    <q-page>
      <div class="row q-col-gutter-md q-mt-md">
        <q-card
          v-for="product in products"
          :key="product.id"
          class="col-xs-12 col-sm-6 col-md-4"
        >
          <q-img :src="product.image" />
          <q-card-section>
            <div class="text-h6">{{ product.name }}</div>
            <div>{{ product.price }}</div>
          </q-card-section>
        </q-card>
      </div>
    </q-page>
  </q-page-container>
</template>

<script>
export default {
  name: "ProductCard",
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Cpu Gacorr",
          price: "Rp10.000.000",
          image:
            "https://images-na.ssl-images-amazon.com/images/I/91kXZN089WL.jpg",
        },
        {
          id: 2,
          name: "Monitor Menyala",
          price: "Rp5.000.000",
          image:
            "https://www.notebookcheck.net/fileadmin/Notebooks/News/_nc3/ROG_Swift_OLED_PG48UQ___L.jpg",
        },
        {
          id: 3,
          name: "Mouse Keren",
          price: "Rp1.000.000",
          image:
            "https://luckyretail.com/Uploadfile/202003202/358168/358168-2.jpg",
        },
      ],
    };
  },
};
</script>
