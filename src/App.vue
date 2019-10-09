<template lang='pug'>
v-app
  v-system-bar(absolute app window)
    span.mx-2.font-weight-bold Stick
    span.mx-2 File
    span.mx-2 Edit
    v-spacer
    v-icon mdi-minus
    v-icon mdi-checkbox-blank-outline
    v-icon mdi-close
  v-navigation-drawer(app)
    span file tree if folder selected
  v-content(app)
    HelloWorld
  v-footer(app)
    span.mx-2 cursor location
    v-spacer
    span.mx-2 language
    span.mx-2 spaces
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
    //
  }),
};
</script>
