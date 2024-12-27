<template>
    <div class="row">
      <div class="header">Kompetensi Keahlian</div>
      <div class="col-4">
        <div class="alert alert-secondary">
            <img src="..." class="card-img-top" alt="...">
          <h3>Teknik Komputer dan Jaringan</h3>
          <div>sarana pendukung pembelajaran:</div>
        </div>
      </div>
      <div class="col-4">
        <div class="alert alert-secondary">
            <img src="..." class="card-img-top" alt="...">
          <h3>Rekayasa Perangkat Lunak dan Gim</h3>
          <div>sarana pendukung pembelajaran:</div>
        </div>
      </div>
      <div class="col-4">
        <div class="alert alert-secondary">
            <img src="..." class="card-img-top" alt="...">
          <h3>Teknik dan Bisnis Sepeda Motor</h3>
          <div>sarana pendukung pembelajaran:</div>
        </div>
      </div>
      <div class="col-4">
        <div class="alert alert-secondary">
            <img src="..." class="card-img-top" alt="...">
          <h3>Desain Komunikasi Visual</h3>
          <div>sarana pendukung pembelajaran:</div>
        </div>
      </div>
      <div class="col-4">
        <div class="alert alert-secondary">
            <img src="..." class="card-img-top" alt="...">
          <h3>Teknik Otomasi Industri</h3>
          <div>sarana pendukung pembelajaran</div>
        </div>
      </div>
    </div>
  </template>
  
  <style>
  
  .row {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
    padding: 20px;
    background-color: #f8f9fa; 
    border-radius: 8px;
    margin: 20px auto;
    max-width: 1200px; 
  }
  
  
  .header {
    font-size: 24px;
    font-weight: bold;
    text-align: center;
    width: 100%;
    margin-bottom: 20px;
    color: #343a40;
  }
  

  .col-4 {
    flex: 0 0 calc(33.333% - 20px); 
    box-sizing: border-box;
  }
  
  @media (max-width: 768px) {
    .col-4 {
      flex: 0 0 calc(50% - 20px); 
    }
  }
  
  @media (max-width: 576px) {
    .col-4 {
      flex: 0 0 100%; 
    }
  }
  
  /* Styling untuk alert */
  .alert {
    background-color: #ffffff;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); 
    transition: transform 0.3s, box-shadow 0.3s;
  }
  
  .alert:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15); 
  }
  
  
  .alert h3 {
    font-size: 18px;
    font-weight: bold;
    color: #007bff; 
    margin-bottom: 10px;
  }
  
  
  .alert div {
    font-size: 14px;
    color: #6c757d; 
  }
  </style>
  
