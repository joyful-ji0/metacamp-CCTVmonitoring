<template>
  <div>
    <b-container fluid style="padding: 0px">
      <b-row>
        <!-- Side bar -->
        <b-col id="index-sidebar" cols="2" style="padding: 0">
          <app-sidebar />
        </b-col>
        <!-- Body Contents -->
        <b-col id="index-content-body" style="padding-left: 0px; padding-right: 0px">
          <div class="content-body">
            <router-view />
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Sidebar from '../components/layout/Sidebar'

export default {
  components: {
    'app-sidebar': Sidebar
  }
}
</script>

<style lang="scss" scoped></style>
