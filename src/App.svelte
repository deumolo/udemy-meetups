<script>
  import Header from "./UI/Header.svelte";
  import meetups from "./meetups.js";
  import MeetupGrid from "./Meetups/MeetupGrid.svelte";
</script>

<Header />

<section id="meetups">
    <MeetupGrid {meetups} />    
</section>

<style>
  #meetups {
    margin-top: 50px;
    margin-bottom: 50px;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 1rem;
  }
</style>
