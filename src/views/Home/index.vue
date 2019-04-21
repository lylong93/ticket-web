<template>
  <div class="HomeWrapper">
     <HomeHead/>
     <HomeDrawer/>
  </div>
</template>

<script>
import HomeHead from "./HomeHead";
import HomeDrawer from "./HomeDrawer";
export default {
  data() {
    return {
      name: "one"
    };
  },
  components: {
    HomeHead,
    HomeDrawer
  }
};
</script>
<style lang="scss" scoped>
.HomeWrapper {

}
</style>

