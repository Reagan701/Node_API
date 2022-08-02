<template>
  <div id="main" class="login">
      <h1 class="text-light">This is a Login page</h1>
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col-lg-4 col-md-6 col-sm-6">
          <div class="card shadow">
            <div class="card-title text-center border-bottom">
            <h2 class="p-3">Login</h2>
            </div>
            <div class="card-body">
            <form>
              <div class="mb-4">
                <label for="username" class="form-label">Email</label>
                <input type="text" class="form-control" id="username" />
              </div>
              <div class="mb-4">
                <label for="password" class="form-label">Password</label>
                <input type="password" class="form-control" id="password" />
              </div>
              <div class="mb-4">
                <input type="checkbox" class="form-check-input" id="remember" />
                <label for="remember" class="form-label">Remember Me</label>
              </div>
              <div class="d-grid">
                <button type="submit" class="btn bg-primary text-dark">Login</button>
              </div>
            </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
:root{
  --main-bg: ;
}

.main-bg {
  background: var(--main-bg) !important;
}

#main{
  background-image: linear-gradient(50deg, #0014a9, #ff0000);
  padding: 175px 0 175px 0;
}

input:focus, button:focus {
  border: 1px solid var(--main-bg) !important;
  box-shadow: none !important;
}

.form-check-input:checked {
  background-color: var(--main-bg) !important;
  border-color: var(--main-bg) !important;
}

.card, .btn, input{
  border-radius:0 !important;
}

</style>
