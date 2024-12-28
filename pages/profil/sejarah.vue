<template>
    <div class="history">
      <div class="container">
        <div class="row">
          <!-- Gambar Profil -->
          <div class="image-container">
            <img src="/assets/img/PaKur.jpg" alt="Kepala Sekolah" class="profile-image" />
          </div>
          <!-- Konten Sejarah -->
          <div class="content">
            <h2>Sejarah SMK Negeri 4 Tasikmalaya</h2>
            <p>
              Sejalan dengan Program Pemerintah dibidang pendidikan Menengah Kejuruan pada saat itu yakni pemerataan akses ditambah pula dengan banyaknya keinginan masyarakat yang
              mengharapkan adanya SMK Negeri di daerah Kecamatan Purbaratu Kota Tasikmalaya, terutama untuk menampung tamatan dari SLTP yang ingin melanjutkan ke SMK maka beberapa
              tokoh masyarakat, unsur pejabat pemerintah di Kecamatan Purbaratu Kota Tasikmalaya mengusulkan kepada pemerintah Kota Tasikmalaya dan Pemerintah Provinsi Jawa Barat,
              agar berdirinya SMK Negeri di Kecamatan Purbaratu Kota Tasikmalaya.
            </p>
            <p>
              Setelah melalui perjuangan yang sangat panjang dari berbagai pihak khususnya Disdik Kota Tasikmalaya dan pihak-pihak terkait lainnya sesuai prosedur dan ketentuan yang
              berlaku pada waktu itu dengan mengucapkan syukur Alhamdulillah akhirnya pada tahun pelajaran 2010/2011 SMK Negeri 4 Tasikmalaya mulai berdiri, pada awalnya membuka
              Kompetensi Keahlian Teknik Komputer dan Jaringan dengan pendaftar peserta Didik Baru pada waktu itu berjumlah 44 orang. Pada awalnya tempat belajar menumpang di SMP
              Negeri 17 Kota Tasikmalaya, dan sekolah induknya adalah SMK Negeri 2 Kota Tasikmalaya. Untuk Tenaga pendidik dan Tenaga Kependidikan masih dibantu sepenuhnya oleh kedua
              sekolah tersebut.
            </p>
            <p>
              Pada tahun 2012 keluarlah surat Izin Pendirian berdasarkan keputusan kepala Badan Pelayanan Perizinan Terpadu Kota Tasikmalaya No. 420/9/SK-BPPT/2012 Tanggal 06
              Februari 2012.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="table-container">
    <h1>Perkembangan Infrastruktur SMKN 4 Tasikmalaya Pertahun</h1>
    <table>
      <thead>
        <tr>
          <th>Tahun</th>
          <th>Ruang Kelas</th>
          <th>Kompetensi Keahlian</th>
          <th>Jumlah Siswa</th>
          <th>Pimpinan</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(row, index) in data" :key="index">
          <td>{{ row.tahun }}</td>
          <td>{{ row.ruangKelas }}</td>
          <td>{{ row.kompetensiKeahlian }}</td>
          <td>{{ row.jumlahSiswa }}</td>
          <td>{{ row.pimpinan }}</td>
        </tr>
      </tbody>
    </table>
  </div>
  <div class="row">
    <div class="col-4">   
        <table>
        { tahun: "2010/2011", ruangKelas: "di SMPN 17", kompetensiKeahlian: "TKJ", jumlahSiswa: "44", pimpinan: "PLT. Drs. H. Ario Wiguno, M.MPd" },
        { tahun: "2011/2012", ruangKelas: "di SMPN 17", kompetensiKeahlian: "TKJ", jumlahSiswa: "?", pimpinan: "PLT. Drs. H. Ario Wiguno, M.MPd" },
        { tahun: "2012/2013", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ", jumlahSiswa: "?", pimpinan: "PLT. H. Edy Sugandi, MM" },
        { tahun: "2013/2014", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ", jumlahSiswa: "?", pimpinan: "PLT. H. Edy Sugandi, MM" },
        { tahun: "2014/2015", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ", jumlahSiswa: "268", pimpinan: "Drs. H. Desnueri" },
        { tahun: "2015/2016", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TSM", jumlahSiswa: "?", pimpinan: "Drs. H. Desnueri" },
        { tahun: "2016/2017", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TSM", jumlahSiswa: "693", pimpinan: "Drs. H. Desnueri" },
        { tahun: "2017/2018", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TBSM", jumlahSiswa: "1021", pimpinan: "Drs. H. Desnueri" },
        { tahun: "2018/2019", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TBSM", jumlahSiswa: "1093", pimpinan: "Drs. H. Desnueri" },
        { tahun: "2019/2020", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TBSM", jumlahSiswa: "1116", pimpinan: "Drs. H. Desnueri" },
        { tahun: "2020/2021", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TBSM", jumlahSiswa: "1150", pimpinan: "Didah S Sukanda, S.Pd, M.Pd" },
        { tahun: "2021/2022", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TBSM", jumlahSiswa: "?", pimpinan: "Kurniawan, S.Pd, M.Pd" },
        { tahun: "2022/2023", ruangKelas: "di SMKN 4", kompetensiKeahlian: "TKJ, RPL, TBSM, TOI, DKV", jumlahSiswa: "1240", pimpinan: "Kurniawan, S.Pd, M.Pd" },
        </table>
      </div>
    </div>
      ],

  </template>
  
  <script>
  export default {
    name: "History",
  };
  </script>
  
  <style scoped>
  .history {
    font-family: Arial, sans-serif;
    margin: 20px;
    padding: 20px;
  }
  .container {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
  }
  .row {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  .image-container {
    flex: 1;
    max-width: 150px;
    text-align: center;
  }
  .profile-image {
    width: 100%;
    border-radius: 50%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  .content {
    flex: 3;
    text-align: justify;
  }
  .content h2 {
    font-size: 24px;
    margin-bottom: 10px;
    color: #333;
  }
  .content p {
    line-height: 1.8;
    margin-bottom: 10px;
    color: #555;
  }
  .table-container {
  font-family: Arial, sans-serif;
  padding: 20px;
  max-width: 1000px;
  margin: auto;
  text-align: left;
  color: #333;
}

h1 {
  text-align: center;
  margin-bottom: 20px;
  color: #444;
}

table {
  width: 100%;
  border-collapse: collapse;
  margin: 0 auto;
}

thead {
  background-color: #f4f4f4;
}

th,
td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: center;
}

th {
  background-color: #f2f2f2;
  font-weight: bold;
}

tr:nth-child(even) {
  background-color: #f9f9f9;
}

tr:hover {
  background-color: #f1f1f1;
}
  </style>
  