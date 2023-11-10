<template>
    <div class="event-card">
        <h2>{{ event.title }}</h2>
        <p>{{ event.description }}</p>

    </div>
</template>
<script>
export default {
    name: 'EventCard',
    props: {
        event: {
            type: Object,
            required: true
        }
    }
}
</script>
<style scoped>
.event-card {
    background-color: aliceblue;
    border: 1px solid gray;
    border-radius: 4px;
    box-shadow: 1px 2px 4px lightgray;
    padding: 1rem;
    margin-bottom: 1rem;
    width: 300px;
}

.event-card:hover {
    cursor: pointer;
    transform: scale(1.02);
    transition: transform .3s;
}
</style>