<!-- TODO: Hãy viết thành một component hoàn chỉnh -->
<template lang="html">
   <div id="img">

   <span v-for="item in items">
   <img :src="'../public/image/' + item.photo" :alt="item.name" width="128" height="128">
       <p>{{item.name}}</p>
       <p>{{item.type}}</p>
    </span>

   </div>
</template>

<script>
export default {
   props: ['items']
}
</script>

<style lang="css">
</style>