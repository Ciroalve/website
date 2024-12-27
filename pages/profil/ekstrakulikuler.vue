<template>
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12">
            <h5 style="background-color: black;" class="text-white text-center rounded-3 p-2 m-3">
              Ekstrakulikuler <b>SMKN 4 TASIKMALAYA</b>
            </h5>
          </div>
  
          <section class="gallery">
        <div class="gallery-item">
          <img src="/assets/image/upacara.jpg" alt="Upacara Bendera" class="gallery-image" />
          <p class="gallery-caption">Upacara Bendera</p>
        </div>
        <div class="gallery-item">
          <img src="" alt="Lomba Futsal" class="gallery-image" />
          <p class="gallery-caption">Lomba Futsal</p>
        </div>
        <div class="gallery-item">
          <img src="" alt="Kunjungan Industri" class="gallery-image" />
          <p class="gallery-caption">Kunjungan Industri</p>
        </div>
        <div class="gallery-item">
          <img src="" alt="Pentas Seni" class="gallery-image" />
          <p class="gallery-caption">Pentas Seni</p>
        </div>
      </section>
  
      </div>
    </div>
  </template>
  
  <style scoped>
  .gallery {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
    margin: 20px 0;
  }
  
  .gallery-item {
    background-color: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 10px;
    transition: transform 0.3s;
  }
  
  .gallery-item:hover {
    transform: scale(1.05);
  }
  
  .gallery-image {
    max-width: 100%;
    border-radius: 8px;
  }
  
  .gallery-caption {
    color: #555;
    margin-top: 10px;
  }
  </style>