<template>
    <div>
        <p>Header Page</p>
        <p>{{ myName }}</p>
    </div>
</template>


<script>
export default {
    name: 'header-vue-page',
    props: ['myName']
}
</script>
