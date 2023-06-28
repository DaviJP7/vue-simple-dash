<script setup>
import HomeIcon from "vue-material-design-icons/Home.vue";
import ListBoxIcon from "vue-material-design-icons/ListBox.vue";
import ChartBarIcon from "vue-material-design-icons/ChartBar.vue";
import CogIcon from "vue-material-design-icons/Cog.vue";
</script>

<template>
  <aside>
    <div class="logo"></div>
    <ul>
      <li class="active">
        <a href="#"><HomeIcon /></a>
      </li>
      <li>
        <a href="#">
          <ListBoxIcon />
        </a>
      </li>
      <li>
        <a href="#">
          <ChartBarIcon />
        </a>
      </li>
      <li>
        <a href="#">
          <CogIcon />
        </a>
      </li>
    </ul>
    <div class="profile">
      <a href="javascript:void(0)" title="Profile">
        <img
          src="https://api.dicebear.com/6.x/lorelei/svg?seed=Cali"
          alt="avatar"
        />
      </a>
    </div>
  </aside>
</template>

<style scoped>
aside {
  padding: 2em;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  .logo {
    width: 50px;
    height: 50px;
    background-color: #000;
    border-radius: 50%;
    position: relative;
    &::after {
      content: "";
      display: block;
      width: 15px;
      height: 15px;
      border-top-right-radius: 100%;
      border-bottom-left-radius: 100%;
      position: absolute;
      left: 35%;
      top: 34%;
      background-color: limegreen;
      animation: animelogo 4s infinite;
    }
  }

  & > ul {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 3em;

    & > li {
      color: rgba(0, 0, 0, 0.3);
      &.active {
        color: #000;
      }
      & > a {
        color: inherit;
        text-decoration: none;
      }
    }
  }

  & .profile {
    width: 45px;
    height: 45px;
    border: 1px solid rgba(0, 0, 0, 0.6);
    border-radius: 50%;
  }
}
@keyframes animelogo {
  0% {
    rotate: 0deg;
  }
  50% {
    rotate: 90deg;
  }
  100% {
    rotate: 0deg;
  }
}
</style>
