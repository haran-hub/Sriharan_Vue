<template>
  
  <MyHeader />
  <WhiskeyBox :Whiskey="Whiskey" />
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import WhiskeyBox from './components/WhiskeyBox.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    WhiskeyBox
  },
  data(){
    return {
      Whiskey: []
    }
  },
  methods: {
    // promises

      async fetchWhiskey(){
         const res= await fetch('http://localhost:5000/Whiskey')
         const data= await res.json()
        
          console.log(data)
         return data
      }

  },

  async created(){
    this.Whiskey = await this.fetchWhiskey()
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: black;
}
</style>
