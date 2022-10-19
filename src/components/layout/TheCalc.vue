<template>
<div>
    <div><input type="number" v-model="amount" /></div>
   <p>Total Walked {{ total }}</p>
   <div>
    <button @click="addAmountToTotal()">Submit</button>
   </div>
   <p>Distance to go {{ distanceToGo }}</p>
</div>
</template>

<script>
export default {
  name: "TheCalc",
  data() {
    return {
      total: 0, 
      amount: 2
         
    };
  },
  computed:
  {
    distanceToGo(){
       return 1800 - this.total
    }
  },
  methods:{
    addAmountToTotal() {
     this.total += this.amount
    }
  }
};

</script>