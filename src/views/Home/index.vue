<template>
    <section id="join-frame">
        <div class="progress"></div>
        <h1 class="title">Create Account</h1>
        <h3 class="sub-title">Glad to see you here!</h3>
        <form id="register" @submit="checkForm" action="" method="post">
            <div>
                <label :for="registerForm.account">Account</label>
                <input v-model="registerForm.account" type="text" placeholder="example@email.com">
            </div>
            <div>
                <label :for="registerForm.password">Password</label>
                <input v-model="registerForm.password" type="text" placeholder="●●●●●●●●">
            </div>
            <div>
                <label :for="registerForm.repassword">Comfirm Password</label>
                <input v-model="registerForm.repassword" type="text" placeholder="●●●●●●●●">
            </div>
            <div>
                <button>SUBMIT & NEXT</button>
            </div>
        </form>
    </section>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      registerForm: {
        account: '',
        password: '',
        repassword: ''
      }
    }
  }
}
</script>

<style lang="sass" src="../../assets/css/home.sass" scoped>
</style>
