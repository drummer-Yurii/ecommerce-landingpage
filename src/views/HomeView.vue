<template>
  <div>
    <Banner />
    <CategoryProducts :tabs="womenTabs" :title="womenTitle" :products="womenProducts" />
    <CategoryProducts :tabs="womenTabs" :title="menTitle" :products="womenProducts" />
    <Featured />
  </div>
</template>

<script setup>
import Banner from '../components/Banner.vue';
import CategoryProducts from '../components/CategoryProducts.vue';
import Featured from '../components/Featured.vue';
import { ref } from 'vue';

const womenTabs = ref([
  'NEW ARRIVALS',
  'SPECIALS',
  'BESTSELLERS',
  'MOST VIEWED',
  'FEATURED PRODUCTS',
]);

const womenProducts = ref([
  {
    img: '@/assets/images/p1.jpg',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p2.png',
    sale: true,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p3.png',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p2.png',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p3.png',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p1.jpg',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p3.png',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
  {
    img: '@/assets/images/p2.png',
    sale: false,
    name: `Women's tracksuit Q109`,
    price: '$ 38.00',
    rating: '@/assets/images/rating.png',
  },
]);

const womenTitle = ref('Womens');
const menTitle = ref('Men');
</script>