<template>
  <q-footer elevated class="bg-grey-9" v-if="$q.screen.lt.md">
    <q-tabs
      dense
      class="shadow-2"
      active-color="primary"
      align="justify"
    >
      <q-route-tab icon="view_list" :label="$t('task-list')" to="/task">
        <!--        <q-badge color="primary" text-color="white" floating>2</q-badge>-->
      </q-route-tab>
<!--      <q-route-tab icon="video_library" :label="$t('media')" to="/task">-->
      <q-route-tab icon="stop" :label="$t('stopped')" to="/task/stopped">
        <!--        <q-badge color="primary" text-color="white" floating>2</q-badge>-->
<!--      </q-route-tab>-->
        <!--        <q-badge color="purple" text-color="white" floating>10+</q-badge>-->
      </q-route-tab>
      <q-route-tab icon="settings_applications" :label="$t('Settings')" to="/preference" />
    </q-tabs>
  </q-footer>
</template>
