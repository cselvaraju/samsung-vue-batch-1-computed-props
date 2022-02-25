<template>
  <h1>Computed Props Demo</h1>
  Full Name: {{ firstName }} {{ lastName }}
  <br />
  Full Name: {{ firstName + " " + lastName }}
  <br />
  Full Name using Method: {{ fullNameMethod() }}
  <br />
  Full Name using Computed Prop: {{ fullNameComputedProp }}
  <p>
      <h3>Actor Details</h3>
      <p>{{ actor.name }}</p>
      <p>Movie Info: {{ movieInfo }} </p>
  </p>
</template>

<script>
export default {
  data() {
    return {
      firstName: "Amitabh",
      lastName: "Bachhan",
      actor: {
          name: 'Shashi Kapoor',
          movies: [
              'Deewar', 'Muqadda Ka Sikandar'
          ]
      }
    };
  },
  methods: {
    fullNameMethod() {
      return this.firstName + " " + this.lastName;
    },
  },
  computed: {
    fullNameComputedProp() {
      return this.firstName + " " + this.lastName;
    },
    movieInfo() {
        return this.actor.movies.length !== 0 ? this.actor.movies.length + ' movies' : 'No movies info!!'
    }
  },
};
</script>

<style>
</style>