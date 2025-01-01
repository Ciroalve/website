<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
          <h5 style="background-color: black;" class="text-white text-center rounded-3 p-2 m-3">
            Statistik Data <b>SMKN 4 TASIKMALAYA</b>
          </h5>
        </div>
        <div class="col-lg-12">
          <p style="background-color: whitesmoke;" class="rounded-3 p-1 m-3 text-secondary">
            <NuxtLink to="/profil" class="text-decoration-none">Profil</NuxtLink>/ Statistik Data
          </p>
        </div>
        <!-- Statistik Data -->
      <div class="col-lg-12 mb-3">
        <div class="card">
          <div class="card-header bg-light">
            <h5 class="text-center">Statistik Data</h5>
          </div>
          <div class="card-body">
            <div class="row">
              <!-- Jumlah Siswa -->
              <div class="col-md-6 mb-3">
                <div class="card bg-success text-white text-center">
                  <div class="card-body">
                    <h6>Jumlah Siswa</h6>
                    <h3>1610</h3>
                  </div>
                </div>
              </div>
              <!-- Jumlah Rombel -->
              <div class="col-md-6 mb-3">
                <div class="card bg-danger text-white text-center">
                  <div class="card-body">
                    <h6>Jumlah Rombel</h6>
                    <h3>41</h3>
                  </div>
                </div>
              </div>
              <!-- Jumlah Guru -->
              <div class="col-md-6 mb-3">
                <div class="card bg-warning text-white text-center">
                  <div class="card-body">
                    <h6>Jumlah Guru</h6>
                    <h3>82</h3>
                  </div>
                </div>
              </div>
              <!-- Jumlah Tenaga Administrasi -->
              <div class="col-md-6 mb-3">
                <div class="card bg-info text-white text-center">
                  <div class="card-body">
                    <h6>Jumlah Tenaga Administrasi</h6>
                    <h3>12</h3>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.container-fluid {
  padding: 20px;
}

.text-white {
  color: #ffffff !important;
}

.text-secondary {
  color: #6c757d !important;
}

.text-center {
  text-align: center !important;
}

.text-decoration-none {
  text-decoration: none !important;
}

.bg-light {
  background-color: #f8f9fa !important;
}

.bg-success {
  background-color: #28a745 !important;
}

.bg-danger {
  background-color: #dc3545 !important;
}

.bg-warning {
  background-color: #ffc107 !important;
}

.bg-info {
  background-color: #17a2b8 !important;
}

.card {
  border: none;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card-body h6 {
  font-size: 1rem;
  margin-bottom: 10px;
}

.card-body h3 {
  font-size: 2rem;
  font-weight: bold;
}

h5 {
  font-size: 1.5rem;
  margin: 0;
}

h6 {
  font-size: 1.1rem;
}

p {
  font-size: 0.9rem;
  margin: 0;
}

.rounded-3 {
  border-radius: 16px !important;
}

.p-2 {
  padding: 10px !important;
}

.p-1 {
  padding: 5px !important;
}

.m-3 {
  margin: 15px !important;
}

.mb-3 {
  margin-bottom: 15px !important;
}

.row {
  margin-left: 0;
  margin-right: 0;
}

</style>