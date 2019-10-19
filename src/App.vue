<template>
  <div id="app">
   <AppHeader />
      <router-view />
    <AppFooter />
  </div>
</template>


<script lang="ts">
import {Vue, Component} from 'vue-property-decorator';
// import nav header
import AppHeader from '@/components/static/AppHeader/AppHeader.vue';
import AppFooter from '@/components/static/AppFooter/AppFooter.vue';


// declare vuejs component
@Component({
  components: {AppHeader, AppFooter},
})
export default class App extends Vue {
}

</script>