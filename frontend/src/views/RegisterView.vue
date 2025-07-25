<template>
  <section class="full-section-heigth">
    <div ></div>
    <div class="container position-relative" style="z-index: 2;">
      <form @submit.prevent="submitForm">
        <!-- Başlık -->
        <div class="text-center mb-4">
          <h2 class="form-title">📚 Kayıt Ol ve Kitap Dünyasına Katıl!</h2>
          <p class="form-subtitle">Favori kitaplarını keşfet, yorum yap ve topluluğumuza katıl.</p>
        </div>

        <!-- Kullanıcı Adı -->
        <div class="row justify-content-center">
          <div class="col-md-6 col-10 mb-3 position-relative">
            <label for="username" class="form-label">Kullanıcı Adı</label>
            <input
              type="text"
              class="form-control input-icon"
              id="username"
              name="username"
              v-model.trim="formData.username"
              required
            />
            <span class="input-icon-left">👤</span>
          </div>
        </div>

        <!-- Email -->
        <div class="row justify-content-center">
          <div class="col-md-6 col-10 mb-3 position-relative">
            <label for="email" class="form-label">Email</label>
            <input
              type="email"
              class="form-control input-icon"
              id="email"
              name="email"
              v-model.trim="formData.email"
              required
            />
            <span class="input-icon-left">✉️</span>
          </div>
        </div>

        <!-- Şifre -->
        <div class="row justify-content-center">
          <div class="col-md-6 col-10 mb-4 position-relative">
            <label for="password" class="form-label">Şifre</label>
            <input
              type="password"
              class="form-control input-icon"
              id="password"
              name="password"
              v-model.trim="formData.password"
              required
            />
            <span class="input-icon-left">🔒</span>
          </div>
        </div>

        <!-- Buton -->
        <div class="row justify-content-center">
          <div class="col-md-6 col-10 mb-3">
            <button type="submit" class="btn btn-primary w-100">Kayıt Ol</button>
          </div>
        </div>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "RegisterView",
  data() {
    return {
      formData: {
        username: '',
        email: '',
        password: '',
      }
    };
  },
  methods: {
    submitForm() {
      console.log("Form gönderildi:", this.formData);
      // Buraya kayıt işlemi entegre edilecek
    }
  }
};
</script>