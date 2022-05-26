<template>
  <div id="app">
      <div id="main-wrapper">
        <Header />
        <Sidebar />
        <div class="page-wrapper">
          <div class="container-fluid">
            <Breadcrumbs />
            <div class="row">
              <div class="col-12">
                  <div class="card">
                      <div class="card-body">
                          <router-outlet></router-outlet>
                      </div>
                  </div>
              </div>
            </div>
          </div>
          <footer class="footer">
            © 2017 Admin Pro by wrappixel.com
          </footer>
        </div>
      </div>
  </div>
</template>

<script>
import Header from './components/shared/HeaderComponent.vue'
import Breadcrumbs from './components/shared/BreadcrumbsComponent.vue'
import Sidebar from './components/shared/SidebarComponent.vue'

export default {
  name: 'App',
  components: {
    Header,
    Breadcrumbs,
    Sidebar
  }
}
</script>

<style>
/*#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}*/
</style>
