<template>
    <div class="time">

        {{ currentHours + ":" + currentMinutes }}
        
    </div>
</template>

<script>
import { mapState } from 'vuex'
export default {

    name: 'currentTime',

    computed: {

        ...mapState([
            'currentHours',
            'currentMinutes'
        ])

    }

}
</script>

<style scoped>
.time {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    padding: 20px 0;
}
</style>
