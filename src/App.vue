<template>
    <div id="app">
        <compBookListOne></compBookListOne>
        <compBookListTwo></compBookListTwo>
        <button @click="reduceprice" class="btn btn-primary">Reduce</button>
    </div>
</template>

<script>
import compBookListOne from "./components/BookListOne"
import compBookListTwo from "./components/BookListTwo"
export default {
    components:{
      compBookListOne,
      compBookListTwo
    },
    methods:{
        reduceprice(){
            this.$store.commit('reduceprice')
        }
    }
}
</script>
