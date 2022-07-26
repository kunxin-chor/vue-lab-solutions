<template>
    <div>
        {{(parseInt(num1) + parseInt(num2))/2}}
    </div>
</template>

<script>
export default {
    props:['num1', 'num2']
}
</script>

<style scoped>

</style>