<template>
  <div class="lessonContainer">
     
      <div v-for="(lesson, index) in lessons" :key="index" class="lessonCard">
          <i v-bind:class="lesson.icon" class="lessonIcon"></i>
          <h2>{{lesson.subject}}</h2>
          <p>Location: {{lesson.location}}</p>
          <p>Price: £{{lesson.price}}</p>
          <p>Available Spaces: {{lesson.spaces}}</p>
          <button>
              <i v-if="lesson.spaces != 0" class="fa-solid fa-cart-plus cartIcon"></i>
              <i v-else class="fa-solid fa-cart-shopping cartIcon"></i>
          </button>
      </div>
  </div>
  
</template>

<script>
export default {
  name: "LessonView",
  props: [ "lessons"]
   

}
</script>

