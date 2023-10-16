<template>
  <q-layout view="hHh lpR fFf">
    <q-header
      elevated
      class="text-white"
      height-hint="98"
      style="background-color: #809ddf; padding-top: 20px"
    >
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />

        <q-toolbar-title> Exams Corner </q-toolbar-title>
      </q-toolbar>

      <q-tabs align="center">
        <q-route-tab no-caps to="/page1" label="Notes " />
        <q-route-tab no-caps to="/page2" label="Exam" />
        <q-route-tab no-caps to="/page3" label="Schemes of Work" />
        <q-route-tab no-caps to="/page2" label="Q&A" />
        <q-route-tab no-caps to="/page2" label="Video Lessons" />
        <q-route-tab no-caps to="/page2" label="Question Papers" />
        <q-route-tab no-caps to="/page2" label="Colleges" />
        <q-route-tab no-caps to="/page2" label="Universities" />
        <q-route-tab no-caps to="/page2" label="Courses" />
        <q-route-tab no-caps to="/page2" label="Resources" />
      </q-tabs>
      <q-tabs align="right">
        <q-route-tab no-caps to="/page1" label="Login " />
        <q-route-tab no-caps to="/page1" label="Register " />
      </q-tabs>
    </q-header>

    <q-drawer show-if-above v-model="leftDrawerOpen" side="left" bordered>
      <!-- drawer content -->
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const leftDrawerOpen = ref(false);

    return {
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
};
</script>
