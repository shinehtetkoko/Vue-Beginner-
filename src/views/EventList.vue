<template>
  <h1>Event for good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event='event'/>
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard
  },
   data(){
        return{
            events:[
              {
                id:5928101,
                category:'animal walfare',
                title:'Meow day',
                description:'find new feline at this event',
                location:'Meow Twon',
                date:'January 21 2028',
                time:'12:00',
                petsAllowed:'true',
                organizer:'Kat laydee'
                },
                {
                id:5928101,
                category:'animal Denied',
                title:'Meow the Best day',
                description:'find new feline at this event',
                location:'Meow Twon',
                date:'January 21 2028',
                time:'12:00',
                petsAllowed:'true',
                organizer:'Kat laydee'
                },
                {
                id:5928101,
                category:'animal welcome',
                title:'cat adoption day',
                description:'find new feline at this event',
                location:'Meow Twon',
                date:'January 21 2028',
                time:'12:00',
                petsAllowed:'true',
                organizer:'Kat laydee'
                },
            ]
        }
    }
};
</script>
<style scoped>
.events{
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
