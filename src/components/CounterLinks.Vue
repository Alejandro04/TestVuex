<template>
  <div class="hello">
    <div class="left">
      <!-- Other code removed for brevity -->
    </div>
    <div class="right">
      <stats />  <!-- Add this -->
    </div>
  </div>
</template>

<script>
import Hello from '@/components/HelloWorld' 
import { mapState } from 'vuex'

export default {
  name: 'HelloWorld',
  components: {                        
    Hello
  },
  computed: {
    // Code removed for brevity
  }
}
</script>