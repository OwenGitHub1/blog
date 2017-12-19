<template>
    <div>
        <MyNav></MyNav>
        <div class="containerBody">
            test
        </div>
        <MyFooter></MyFooter>
    </div>
</template>

<script>
	import MyNav from '~/components/Nav.vue'
	import MyFooter from '~/components/Footer.vue'

    export default {
	    components: {
          MyNav,
          MyFooter
	    }
    }
</script>

<style slot-scoped>
    .containerBody{
        padding-top: 60px;
    }
</style>