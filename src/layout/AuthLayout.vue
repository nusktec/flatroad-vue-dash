<template>
    <div class="main-content bg-default">
        <!-- Header -->
        <div class="header py-7 py-lg-8">
            <div class="container">
                <div class="header-body text-center mb-5">
                    <div class="row justify-content-center">
                        <div class="col-lg-5 col-md-2">
                            <h1 class="text-white">Welcome !</h1>
                            <h3 class="text-lead text-white">Work and Connect Console App</h3>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Page content -->
        <div class="container mt--8 pb-5">
            <slide-y-up-transition mode="out-in" origin="center top">
                <router-view></router-view>
            </slide-y-up-transition>
        </div>
    </div>
</template>
<script>
  import { SlideYUpTransition } from 'vue2-transitions'
  export default {
    name: 'auth-layout',
    components: {
      SlideYUpTransition
    },
    data() {
      return {
        year: new Date().getFullYear(),
        showMenu: false
      }
    },
  }
</script>
<style>
</style>
