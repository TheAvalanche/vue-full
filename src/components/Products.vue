<template>
  <div class="container">
    <div class="row my-4">
      <div class="col-12">
        <h1>Some products header</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus aliquid animi architecto consectetur dolor dolores, eaque ex hic impedit ipsum non omnis pariatur perspiciatis possimus provident repellendus rerum tempora voluptatibus?</p>
      </div>
      <div class="col-3 my-3" v-for="product in products">
        <div class="card">
          <img class="card-img-top" :src="product.img">
          <div class="card-body">
            <h5 class="card-title">{{ product.title }}</h5>
            <p class="card-text">{{ product.text }}</p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Products',
  data: function () {
    return {
      products: [
        {
          title: 'Test title',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          img: 'http://placeimg.com/300/200/animals'
        }, {
          title: 'Some title',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          img: 'http://placeimg.com/300/200'
        }, {
          title: 'Test product',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          img: 'http://placeimg.com/300/200/nature'
        }, {
          title: 'Some product',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          img: 'http://placeimg.com/300/200/people'
        }, {
          title: 'Test test',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          img: 'http://placeimg.com/300/200/tech'
        }, {
          title: 'Test title',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.',
          img: 'http://placeimg.com/300/200/architecture'
        }
      ]
    }
  }
}
</script>
