<script>
  export let meetups;
  import MeetupItem from "./MeetupItem.svelte";
</script>

{#each meetups as meetup}
  <MeetupItem
    title={meetup.title}
    subtitle={meetup.subtitle}
    image={meetup.imageUrl}
    address={meetup.address}
    description={meetup.description}
  />
{/each}

<style></style>
