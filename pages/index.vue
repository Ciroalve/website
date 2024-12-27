<template>
<section id="carousel" class="mb-5">
    <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"></button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></button>
            <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="/assets/img/ft1.png" class="d-block w-100" alt="Ekstrakurikuler 1">
            </div>
            <div class="carousel-item">
                <img src=""  class="d-block w-100" alt="Ekstrakurikuler 2">
            </div>
            <div class="carousel-item">
                <img src="" class="d-block w-100" alt="Ekstrakurikuler 3">
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
            <span class="carousel-control-prev-icon"></span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
            <span class="carousel-control-next-icon"></span>
        </button>
    </div>
    
    <Jurusan />
</section>
<footer class="footer">
    <div class="container">
      <div class="footer-section">
        <h3>Hubungi Kami</h3>
        <p>SMKN 4 Tasikmalaya</p>
        <p>Jl. Depok Kel. Sukamenak Kec. Purbaratu</p>
        <p>Kota Tasikmalaya 46196</p>
        <p><i class="fas fa-phone"></i> +62265312059</p>
        <p><i class="fas fa-envelope"></i> info@smkn4-tsm.sch.id</p>
      </div>
      <div class="footer-section">
        <h3>Media Sosial</h3>
        <ul>
          <li><a href="#"><i class="fab fa-facebook"></i> Facebook</a></li>
          <li><a href="#"><i class="fab fa-twitter"></i> Twitter</a></li>
          <li><a href="#"><i class="fab fa-instagram"></i> Instagram</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>Link Eksternal</h3>
        <ul>
          <li><a href="#">Kemdikbud</a></li>
          <li><a href="#">Dapodikdasmen</a></li>
          <li><a href="#">PSMK</a></li>
          <li><a href="#">Disdik Jabar</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <p>© SMKN 4 Tasikmalaya. All rights reserved.</p>
      <p>Designed and Engineered by <span class="operator">Operator</span></p>
    </div>
  </footer>
</template>

<style>
    .carousel-item img {
        width: 100%;
        height: 600px; 
        object-fit: cover; 
    }

    
    .carousel-item {
        position: relative;
    }

    .carousel-item::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(to bottom, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
        z-index: 1;
    }

    .carousel-item img {
        position: relative;
        z-index: 2;
    }

   
    .carousel-control-prev-icon,
    .carousel-control-next-icon {
        filter: invert(1);
    }

    
    .carousel-indicators button {
        width: 12px;
        height: 12px;
        border-radius: 50%;
        background-color: rgba(255, 255, 255, 0.5);
    }

    .carousel-indicators .active {
        background-color: #fff;
    }

    
    @media (max-width: 768px) {
        .carousel-item img {
            height: 500px;
        }
    }
    body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}
#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
.footer {
  background-color: #333;
  color: #fff;
  padding: 20px 0;
}
.container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
.footer-section {
  flex: 1;
  margin: 10px;
}
.footer-section h3 {
  margin-bottom: 10px;
  font-size: 18px;
}
.footer-section p,
.footer-section ul {
  margin: 5px 0;
}
.footer-section ul {
  list-style: none;
  padding: 0;
}
.footer-section ul li a {
  color: #fff;
  text-decoration: none;
}
.footer-section ul li a:hover {
  text-decoration: underline;
}
.footer-bottom {
  text-align: center;
  margin-top: 20px;
  font-size: 14px;
}
.operator {
  font-weight: bold;
  color: #ff4747;
}
</style>
