<script setup lang="ts">
import ProductCard from '../ProductCard/ProductCard.vue'
import product1 from '../../assets/images/product1.png'
import product2 from '../../assets/images/product2.png'
import product3 from '../../assets/images/product3.png'


</script>
<template>
<section class="rec-section" id="recommended">
        <h2 class="rec-h2">Recommended</h2>
        <ul class="product-ul">
            <ProductCard 
                :img = "product1"
                title = "Bose portable Smart speaker"
                category = "Smart home"
                price = "$ 399.00"
                />
            <ProductCard 
                :img = "product2"
                title = "Bose portable Smart speaker"
                category = "Smart home"
                price = "$ 399.00"
                />
            <ProductCard 
                :img = "product3"
                title = "SoundLink Color Bluetooth speaker II"
                category = "Portable bluetooth"
                price = "$ 129.00"
                />
        </ul>
      </section>    
</template>

<style scoped>
.rec-section {
    padding: 120px;
    flex-direction: column;
}
.rec-h2 {
  color: #292929;
  text-align: center;
  font-family: Inter;
  font-size: 35px;
  font-style: normal;
  font-weight: 700;
  line-height: 1em; /* 100% */
  letter-spacing: -0.03125em;
  margin: 0;
  margin-bottom: 64px;
}
.product-ul {
    display: flex;
    gap: 24px;
    justify-content: center;
    margin: 0;
    flex-direction: row;
}
@media screen and (min-width: 472px) {
  .rec-section {
    padding: 0 20px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
   .product-ul :nth-child(-n + 3) {
    display: flex;
    align-items: center;
  }
  .product-ul{
     flex-direction: column;
  }
}

@media screen and (min-width: 1260px) {
 .rec-section {
    padding: 120px;
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
 .product-ul{
     flex-direction: row;
  }
}





</style>