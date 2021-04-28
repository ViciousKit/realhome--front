<template>
    <div class="container blog">
        <div class="col-md-12 blog_link about_us_link"><a href="/">Home</a><b>-></b> Blog</div>
        <div class="d-flex flex-row blog_flex">
            <div class="d-flex flex-column blog_column_post">
                <div class="col-md-8 blog_post" v-for="post in blog_posts" :key="post.id">
                    <div class="blog_post_title">{{post.title}}</div>
                    <img :src="require(`../assets/img/blog/${post.img}`)" alt="" class="blog_post_image">
                    <p class="blog_post_text">{{post.text}}</p>
                    <div class="col-2">
                    <router-link class="nav-link active blog_post_button" aria-current="page" :to="{name:'Blog-post', params: {id: post.id}}">
                        Read More
                    </router-link>
                    </div>
                </div>
            </div>
            <div class="blog_column_nav">    
                <div class="col-md-4 d-flex flex-column blog_nav">
                <div class="blog_nav_block blog_nav_block_categories">
                    <h1 class="blog_nav_title blog_nav_title_first">Categories</h1>
                    <p class="blog_nav_link">Art Direction</p>
                    <p class="blog_nav_link">Digital Photography</p>
                    <p class="blog_nav_link">Information Architecture</p>
                    <p class="blog_nav_link">Interior Design</p>
                    <p class="blog_nav_link">Motion Graphics</p>
                    <p class="blog_nav_link">Photoshop Tools</p>
                    <p class="blog_nav_link">Web Design</p>
                </div>
                <div class="blog_nav_block blog_nav_block_archives">
                    <h1 class="blog_nav_title">Archives</h1>
                    <p class="blog_nav_link">May 2014</p>
                    <p class="blog_nav_link">March 2013</p>
                    <p class="blog_nav_link">February 2013</p>
                    <p class="blog_nav_link">January 2013</p>
                    <p class="blog_nav_link">December 2012</p>
                    <p class="blog_nav_link">May 2012</p>
                </div>
                <div class="blog_nav_block blog_nav_block_recent">
                    <h1 class="blog_nav_title">Recent Posts</h1>
                    <h1 class="blog_nav_title_recentPost">Aliquam erat volutpat</h1>
                    <p class="blog_nav_postText">Proin umcorper urna et felisstibulum iaculis lacinia est. Proin dictum elem entum velit fusce euismod. Aenean commodo ligula eget dolor. Proin dictum elem entum velit fusce.</p>
                    <p class="blog_nav_postDate">May 27, 2014</p>
                </div>
                </div>
            </div>    
        </div>
    </div>
</template>


<script>
import {blog_posts} from '@/data/data.blog_posts.js';
export default {
    data() {
        return {
            blog_posts
        }
    }
}
</script>