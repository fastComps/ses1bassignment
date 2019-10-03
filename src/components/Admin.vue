<template>
  <div> 
    <fc-admin-hidden v-if="currentUser"></fc-admin-hidden> 
    <hr>
    <div class="row">
      <div class="col-sm-12 col-lg-6">
        <fc-login></fc-login>
      </div>
    </div>
  </div>
</template>

<script>
import NewProduct from "./NewProduct.vue";
import Login from "./Login.vue";
import { mapGetters } from "vuex"
import AdminHidden from './AdminHidden.vue'

export default {
  components: {
    fcLogin: Login,
    fcAdminHidden: AdminHidden
  },
  computed: {
    ...mapGetters([
      'currentUser'
    ])
  }
};
</script>

<style>
    .admin-purchase {
        padding-top: 50px;
    }
</style>