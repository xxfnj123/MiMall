<template>
    <div>
        
        <service-bar></service-bar>
    </div>
</template>
<script>
    import ServiceBar from './../components/ServiceBar'
    export default{
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'index',
        components: {
            ServiceBar
        }
    }
</script>