<template>
  <div class="app">
    <AppHeader/>
    <div class="app-body">
      <Sidebar :navItems="nav"/>
      <main class="main">
        <breadcrumb :list="list"/>
             <div class="container-fluid">
          <router-view></router-view>
        </div>
      </main>
    </div>
    <AppFooter/>
  </div>
</template>

<script>
import nav from '../layouts/_nav'

import { Header as AppHeader, Sidebar, Footer as AppFooter, Breadcrumb } from '../components/'

export default {
  name: 'FullLayout',
  components: {
    AppHeader,
    Sidebar,
    AppFooter,
    Breadcrumb
  },
  data () {
    return {
      nav: nav.items
    }
  },
  computed: {
    name () {
      return this.$route.name
     },
    list () {
      return this.$route.matched
    }
  }
}
</script>
