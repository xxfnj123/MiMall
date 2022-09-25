<template>
    <div>
        <order-header></order-header>
        <router-view></router-view>
        <nav-footer></nav-footer>
    </div>
</template>
<script>
    import OrderHeader from './../components/OrderHeader'
    import NavFooter from './../components/NavFooter'
    export default{
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'order',
        components: {
            OrderHeader,
            NavFooter
        }
    }
</script>