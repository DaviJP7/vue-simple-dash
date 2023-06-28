<script setup>
import SideBar from "./components/SideBar.vue";
import ArrowRightThinIcon from "vue-material-design-icons/ArrowRightThin.vue";
</script>

<template>
  <main>
    <SideBar />
    <div class="content">
      <section class="first-section">
        <div class="card card-sales">
          <div class="card-head">
            <div class="card-title">Sales Activity</div>
            <button class="btn">Details</button>
          </div>
          <div class="card-body">
            <small>
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptatum voluptate non, laudantium quaerat vel deleniti vitae
              ullam repellat corrupti veniam culpa perferendis qui et laboriosam
              neque molestiae, iusto obcaecati. Hic.
            </small>
          </div>
        </div>
        <div class="card card-primary">
          <div class="card-head">
            <div class="card-title">Team Rating</div>
            <button class="btn">
              <ArrowRightThinIcon />
            </button>
          </div>
          <div class="card-body">
            <div class="avatars">
              <div class="avatar">
                <img
                  src="https://api.dicebear.com/6.x/lorelei/svg?seed=Sophie"
                  alt="avatar"
                />
              </div>
              <div class="avatar">
                <img
                  src="https://api.dicebear.com/6.x/lorelei/svg?seed=Lucky"
                  alt="avatar"
                />
              </div>
              <div class="avatar">
                <img
                  src="https://api.dicebear.com/6.x/lorelei/svg?seed=Muffin"
                  alt="avatar"
                />
              </div>
            </div>
          </div>
        </div>
        <div class="card card-skeleton">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="38"
            height="38"
            viewBox="0 0 38 38"
          >
            <defs>
              <linearGradient
                x1="8.042%"
                y1="0%"
                x2="65.682%"
                y2="23.865%"
                id="a"
              >
                <stop stop-color="#fff" stop-opacity="0" offset="0%" />
                <stop stop-color="#fff" stop-opacity=".631" offset="63.146%" />
                <stop stop-color="#fff" offset="100%" />
              </linearGradient>
            </defs>
            <g fill="none" fill-rule="evenodd">
              <g transform="translate(1 1)">
                <path
                  d="M36 18c0-9.94-8.06-18-18-18"
                  id="Oval-2"
                  stroke="url(#a)"
                  stroke-width="2"
                >
                  <animateTransform
                    attributeName="transform"
                    type="rotate"
                    from="0 18 18"
                    to="360 18 18"
                    dur="0.9s"
                    repeatCount="indefinite"
                  />
                </path>
                <circle fill="#fff" cx="36" cy="18" r="1">
                  <animateTransform
                    attributeName="transform"
                    type="rotate"
                    from="0 18 18"
                    to="360 18 18"
                    dur="0.9s"
                    repeatCount="indefinite"
                  />
                </circle>
              </g>
            </g>
          </svg>
        </div>
      </section>

      <section class="second-section">
        <!-- <div class="control-panel">
          <div>Control panel</div>
          <div>photos</div>
        </div>
        <div>
          <div class="content-1">
            <div>B2B DISTRIBUITION</div>
            <small>Sales Deals</small>
          </div>
          <div class="content-2">
            <ul>
              <li>Cozy Home Funishings</li>
            </ul>
          </div>
        </div> -->
      </section>
    </div>
  </main>
</template>

<style scoped lang="scss">
main {
  display: flex;
  .content {
    display: flex;
    padding-top: 2em;
    padding-left: 130px;
    height: 100vh;
    width: 100%;
    gap: 2em;

    section.first-section {
      width: 65%;
      display: grid;
      grid-template-rows: 1fr 1fr;
      grid-template-columns: 1fr 1fr;
      gap: 1.5em;
    }

    section.second-section {
      width: 35%;
      display: flex;
      padding: 2em;
    }

    .card {
      padding: 2em;
      border-radius: 1em;
      width: 100%;

      .card-head {
        display: flex;
        justify-content: space-between;
        align-items: center;
        button {
          text-transform: uppercase;
          border-radius: 1em;
          padding: 5px 0.9em;
          font-size: 11pt;
          background-color: $primary;
          border: none;
          font-weight: bold;
          cursor: pointer;
        }
      }

      &.card-sales {
        color: #fff;
        background-color: #000;
        min-height: 350px;
        grid-row-start: 1;
        grid-column-start: 1;
        grid-row-end: 2;
        grid-column-end: 3;

        .card-title {
          font-size: 40pt;
        }

        .card-body {
          margin-top: 1em;
          small {
            display: block;
            color: rgba(255, 255, 255, 0.6);
            width: 70%;
          }
          img {
            margin-top: 1em;
            width: 350px;
            border-radius: 1em;
          }
        }
      }

      &.card-primary {
        background-color: rgb(24, 140, 242);
        height: 250px;
        color: #fff;
        .card-head {
          border-bottom: 1px solid #fff;
          padding-bottom: 1em;

          button {
            font-weight: normal;
            font-size: 10pt;
            padding: 0 2em;
          }

          .card-title {
            font-size: 12pt;
            font-weight: bold;
          }
        }

        .avatars {
          display: flex;
          justify-content: space-around;
          margin-top: 2em;
          .avatar {
            border: 1px solid rgba(0, 0, 0, 0.5);
            border-radius: 50%;
            width: 80px;
            background-color: #ccc;
          }
        }
      }

      &.card-skeleton {
        background-color: #ccc;
        height: 250px;
        display: grid;
        place-content: center;
      }
    }
  }
}
</style>
