<template>
  <section>
    <b-sidebar
      v-model="open"
      type="is-success"
      :fullheight="fullheight"
      :fullwidth="fullwidth"
      :overlay="overlay"
      :right="right"
      mobile="fullWidth"
      class="is-flex is-flex-direction-column"
    >
      <!-- <form
        class="is-flex-grow-1"
        name="contact"
        method="POST"
        data-netlify="true"
      >
        <p>
          <label>Your Name: <input type="text" name="name" /></label>
        </p>
        <p>
          <label>Your Email: <input type="email" name="email" /></label>
        </p>
        <p>
          <label
            >Your Role:
            <select name="role[]" multiple>
              <option value="leader">Leader</option>
              <option value="follower">Follower</option>
            </select></label
          >
        </p>
        <p>
          <label>Message: <textarea name="message"></textarea></label>
        </p>
        <p>
          <button type="submit">Send</button>
        </p>
      </form> -->
      <!-- <b-menu>
          <b-menu-list label="Menu">
            <b-menu-item icon="information-outline" label="Info"></b-menu-item>
            <b-menu-item icon="settings">
              <template #label="props">
                Contact Options
                <b-icon
                  class="is-pulled-right"
                  :icon="props.expanded ? 'menu-down' : 'menu-up'"
                ></b-icon>
              </template>
              <b-menu-item icon="account" label="Users"></b-menu-item>
              <b-menu-item icon="cellphone-link">
                <template #label>
                  Devices
                  <b-dropdown
                    aria-role="list"
                    class="is-pulled-right"
                    position="is-bottom-left"
                  >
                    <template #trigger>
                      <b-icon icon="dots-vertical"></b-icon>
                    </template>
                    <b-dropdown-item aria-role="listitem"
                      >Action</b-dropdown-item
                    >
                    <b-dropdown-item aria-role="listitem"
                      >Another action</b-dropdown-item
                    >
                    <b-dropdown-item aria-role="listitem"
                      >Something else</b-dropdown-item
                    >
                  </b-dropdown>
                </template>
              </b-menu-item>
              <b-menu-item
                icon="cash-multiple"
                label="Payments"
                disabled
              ></b-menu-item>
            </b-menu-item>
            <b-menu-item icon="account" label="My Account">
              <b-menu-item label="Account data"></b-menu-item>
              <b-menu-item label="Addresses"></b-menu-item>
            </b-menu-item>
          </b-menu-list>
          <b-menu-list>
            <b-menu-item
              label="Expo"
              icon="link"
              tag="router-link"
              target="_blank"
              to="/expo"
            ></b-menu-item>
          </b-menu-list>
          <b-menu-list label="Actions">
            <b-menu-item label="Logout"></b-menu-item>
          </b-menu-list>
        </b-menu> -->

      <b-button class="button m-5" @click="open = false">Hide</b-button>
    </b-sidebar>
    <div class="block">
      <b-button class="button" @click="open = true">Contact</b-button>
      <!-- <b-field grouped group-multiline>
        <div class="control">
          <b-switch v-model="overlay">Overlay</b-switch>
        </div>
        <div class="control">
          <b-switch v-model="fullheight">Fullheight</b-switch>
        </div>
        <div class="control">
          <b-switch v-model="fullwidth">Fullwidth</b-switch>
        </div>
        <div class="control">
          <b-switch v-model="right">Right</b-switch>
        </div>
      </b-field> -->
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      open: false,
      overlay: true,
      fullheight: true,
      fullwidth: false,
      right: true,
      fullWidth: true,
    }
  },
}
</script>

<style>
.p-1 {
  padding: 1em;
}
.m-auto {
  margin-top: auto;
}
</style>
