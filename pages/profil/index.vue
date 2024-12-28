<template>
    <div class="profile-container">
      <div class="profile-header">
        <h1>Profil SMKN 4 Tasikmalaya</h1>
      </div>
      <div class="profile-content">
        <div class="profile-tab">
          <button @click="activeTab = 'profil'" :class="{ active: activeTab === 'profil' }">Profil</button>
        </div>
        <div v-if="activeTab === 'profil'" class="profile-details">
          <h2>Sejarah SMK Negeri 4 Tasikmalaya</h2>
          <div class="profile-description">
            <img src="/assets/img/pakur.jpg" alt="Foto Kepala Sekolah" width="100" height="100" />
            <p>
              Sejalan dengan Program Pemerintah di bidang pendidikan Menengah Kejuruan pada saat itu yakni pemerataan akses
              ditambah pula dengan banyaknya keinginan masyarakat yang mengharapkan adanya SMK Negeri di daerah Kecamatan
              Purbaratu Kota Tasikmalaya, terutama untuk menampung tamatan dari SLTP yang ingin melanjutkan ke SMK, maka
              beberapa tokoh masyarakat, unsur pejabat pemerintah di Kecamatan Purbaratu Kota Tasikmalaya mengusulkan
              kepada pemerintah Kota Tasikmalaya dan Pemerintah Provinsi Jawa Barat, agar berdirinya SMK Negeri di
              Kecamatan Purbaratu Kota Tasikmalaya.
            </p>
          </div>
          <button class="read-more-button">Read more</button>
        </div>
      </div>
    </div>
    <div class="visi-misi-container">
    <div class="visi-misi-header">
      <h1>Visi dan Misi SMK Negeri 4 Tasikmalaya</h1>
    </div>
    <div class="visi-misi-content">
      <div class="visi-section">
        <h2>Visi:</h2>
        <blockquote>
          "Dengan Berlandaskan Iman dan Taqwa Menghasilkan Tamatan yang Cerdas, Akhlak mulia, Kreatif, Aktif, Produktif (CAKAP)"
        </blockquote>
      </div>
      <div class="misi-section">
        <h2>Misi:</h2>
        <ol>
          <li>
            Mengembangkan kecerdasan Peserta didik agar Berprestasi, beriman dan bertaqwa pada Tuhan Yang Maha Esa, berakhlak mulia, berkarakter, 
            berwawasan kebangsaan, berjiwa entrepreneur, serta peduli lingkungan.
          </li>
        </ol>
      </div>
      <button class="read-more-button">Read more</button>
    </div>
  </div>
  <div class="identitas-sekolah-container">
    <div class="identitas-header">
      <h1>Identitas Sekolah Menengah Kejuruan Negeri 4 Tasikmalaya</h1>
    </div>
    <div class="identitas-content">
      <ul>
        <li>
          <strong>a. Nama Sekolah</strong> : SMK Negeri 4 Kota Tasikmalaya
        </li>
        <li>
          <strong>b. NPSN</strong> : 20276063
        </li>
        <li>
          <strong>c. Nomor Statistik Sekolah</strong> : 401327810004
        </li>
        <li>
          <strong>d. Alamat</strong> :
          <ul>
            <li><strong>Jalan</strong> : Jl Depok RT 02 RW 05</li>
            <li><strong>Kelurahan</strong> : Sukamenak</li>
            <li><strong>Kecamatan</strong> : Purbaratu</li>
            <li><strong>Kota</strong> : Tasikmalaya</li>
          </ul>
        </li>
      </ul>
      <button class="read-more-button">Read more</button>
    </div>
  </div>
  <div class="container">
    <h3 class="title">Pendidik dan Tenaga Kependidikan</h3>
    <div class="cards">
      <div v-for="(card, index) in cards" :key="index" class="card">
        <h4><i class="info-icon">ℹ️</i> {{ card.title }}</h4>
        <p>Laki-laki : {{ card.male }} orang</p>
        <p>Perempuan : {{ card.female }} orang</p>
        <p>Total : {{ card.total }} orang</p>
      </div>
    </div>
    <button class="read-more">Read more</button>
  </div>
  <div class="container">
    <h3 class="title">Struktur Organisasi</h3>
    <ul class="organization-list">
      <li v-for="(person, index) in organization" :key="index">
        <span class="role">{{ index + 1 }}. {{ person.role }}</span> : <span class="name">{{ person.name }}</span>
      </li>
    </ul>
    <button class="read-more">Read more</button>
  </div>
  <script>
  export default {
    data() {
    return {
      organization: [
        { role: "Kepala Sekolah", name: "Kurniawan, S.Pd, M.Pd." },
        { role: "Komite Sekolah", name: "H. Abun Sulaeman, S.Ag" },
        { role: "PLT Kasubag TU", name: "Yaman Suryaman, S.Sos." },
      ],
    };
  },
};
</script>

 
  </template>
  
  <script>
  export default {
    data() {
      return {
        activeTab: 'profil',
      };
    },
  };
  </script>
  
  <style scoped>
  .profile-container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    font-family: Arial, sans-serif;
  }
  
  .profile-header {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .profile-tab {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
  }
  
  .profile-tab button {
    padding: 10px 20px;
    margin: 0 5px;
    border: none;
    background-color: #f0f0f0;
    cursor: pointer;
  }
  
  .profile-tab button.active {
    background-color: #333;
    color: white;
  }
  
  .profile-details {
    text-align: center;
  }
  
  .profile-description {
    display: flex;
    align-items: flex-start;
    justify-content: center;
    margin-top: 20px;
  }
  
  .profile-description img {
    border-radius: 50%;
    margin-right: 20px;
  }
  
  .profile-description p {
    text-align: justify;
  }
  
  .read-more-button {
    margin-top: 20px;
    padding: 10px 20px;
    border: none;
    background-color: #007bff;
    color: white;
    cursor: pointer;
    border-radius: 5px;
  }
  
  .read-more-button:hover {
    background-color: #0056b3;
  }
  .visi-misi-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  font-family: Arial, sans-serif;
}

.visi-misi-header {
  text-align: center;
  margin-bottom: 20px;
}

.visi-misi-content {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
}

.visi-section,
.misi-section {
  margin-bottom: 20px;
}

.visi-section blockquote {
  font-size: 16px;
  font-style: italic;
  text-align: center;
  color: #555;
  margin: 0;
  padding: 10px;
  border-left: 5px solid #007bff;
  background-color: #fff;
}

.misi-section ol {
  margin: 0;
  padding-left: 20px;
  list-style: decimal;
}

.misi-section li {
  font-size: 14px;
  line-height: 1.8;
}

.read-more-button {
  display: block;
  margin: 20px auto 0;
  padding: 10px 20px;
  border: none;
  background-color: #007bff;
  color: white;
  cursor: pointer;
  border-radius: 5px;
}

.read-more-button:hover {
  background-color: #0056b3;
}
.identitas-sekolah-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  font-family: Arial, sans-serif;
}

.identitas-header {
  text-align: center;
  margin-bottom: 20px;
}

.identitas-content {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
}

.identitas-content ul {
  list-style: none;
  padding: 0;
}

.identitas-content li {
  font-size: 16px;
  margin-bottom: 10px;
}

.identitas-content li strong {
  font-weight: bold;
}

.identitas-content ul ul {
  margin-left: 20px;
}

.read-more-button {
  display: block;
  margin: 20px auto 0;
  padding: 10px 20px;
  border: none;
  background-color: #007bff;
  color: white;
  cursor: pointer;
  border-radius: 5px;
}

.read-more-button:hover {
  background-color: #0056b3;
}
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
  font-family: Arial, sans-serif;
}

.title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 20px;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

.card {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
  width: 200px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: left;
}

.card h4 {
  font-size: 1.2rem;
  margin-bottom: 10px;
}

.info-icon {
  font-size: 1.2rem;
  margin-right: 5px;
}

.read-more {
  margin-top: 20px;
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 1rem;
}

.read-more:hover {
  background-color: #0056b3;
}
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
  font-family: Arial, sans-serif;
}

.title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 20px;
}

.organization-list {
  text-align: left;
  margin: 0 auto;
  padding: 0;
  list-style: none;
}

.organization-list li {
  margin: 10px 0;
  font-size: 1rem;
}

.role {
  font-weight: bold;
}

.read-more {
  margin-top: 20px;
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 1rem;
}

.read-more:hover {
  background-color: #0056b3;
}
  </style>
  