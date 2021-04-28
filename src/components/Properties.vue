<template>
    <div class="container-fluid p-0 properties">
        <div class="container p-0">
            <div class="row">
                <div class="col block_title">
                    <h3>Featured <b>Properties</b></h3>
                    <p>Quisque diam lorem interdum vitaapibus vitae pede. Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum auctovinar.</p>
                </div>
            </div>
            <div class="row d-flex justify-content-around">
                <div class="col-md-4 col-sm-12 item properties_col" v-for="item in data" :key="item.id">
                    <img class="properties__img" :src="require(`../assets/img/houses/${item.photo}`)" alt="">
                    <h4 class="properties_title">{{item.title}}</h4>
                    <p class="properties_field">{{item.field}}</p>
                    <p class="properties_price">{{item.price}}</p>
                    <ul class="properties_desc">
                        <li class="properties_item">{{item.desc.area}}</li>
                        <li class="properties_item">{{item.desc.bedrooms}}</li>
                        <li class="properties_item">{{item.desc.bathrooms}}</li>
                    </ul>
                </div>
            </div>
            <button class="btn btn-primary properties_button">ALL PROPERTIES</button>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        data: {
            type: Array,
            default: () => []
        }
    },
}
</script>