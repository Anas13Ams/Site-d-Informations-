<template>
  <div class="card-list">
    <span class="card-title">{{ event.title }} </span>
    <img class="card-img" :src="event.galery_pictures" />
    <span>{{ event.content }} </span>
    <span class="price">{{ event.price }} €.TTC </span>
    <span class="date">{{ event.date }}</span>
    <router-link :to="routePath" class="button">Plus d'information</router-link>
  </div>
</template>
<script>
export default {
  name: "EventList",
  props: { event: Object },
  data() {
    return { routePath: "/events/" + this.event.id };
  },
};
</script>
<style scoped>
.card-img {
  margin-left: 10px;
}
</style>
