<template>
  <div class="online-players-table">
    <table>
      <tr>
        <th class="table-data" colspan="5">Online Players</th>
      </tr>
      <tr>
        <td class="table-data">PC</td>
        <td class="table-data">PS3</td>
        <td class="table-data">PS4</td>
        <td class="table-data">XBOX 360</td>
        <td class="table-data">XBOX One</td>
      </tr>
      <tr>
        <td class="table-data">{{ info.pc.count }}</td>
        <td class="table-data">{{ info.ps3.count }}</td>
        <td class="table-data">{{ info.ps4.count }}</td>
        <td class="table-data">{{ info.xbox.count }}</td>
        <td class="table-data">{{ info.xone.count }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  props: ['info']
}
</script>

<style>
.online-players-table {
  display: flex;
  justify-content: center;
}

.table-data {
  padding: 1px 21px;
  border: 1px solid white;
  text-align: center;
}
</style>
