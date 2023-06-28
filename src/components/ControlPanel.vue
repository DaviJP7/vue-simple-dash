<script setup>
import List from "@/components/List.vue";
import items from '@/list-items.json'
</script>

<template>
  <div class="control-panel">
    <div class="head">
      <div class="title">Control panel</div>
      <div class="avatars">
        <div class="avatar">
          <img
            src="https://api.dicebear.com/6.x/lorelei/svg?seed=Toby"
            alt="avatar"
          />
        </div>
        <div class="avatar">
          <img
            src="https://api.dicebear.com/6.x/lorelei/svg?seed=Toby"
            alt="avatar"
          />
        </div>
        <div class="avatar">
          <img
            src="https://api.dicebear.com/6.x/lorelei/svg?seed=Toby"
            alt="avatar"
          />
        </div>
        <div class="avatar">+3</div>
      </div>
    </div>
    <input type="search" placeholder="Enter your search request..." />
  </div>
  <div>
    <div class="content-1">
      <div>B2B DISTRIBUITION</div>
      <small>Sales Deals</small>
    </div>
    <div class="content-2">
      <List :items="items"/>
    </div>
  </div>
</template>

<style scoped lang="scss">
.control-panel {
  margin-bottom: 3em;

  .head {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 1.5em;
    .title {
      font-size: 20pt;
    }
    .avatars {
      display: flex;
      .avatar {
        width: 45px;
        height: 45px;
        border: 3px solid #fff;
        background-color: #ccc;
        border-radius: 50%;
        margin-left: -18px;

        &:last-child {
          display: flex;
          justify-content: center;
          align-items: center;
          background-color: orange;
        }
      }
    }
  }
  input {
    width: 100%;
    border-radius: 2em;
    outline: none;
    border: none;
    background-color: #eee;
    font-size: 12pt;
    padding: 0.9em 2em;
  }


}
.content-1 {
    div {
      font-weight: bold;
    }
    border-bottom: 1.5px solid rgba(0, 0, 0, 0.2);
    padding-bottom: 1em;
  }

  .content-2 {
    overflow-y: auto;
    max-height: 375px;

    &::-webkit-scrollbar {
      width: 5px;
      background-color: #f5f5f5;
    }

    &::-webkit-scrollbar-thumb {
      border-radius: 10px;
      background-color: #ccc;
    }
    padding-top: 1.5em;
  }

</style>
