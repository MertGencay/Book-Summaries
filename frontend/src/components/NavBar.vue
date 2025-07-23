<template>
    <nav class="navbar navbar-expand-md custom-nav">
        <div class="container">
            <a class="navbar-brand" href="#">Kitap Özetleri</a>
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a class="nav-link" href="#">Anasayfa</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Kitaplar</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">İletişim</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Giriş Yap</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Kayıt Ol</a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "NavBar",
    }
</script>

<style scoped>
.custom-nav{
    background-color: #00ae8e;
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
    padding: 10px 25px;
    color: #fff;
    text-align: center;
}
</style>