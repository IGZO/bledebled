<template>
  <section class="categorie-area">
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <!-- Section Title -->
          <div class="section-title mt-res-sx-30px mt-res-md-30px">
            <h2>Catégories populaires</h2>
          </div>
          <!-- Section Title -->
        </div>
      </div>
      <!-- Category Slider Start -->
      <div class="category-slider owl-carousel owl-nav-style">
        <div v-for="cat in categories" :key="cat" class="category-item">
          <div class="category-list mb-30px">
            <div class="category-thumb">
              <a :href="cat.link">
                <img :src="cat.img" alt="" />
              </a>
            </div>
            <div class="desc-listcategoreis">
              <div class="name_categories">
                <h4
                  style="
                    color: white;
                    padding: 5px 5px;
                    text-align: center;
                    border-radius: 5px;
                    text-align: center;
                    background-color: black;
                  "
                >
                  {{ cat.name }}
                </h4>
              </div>
              <span
                style="
                  color: black;
                  padding: 5px 5px;
                  text-align: center;
                  font-size: 10px;
                  border-radius: 5px;
                  text-align: center;
                  background-color: white;
                "
                class="number_product"
              >
                {{ cat.count }} Produits
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Caategories",
  data() {
    return {
      categories: [
        {
          link: "/shop?cat=couscous",
          img: "assets/images/product-image/organic/couscous.jpg",
          name: "couscous",
          //count: 17,
        },
        {
          link: "/shop?cat=Avoine",
          img: "assets/images/product-image/organic/avoine.jpg",
          name: "Avoine",
          //count: 17,
        },
        {
          link: "/shop?cat=Hssoua",
          img: "assets/images/product-image/organic/hssoua.jpg",
          name: "Hssoua",
          //count: 17,
        },
        {
          link: "/shop?cat=zemita",
          img: "assets/images/product-image/organic/zemita.jpg",
          name: "Zemita",
          //count: 17,
        },
        {
          link: "/shop?cat=Blé",
          img: "assets/images/product-image/organic/ble.jpg",
          name: "Blé",
          //count: 17,
        },
        {
          link: "/shop?cat=farine",
          img: "assets/images/product-image/organic/farine.jpg",
          name: "farine",
          //count: 17,
        },
        {
          link: "/shop?cat=dchicha",
          img: "assets/images/product-image/organic/dchicha.jpg",
          name: "dchicha",
          //count: 17,
        },
        {
          link: "/shop?cat=berkoukech",
          img: "assets/images/product-image/organic/berkoukch.jpg",
          name: "berkoukech",
          //count: 17,
        },
      ],
    };
  },
};
</script>
