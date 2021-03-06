<template>
  <div>
    <h1 class="mb-0">Kaydol</h1>
    <p>Bilgilerinizi girdikten sonra İnönü Sosyal'e kaydolabilirsiniz.</p>
    <form class="mt-4">
      <div class="form-group">
        <label for="exampleInputEmail1">Your Full Name</label>
        <input type="email" class="form-control mb-0" id="exampleInputEmail1" placeholder="Your Full Name">
      </div>
      <div class="form-group">
        <label for="exampleInputEmail2">Email address</label>
        <input type="email" class="form-control mb-0" id="exampleInputEmail2" placeholder="Enter email">
      </div>
      <div class="form-group">
        <label for="exampleInputPassword1">Password</label>
        <input type="password" class="form-control mb-0" id="exampleInputPassword1" placeholder="Password">
      </div>
      <div class="d-inline-block w-100">
        <div class="custom-control custom-checkbox d-inline-block mt-2 pt-1">
          <input type="checkbox" class="custom-control-input" id="customCheck1">
          <label class="custom-control-label" for="customCheck1"><a href="#">Şart ve koşulları</a>  kabul ediyorum</label>
        </div>
        <button type="submit" class="btn btn-primary float-right" @click="$router.push({name: 'social.list'})">Kaydol</button>
      </div>
      <div class="sign-info">
        <span class="dark-color d-inline-block line-height-2">Zaten bir hesabın var mı? <router-link :to="{ name: 'auth1.sign-in1'}">Giriş Yap</router-link></span>
      </div>
    </form>
  </div>
</template>
<script>

export default {
  name: 'SignUp1',
  data: () => ({}),
  methods: {
  }
}
</script>
