<template>
    <nav class="navbar navbar-expand-md custom-nav">
        <div class="container">
            <RouterLink class="navbar-brand" :to="{name: 'home'}">{{brandName}}</RouterLink>
            <ul class="navbar-nav">
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{name: 'home'}">Anasayfa</RouterLink>
                </li>
                 <li class="nav-item">
                    <RouterLink class="nav-link" :to="{name: 'books'}">Kitaplar</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{name: 'contact'}">İletişim</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{name: 'login'}">Giriş Yap</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink class="nav-link" :to="{name: 'register'}">Kayıt Ol</RouterLink>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
import { RouterLink } from 'vue-router';

    export default {
        name: "NavBar",
        data(){
            return{
                brandName: "Kitap Özetleri",
            }
        }
    }
</script>

<style scoped>
.custom-nav{
    background-color: var(--primary-color);
    padding: 8px 0;
}

.navbar-brand{
    padding: 0;
    margin: 0;
    color: #fff;
    font-size: 24px;
    font-weight: bold;
}

.nav-link{
    padding: 10px 15px !important;
    color: #fff;
    text-align: center;
}

.nav-link:hover{
    color: var(--secondary-color);
}

.active-link{
    color: var(--secondary-color);
}
</style>