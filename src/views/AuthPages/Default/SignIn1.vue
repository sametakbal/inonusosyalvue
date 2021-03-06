<template>
  <div>
    <h1 class="mb-0">Giriş Yap</h1>
    <p>İnönü email adresiniz veya kullanıcı adınız ile İnönü Sosyal'e giriş yapabilirsiniz.</p>
    <form class="mt-4">
      <div class="form-group">
        <label for="exampleInputEmail1">Email veya Kullanıcı adı</label>
        <input type="email" class="form-control mb-0" id="exampleInputEmail1" placeholder="Emaili giriniz">
      </div>
      <div class="form-group">
        <label for="exampleInputPassword1">Parola</label>
        <router-link :to="{ name: 'auth1.password-reset1' }" class="float-right">Şifrenizi mi unuttunuz?</router-link>
        <input type="password" class="form-control mb-0" id="exampleInputPassword1" placeholder="Parola">
      </div>
      <div class="d-inline-block w-100">
        <div class="custom-control custom-checkbox d-inline-block mt-2 pt-1">
          <input type="checkbox" class="custom-control-input" id="customCheck1">
          <label class="custom-control-label" for="customCheck1">Beni hatırla</label>
        </div>
        <button type="submit" class="btn btn-primary float-right" @click="$router.push({name: 'social.list'})">Giriş Yap</button>
      </div>
      <div class="sign-info">
        <span class="dark-color d-inline-block line-height-2">Hesabınız yok mu? <router-link :to="{ name: 'auth1.sign-up1'}">Kaydol</router-link></span>
      </div>
    </form>

  </div>
</template>

<script>

export default {
  name: 'SignIn1',
  data: () => ({}),
  mounted () {
  },
  methods: {
  }
}
</script>
