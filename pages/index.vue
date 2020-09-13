<template>
  <div>
    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /
        </div>
        <div class="col-md-6">
          <button @click="example()">Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{}"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" v-model="exampleContent" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /register
        </div>
        <div class="col-md-6">
          <button @click="register()">Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{ email: '', password: '' }"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /login
        </div>
        <div class="col-md-6">
          <button @click="login()">Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{ email: '', password: '' }"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" v-model="loginContent" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /logout
        </div>
        <div class="col-md-6">
          <button @click="logout()">Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{}"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row mt-3">
        <div class="col-md-6">
          url: /changepassword
        </div>
        <div class="col-md-6">
          <button @click="changePassword()">Fetch</button>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="{ oldpassword: '' }"></textarea>
        </div>
        <div class="col-md-6 mt-3">
          <textarea class="w-100 p-2" rows="5" placeholder="Results..."></textarea>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  components: {},
  data() {
    return {
      exampleContent: '',
      loginContent: '',
    }
  },
  methods: {
    example: function () {
      var data = {}

      var headers = {      
        'Content-Type': 'application/json;charset=UTF-8',
      }

      const self = this

      axios.get('https://cors-anywhere.herokuapp.com/https://powerful-thicket-49412.herokuapp.com/', data, headers)
        .then(function (response) {
          console.log(response.data);
          self.exampleContent = response.data
          alert('Fetch successful.')
        })
        .catch(function (error) {
          console.log(error);
          // self.example = error
          alert('Could not fetch.')
        });
    },
    register: function () {
      var data = {
        email: 'bird@gmail.com',
        password: 'abcd1234'
      }

      var headers = {      
        'Content-Type': 'application/json;charset=UTF-8',
      }

      const self = this

      axios.post('https://cors-anywhere.herokuapp.com/powerful-thicket-49412.herokuapp.com/register', data, headers)
        .then(function (response) {
          console.log(response.data);
          this.example = response.data
          alert('You are logged in as ' + response.data + '.')
        })
        .catch(function (error) {
          console.log(error);
          alert('Could not login.')
        });
    },
    login: function () {
      var data = {
        email: 'ritwikaghosh48@gmail.com',
        password: 'abcd1234'
      }

      var headers = {      
        'Content-Type': 'application/json;charset=UTF-8',
      }

      const self = this

      axios.post('https://powerful-thicket-49412.herokuapp.com/login', data, headers)
        .then(function (response) {
          console.log(response.data);
          self.loginContent = response.data
          alert('You are logged in as ' + response.data + '.')
        })
        .catch(function (error) {
          console.log(error);
          alert('Could not login.')
        });
    },
    logout: function () {
      var data = {}

      var headers = {      
        'Content-Type': 'application/json;charset=UTF-8',
      }

      const self = this

      axios.get('https://cors-anywhere.herokuapp.com/https://powerful-thicket-49412.herokuapp.com/logout', data, headers)
        .then(function (response) {
          console.log(response.data);
          alert('You logged out.')
        })
        .catch(function (error) {
          console.log(error);
          alert('Could not logout.')
        });
    },
    changePassword: function () {
      var data = {
        oldpassword: 'abcd1234',
        newpassword: 'abcd12345'
      }

      var headers = {      
        'Content-Type': 'application/json;charset=UTF-8',
      }

      const self = this

      axios.post('https://powerful-thicket-49412.herokuapp.com/changepassword', data, headers)
        .then(function (response) {
          console.log(response.data);
          alert('You logged out.')
        })
        .catch(function (error) {
          console.log(error);
          alert('Could not logout.')
        });
    }
  },
}
</script>

<style>
</style>
