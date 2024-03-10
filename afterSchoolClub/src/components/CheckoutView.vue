 <template>
    <div class="checkout-container col-11 p-0">
      <div class="checkout-header col-12 p-4">
        <h2>welcome <br> to checkout page</h2>
        <hr class = "divider">

      </div>
     

      <div class="checkout-form col-12">
        <h3>Enter your details and <br> Submit your order</h3>
        <input type="text" placeholder="Full Name" class="col-10">
        <input type="text" placeholder="Phone Number" class="col-10">
      </div>

      <div class="list-of-items container-fluid p-0">
        <ul class="col-12 p-3">
          <li>

          </li>
          <li>

</li>
<li>

</li>
          
        </ul>
      </div>

      <div class="button-container col-12">
        <button>Submit Order</button>

      </div>

    </div>
  </template>
  
 
  <script>
  export default {
    name: 'Checkout',
    props: ['cart'],
    methods: {
      removeFromCart(item) {
        this.$emit('remove-item-from-cart', item);
      }
    }
  }
  </script>
  
  <style scoped>
  .checkout-container{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    flex-direction: column;
   height: 100vh;
    background: #fff;

  }

  .checkout-container h2{
    font-size: 1.7em;
    color: green;
    text-align: center;
    font-weight: bold;
    text-transform: uppercase;
  }

  .checkout-form{
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-direction: column;
    text-align: center;
    min-height: 230px;
  }

  .checkout-form input[type="text"]{
    border: none;
    padding: 10px;
    border-radius: 20px;
    background: rgb(239, 239, 239);
    outline: none;

  }

  .checkout-header{
    display: flex;
    align-items: center;
    flex-direction: column;
  
  }

  .list-of-items{
    min-height: 300px;
    scroll-behavior: smooth;
    overflow-y: auto;
    overflow-x: hidden;


  }

  .list-of-items ul{
    background: transparent;
    min-height: 280px;
    max-height: 280px;

  }

  .list-of-items ul li{
    width: 100%;
    height: 120px;
    background: #ffff;
    border-radius: 20px;
    border: solid 2px green;
    margin-bottom: 10px;
  }

  .button-container{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100px;
 

  }


  .button-container button{
    border: none;
    padding: 20px;
    width: 200px;
    border-radius: 20px;
    color: #fff;
    background: green;
    font-weight: bold;
  }
  
  </style>
  