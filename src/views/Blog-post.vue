<template>
<div class="container">
    <div class="col-md-12 blog_link about_us_link text-center"><a href="/blog">Blog</a><b>-></b> Post</div>
    <div class="row justify-content-center">
        <div class="col-6 ">
            <div class="blog_post_title">{{currentPost.title}}</div>
            <img :src="require(`../assets/img/blog/${currentPost.img}`)" alt="" class="blog_post_image">
            <p class="blog_post_text">{{currentPost.text}}</p>
        </div>
    </div>
</div>
</template>


<script>

import {blog_posts} from '@/data/data.blog_posts.js';
export default {
    props: ['id'],
    data() {
        return {
            blog_posts,
            currentPost: 0
        }
    },
    created() {
        this.currentPost = this.blog_posts[this.id]
    } 
}
</script>