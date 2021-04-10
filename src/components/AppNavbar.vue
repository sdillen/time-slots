<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <b-navbar-brand>
        time-slots
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-navbar-item-dropdown>
            <b-nav-item-dropdown text="User" right>
              <b-dropdown-item href="#">
                <b-icon icon="person"></b-icon>
                Profile
              </b-dropdown-item>
              <b-dropdown-item href="#">
                <b-icon icon="gear"></b-icon>
                Settings
              </b-dropdown-item>
            </b-nav-item-dropdown>
          </b-navbar-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'app-navbar'
}
</script>

<style>

</style>
