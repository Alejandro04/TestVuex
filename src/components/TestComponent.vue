<template>
  <div class="hello">
    <div class="left">
      <h1>{{ title }}</h1>
      <h1>{{ custom }}</h1>

       <ul>
        <li v-for="(link, index) in links" v-bind:key="index">
          {{ link }}
        </li>
      </ul>

    </div>
    <div class="right">

    </div>
  </div>
</template>


<script>
import { mapState } from 'vuex'

export default {
  name: 'TestComponent',
  computed: {
    ...mapState([
      'title',
      'custom',
      'links'
    ]),
    // Other properties
  }
}
</script>