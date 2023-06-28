<script setup>
    defineProps({
        items: {
            type: Array,
            required: true,
        }
    })
</script>

<template>
  <ul>
    <li v-for="item in items" :key="item">
      <div class="account-avatar">
        <div class="avatar">{{ item.avatar }}</div>
        <div class="account">
          <span class="emphasis">{{ item.name }}</span>
          <small class="muted">{{ item.tot_items }} items</small>
        </div>
      </div>
      <div class="info">
        <span class="emphasis">{{ item.price }}</span>
        <small class="muted">{{ item.date }}</small>
      </div>
    </li>
  </ul>
</template>

<style scoped lang="scss">
ul {
  margin-right: 10px;
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 1.5em;
  li {
    display: flex;
    align-items: center;
    justify-content: space-between;

    .account-avatar {
      display: flex;
      gap: 1em;
      align-items: center;
    }

    .avatar {
      width: 45px;
      height: 45px;
      border-radius: 50%;
      background-color: #eee;
      display: grid;
      place-content: center;
      font-weight: bold;
    }

    .account,
    .info {
      display: flex;
      flex-direction: column;
      gap: 0.4em;
    }

    .info {
      text-align: right;
    }

    .emphasis {
      font-weight: bold;
      font-size: 10pt;
    }
    .muted {
      color: rgba(0, 0, 0, 0.6);
    }
  }
}
</style>
