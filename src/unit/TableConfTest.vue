<template>
  <div class="MatcLight">
    <h1>TabelConf Test</h1>

    <div class="dialog">
      <TableSettings :app="app" :value="widget"/>
    </div>


  </div>
</template>

<style>
  @import url("../style/matc.css");

  .dialog {
    padding: 20px;
    width: 840px;
    margin: 20px;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.2)
  }
</style>

<script>

import app from './data/tableapp.json'
import TableSettings from 'canvas/toolbar/TableSettings'

export default {
  name: "SketchTest",
  mixins: [],
  data: function() {
    return {
        app: app,
        widget: app.widgets.w10868,
        model: null
    };
  },
  components: {
    'TableSettings': TableSettings
  },
  computed: {
  },
  methods: {
  },
  mounted() {
  }
};
</script>
