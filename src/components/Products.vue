<template>
    <h2>Luxury Cars</h2>
<div class="container">
    <div class="card_cars" v-for="item in arr" :key="item">
     <img :src="item.picture" style="height: 500px;" alt="car">
     <h3>{{item.carName}}</h3>
     <h4>{{item.type}}</h4>
     <p>{{item.color}}</p>
   <button class="btn" v-on:click="purchase">Purchase</button>
  </div>
</div>
</template>
<script>
export default {
  name: 'Products',
  methods: {
    purchase() {
    alert("Purchase Successful");
}
  },

  data (){
    return {
  arr : [
  {
    carName: 'Nissan',
    type: 'GTR',
    color: 'Grey',
    picture: 'https://i.postimg.cc/dVq2NQGN/nissan.jpg'
  },
  {
    carName: 'Honda',
    type: 'Civic Type R',
    color: 'Orange',
    picture: 'https://i.postimg.cc/C5S5M5hW/honda.jpg'
  },
  {
    carName: 'Toyota',
    type: 'Supra',
    color: 'Yellow',
    picture: 'https://i.postimg.cc/vmn5c1yB/supra.jpg'
  },
  {
    carName: 'Tesla',
    type: 'Model X',
    color: 'White',
    picture: 'https://i.postimg.cc/Jz4TD5Yh/tesla.jpg'
  }
]
}
  }
}
</script>
<style>
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    padding: 30px;
}

.card_cars {
    border: 1px solid;
    padding: 10px;
    box-shadow: 5px 10px;
}

.btn {
    border: 1px solid;
    padding: 10px;
    box-shadow: 10px 5px;
}

.btn:hover {
    border: 1px solid gold;
    padding: 10px;
    box-shadow: 10px 5px;
}
</style>