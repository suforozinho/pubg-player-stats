<template>
<div class="online-players-table">
    <table v-if="error !== null">
        <tr>
            <td class="table-data">NAME</td>
            <td class="table-data">COUNTRY</td>
            <td class="table-data">PLATFORM</td>
            <td class="table-data">KILLS</td>
            <td class="table-data">DEATHS</td>
        </tr>
        <tr>
            <td class="table-data">{{ info.player.name }}</td>
            <td class="table-data">{{ info.player.countryName }}</td>
            <td class="table-data">{{ info.player.plat }}</td>
            <td class="table-data">{{ info.stats.kills }}</td>
            <td class="table-data">{{ info.stats.deaths }}</td>
        </tr>
    </table>
    <p v-else>ERROR!</p>
</div>
</template>

<script>
export default {
    props: ['info', 'error']
}
</script>
