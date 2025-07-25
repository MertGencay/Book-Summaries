<template>
    <section class="full-section-heigth">
        <div class="container">
             <form  @submit.prevent="submitForm">
          <div class="text-center mb-4">
          <h2 class="form-title">📚 Giriş Yap ve Kitap Dünyası Katıl!</h2>
          <p class="form-subtitle">Favori kitaplarını keşfet, yorum yap ve topluluğumuza katıl.</p>
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

          


          <!-- Submit Button -->
          <div class="row justify-content-center">
            <div class="col-md-6 col-8 mb-3">
              <button type="submit" class="btn btn-primary w-100">Giriş Yap</button>
            </div>
          </div>
        </form>
        </div>
    </section>
</template>


<script>
    export default {
        name: "LoginView",
        data() {
            return {
                formData: {
                    email: '',
                    password: '',
                }
            }
        },
    }
</script>

<style scoped>

form {
  background-color: transparent;
  box-shadow: none;
  border: none;
  padding: 10px;
  margin-bottom: 1px;
}

.form-label {
    font-size: 1rem;
    font-weight: 700;
    color: #ffffff;
}

/* Başlık ve alt metin */
.form-title {
  font-size: 1.8rem;
  font-weight: 700;
  color: #ffffff;
}

.form-subtitle {
  font-size: 1rem;
  color: #f6f6f6;
  margin-bottom: 20px;
}
</style>