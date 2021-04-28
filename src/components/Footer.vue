<template>
    <footer class="footer">
        <div class="container">
            <div class="row text-center">
                <div class="col">
                    <div class="footer_logo"><img src="../assets/img/realhome_footer.png" class="footer_img"></div>
                    <div class="footer_icons">
                        <div class="icons">
                            <a href="#"><img src="../assets/img/icons/f.png" alt=""></a> 
                            <a href="#"><img src="../assets/img/icons/p.png" alt=""></a>
                            <a href="#"><img src="../assets/img/icons/inst.png" alt=""></a>
                            <a href="#"><img src="../assets/img/icons/gmail.png" alt=""></a>
                        </div>
                    </div>
                </div>
                <div class="col navigation">
                    <h3 class="footer_title">Navigation</h3>
                    <ul class="footer_list">
                        <ul class="footer_list">
                        <li class="footer_link" v-for="(menu, index) in footerNavList" :key="index">
                            <router-link :to="menu.path" class="footer_link">{{menu.name}}</router-link>
                        </li>
                    </ul> 
                        
                    </ul> 
                </div>
                <div class="col navigation">
                    <h3 class="footer_title">For Clients</h3>
                    <ul class="footer_list">
                        <li class="footer_item">
                            <a href="" class="footer_link">Sign in</a>
                        </li>
                        <li class="footer_item">
                            <a href="" class="footer_link">Forum</a>
                        </li>
                        <li class="footer_item">
                            <a href="" class="footer_link">Promotions</a>
                        </li>
                        <li class="footer_item">
                            <a href="" class="footer_link">News</a>
                        </li>
                    </ul> 
                </div>
                <div class="col navigation">
                    <h3 class="footer_title">Contuct us</h3>
                    <ul class="footer_list">
                        <li class="footer_adresses">240 Central Park, London OR 10019</li>
                        <li class="footer_adresses">
                            <p>Freephone: +1 800 559 6580</p>
                            <p>Telephone: +1 959 603 6035</p>
                            <p>FAX: +1 800 559 6580</p>
                        </li>
                        <li class="footer_adresses footer_adress_mail">
                            <a href="mailto:info@realhome.com">info@realhome.com</a>

                            </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>


<script>

import {menuList} from '@/constants/menuLinks.js';
export default{
    data() {
        return {
            footerNavList: menuList
        }
    }
}
</script>
