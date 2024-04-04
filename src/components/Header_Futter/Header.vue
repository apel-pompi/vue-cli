<template>
    <div>
        <p>Header Page</p>
        <ul>
            <li v-for="(myNames,index) in myName" :key="index">
                {{ myNames }}
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    name: 'header-vue-page',
    props: {
        myName: {
            type: Array,
            required:true
        }
    }
}
</script>
