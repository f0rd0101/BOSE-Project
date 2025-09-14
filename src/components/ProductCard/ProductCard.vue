<script  setup lang="ts">
import { defineProps } from 'vue';
const props = defineProps({
    img:String,
    title:String,
    category:String,
    price:String,
})

</script>
<template >
 <li class="product-li">
            <img :src="props.img" alt="product-1" class="img-product" />
            <h3 class="h3-rec">{{ props.title }}</h3>
            <p class="p1-rec">{{ props.category }}</p>
            <p class="p2-rec">{{ props.price }}</p>
          </li>
</template>

<style scoped>
.product-li {
  box-shadow: 0px 1px 6px rgba(46, 47, 66, 0.08),
    0px 1px 1px rgba(46, 47, 66, 0.16), 0px 2px 1px rgba(46, 47, 66, 0.08);
  transition: transform 0.3s, box-shadow 0.3s;
  display: flex;
  align-items: center;
  flex-direction: column;
}
.product-li:hover {
  transform: scale(1.04);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}
.img-product {
  width: 100%;
}
.h3-rec {
  color: #292929;

  font-family: Inter;
  font-size: 16px;
  font-style: normal;
  font-weight: 700;
  letter-spacing: 140%;
  margin: 0;
  margin-top: 32px;
}
.p1-rec {
  color: #292929;

  font-family: Inter;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 140%;
  margin: 0;
  margin-top: 8px;
}
 .p2-rec {
    color: #292929;

    font-family: Inter;
    font-size: 16px;
    font-style: normal;
    font-weight: 700;
    line-height: 140%;
    margin: 0;
    margin-top: 12px;
  }

  .h3-rec {
  color: #292929;
  text-align: center;
  font-family: Inter;
  font-size: 16px;
  font-style: normal;
  font-weight: 700;
  letter-spacing: 0.14em;
  margin: 0;
  margin-top: 32px;


}
.product-li {
        width: 300px;
  }





</style>