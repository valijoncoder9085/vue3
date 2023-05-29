<template>
  <input type="text" v-focus />
</template>

<script>
const focus = {
  mounted: (el, bilding) => {
    console.log(el, bilding);
  },
};
export default {
  name: "SidebarComponent",
  directives: {
    focus,
  },
  data() {
    return {
      items: [
        { message: "Name", name: "Alijon" },
        { message: "Email", name: "Valijon" },
      ],
    };
  },
};
</script>
