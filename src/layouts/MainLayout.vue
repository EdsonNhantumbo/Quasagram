<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="bg-white text-grey-10" bordered>
      <q-toolbar>
       <q-btn
       to="/camera"
       class="q-mr-sm "
       icon="eva-camera-outline"
       size="18px"
       flat
       round
       dense
       />

       <q-separator
      spaced
       vertical
       />

        <q-toolbar-title class="text-grand-hotel">
          Quasargram
        </q-toolbar-title>

 <q-btn
       to="/"
       icon="eva-home-outline"
       size="18px"
       flat
       round
       dense
       />

      </q-toolbar>
    </q-header>

     <q-footer class="bg-white small-screen-only" bordered>
         <q-tabs class="text-grey-10" active-color="primary" indicator-color="transparent">
              <q-route-tab to="/" icon="eva-home-outline" />
              <q-route-tab to="/camera"  icon="eva-camera-outline"  />

         </q-tabs>
      </q-footer>

    <q-page-container class="bg-grey-1">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

export default {
  name: 'MainLayout',

  data () {
    return {

    }
  }
}
</script>

<style lang="sass">


.q-toolbar__title
$text-align: center
$font-size: 30px

.q-footer
.q-tab__icon
$font-size: 60px


</style>
