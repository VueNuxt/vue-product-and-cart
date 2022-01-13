<template>
    <div class="card">
        <div class="card-title">
        Carrots
        </div>
        <div class="card-body">
        <i class="icofont-10x icofont-carrot"></i>
        <form>
            <div class="row">
            <div class="cell">
                <label>Type:</label>
            </div>
            <div class="cell">
                <em>Vegetable</em>
            </div>
            </div>
            <div class="row">
            <div class="cell">
                <label>Price:</label>
            </div>
            <div class="cell">
                $4.82
            </div>
            </div>
            <div class="row">
            <div class="cell">
                <label>Quantity:</label>
            </div>
            <div class="cell">
                <input type="number" v-model.number="inventory.carrots">
            </div>
            </div>
        </form>
        </div>
        <div class="card-footer">
        <button @click="addToCart('carrots')" class="btn btn-light">
            Add to cart
        </button>
        </div>
    </div>

    <div class="card">
        <div class="card-title">
        Pineapples
        </div>
        <div class="card-body">
        <i class="icofont-10x icofont-pineapple"></i>
        <form>
            <div class="row">
            <div class="cell">
                <label>Type:</label>
            </div>
            <div class="cell">
                <em>Fruit</em>
            </div>
            </div>
            <div class="row">
            <div class="cell">
                <label>Price:</label>
            </div>
            <div class="cell">
                $1.62
            </div>
            </div>
            <div class="row">
            <div class="cell">
                <label>Quantity:</label>
            </div>
            <div class="cell">
                <input type="number" v-model="inventory.pineapples">
            </div>
            </div>
        </form>
        </div>
        <div class="card-footer">
        <button class="btn btn-light">Add to cart</button>
        </div>
    </div>

    <div class="card">
        <div class="card-title">
        Cherries
        </div>
        <div class="card-body">
        <i class="icofont-10x icofont-cherry"></i>
        <form>
            <div class="row">
            <div class="cell">
                <label>Type:</label>
            </div>
            <div class="cell">
                <em>Fruit</em>
            </div>
            </div>
            <div class="row">
            <div class="cell">
                <label>Price:</label>
            </div>
            <div class="cell">
                $1.04
            </div>
            </div>
            <div class="row">
            <div class="cell">
                <label>Quantity:</label>
            </div>
            <div class="cell">
                <input type="number" v-model="inventory.cherries">
            </div>
            </div>
        </form>
        </div>
        <div class="card-footer">
        <button class="btn btn-light">Add to cart</button>
        </div>
    </div>
</template>

<script>
export default {
  props: ['product', 'index'],
  data () {
      return {
          quantity: 0
      }
  }
}
</script>
