<template>
<nav class="navbar navbar-expand-lg navbar-dark" style="background-color: #563F7A">

      <router-link tag="a" to="/" class="navbar-brand">
          Ürün Listesi
          </router-link>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">

          <router-link  active-class="active" tag="li" to="/urun-islemleri" class="nav-item">
          <a class="nav-link">Ürün İşlemleri</a>
          </router-link>

          <router-link active-class="active" tag="li" to="/urun-cikisi" class="nav-item">
          <a class="nav-link">Ürün Çıkışı</a>
          </router-link>

        </ul>
    </div>
</nav>
</template>
