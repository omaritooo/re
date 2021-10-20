<template>
  <div>
    <model-obj :src="file" mtl="../test1.mtl"></model-obj>
  </div>
</template>
<script>
import { ModelObj } from "vue-3d-model";
import file from "../assets/test1.obj";
export default {
  components: { ModelObj },
  data() {
    return;
    {
      file: file;
    }
  },
  mounted: function () {
    console.log(this.file);
  },
};
</script>