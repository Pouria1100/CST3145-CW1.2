<!-- <template>
    <div class="checkout">
      <h2>Shopping Cart</h2>
      <div v-if="cart.length > 0">
        <ul>
          <li v-for="item in cart" :key="item.id">
            {{ item.subject }} - £{{ item.price }}
            <button @click="removeFromCart(item)">Remove</button>
          </li>
        </ul>
      </div>
      <p v-else>Your cart is empty.</p>
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
  .checkout {
    padding: 20px;
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  }
  
  .checkout h2 {
    color: #4CAF50;
    text-align: center;
  }
  
  .checkout ul {
    list-style-type: none;
    padding: 0;
  }
  
  .checkout li {
    background-color: #f5f5f5;
    margin-bottom: 10px;
    padding: 10px;
    border-radius: 5px;
  }
  
  button {
    margin-left: 10px;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    padding: 5px 10px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  
  button:hover {
    background-color: #367c39;
  }
  
  @media (max-width: 768px) {
    .checkout {
      width: 90%;
      margin: 0 auto;
    }
  }
  </style>
   -->