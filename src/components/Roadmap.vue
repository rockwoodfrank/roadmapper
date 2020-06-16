<template>
  <main class="roadmap dark-text-1">
    <h1 class="roadmap__name">{{ roadmap.name }}</h1>
    <section class="milestone" v-for = "(landmark, index) in roadmap.landmarks" v-bind:key = "index">
      <!-- TODO: Add Line tool -->
      <PathChild v-bind:landmark = "landmark"/>
    </section>
    
  </main>
</template>

<script>
import PathChild from '@/components/PathChild.vue'

export default {
  name: "Roadmap",
  data() {
    return {
      roadmap: {
        name: "Back-end",
        landmarks: [
          {
            name: "Pick a Language",
            children: [
              {
                name: "Node.js",
              },
              {
                name: "Python",
              },
              {
                name: "Scala",
              },
              {
                name: "Ruby",
              },
              {
                name: "PHP",
              },
              {
                name: "Haskell",
              }
            ],
            // TODO: add markdown support
            info: "Picking a first language is very important!",
            completion: 50,
          },
          {
            name: "Version Control"
          }
        ]
      }
    };
  },
  components: {
    PathChild,
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
