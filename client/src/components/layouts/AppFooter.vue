<template>
  <footer class="page-footer orange">
    <div class="container">
      <div class="row">
        <div class="col l6 s12">
          <h5 class="white-text">Bio Kita</h5>
          <p class="grey-text text-lighten-4">Kami Adalah Pengembang Yang Sedang Belajar.</p>


        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Setting</h5>
          <ul>
            <li><a class="white-text" href="#!">Link 1</a></li>
            <li><a class="white-text" href="#!">Link 2</a></li>
            <li><a class="white-text" href="#!">Link 3</a></li>
            <li><a class="white-text" href="#!">Link 4</a></li>
          </ul>
        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Kontak</h5>
          <ul>
            <li><a class="white-text" href="#!">Link 1</a></li>
            <li><a class="white-text" href="#!">Link 2</a></li>
            <li><a class="white-text" href="#!">Link 3</a></li>
            <li><a class="white-text" href="#!">Link 4</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">
        Made by <a class="orange-text text-lighten-3" href="http://materializecss.com">Materialize</a>
      </div>
    </div>
  </footer>
</template>

<script>

  import axios from "axios"
  import swal from "sweetalert2"
  import store from "../../vuex/store"

  export default {
    name: "AppFooter",

    data() {
      return {
        page: 0,
      }
    },

    computed: {

      user: function () {
        return store.getters.getUser
      },

      login: function () {
        return store.getters.getLogin
      }
    },
  }
</script>