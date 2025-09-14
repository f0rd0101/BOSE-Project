<script>
</script>
<template>
     <section id="products" class="product-section">
        <h2 class="h2-prod">
          Browse Bose<br />
          products by category
        </h2>
        <ul class="ul-prod">
          <li class="li-prod">
            <img
              src="../../assets/images/person1.jpg"
              alt="girl with earbuds"
              class="img-product"
            />
            <p class="p-prod">Headphones & earbuds</p>
          </li>
          <li class="li-prod">
            <img
              src="../../assets/images/person2.jpg"
              alt="girl in headphones"
              class="img-product"
            />
          </li>
        </ul>
        <ul class="ul-prod">
          <li class="li-prod">
            <img
              src="../../assets/images/person3.jpg"
              alt="light-blue BOSE speaker"
              class="img-product"
            />
            <p class="p-prod">Speakers</p>
          </li>
          <li class="li-prod">
            <img
              src="../../assets/images/person4.jpg"
              alt="aquamarine BOSE speaker"
              class="img-product"
            />
          </li>
        </ul>
        <ul class="ul-prod">
          <li class="li-prod">
            <img
              src="../../assets/images/person5.jpg"
              alt="light-blue BOSE man"
              class="img-product"
            />
            <p class="p-prod">Audio sunglasses</p>
          </li>
          <li class="li-prod">
            <img     src="../../assets/images/person6.jpg" alt="aquamarine BOSE speaker" />
          </li>
        </ul>
      </section>
</template>
<style scoped>
.product-section {
    padding: 120px;
  }
  .h2-prod {
    margin: 0;
    color: #292929;
    text-align: center;
    font-family: Inter;
    font-size: 48px;
    font-style: normal;
    font-weight: 700;
    line-height: 1em;
    letter-spacing: -0.03125em;
  }
  .ul-prod {
    display: flex;
    gap: 24px;
    justify-content: center;
    margin: 0;
    margin-top: 64px;
  }

  .p-prod {
    color: #292929;
    font-family: Inter;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: 140%; /* 33.6px */
    margin: 0;
    margin-top: 16px;
  }
</style>