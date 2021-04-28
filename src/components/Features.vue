<template>
<div class="container-fluid p-0 features" v-bind:style="{backgroundColor: color}">
    <div class="container">
        <div class="row">
            <div class="col-md-3" v-for="item in data" :key="item.id">
                <div class="feature">
                    <span class="icon">
                        <img :src="require(`../assets/img/icons/${item.icon}.png`)" alt="">
                        </span>
                    <h4>{{item.title}}</h4>
                    <p>{{item.text}}</p>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    props: {
        data: {
            type: Array,
            default: () => []
        },
        color: String
    },
}
</script>