<template>
    <div>
        <h2 class="title">{{post.title}}</h2>
        <p class="date">{{post.date}}</p>
        <p class="text">{{post.text}}</p>
    </div>
</template>

<script>
export default {
    name: "BlogPost",
    props: ["post"]
}
</script>

<style scoped>
.title{

}

.date{

}

.text{

}

</style>

