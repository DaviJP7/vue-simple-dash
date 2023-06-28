<script setup>
import SideBar from "./components/SideBar.vue";
import Loader from "@/components/Loader.vue";
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
          <Loader />
        </div>
      </section>

      <section class="second-section">
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
            <ul>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
              <li>
                <div class="account-avatar">
                  <div class="avatar">C</div>
                  <div class="account">
                    <span class="emphasis">Cozy Home Funishings</span>
                    <small class="muted">520 items</small>
                  </div>
                </div>
                <div class="info">
                  <span class="emphasis">$11.190,00</span>
                  <small class="muted">Mon, Oct 14</small>
                </div>
              </li>
            </ul>
          </div>
        </div>
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
    gap: 1em;

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

  .second-section {
    display: flex;
    flex-direction: column;

    .control-panel {
      margin-bottom: 3em;
    }

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
      //   -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
      background-color: #ccc;
    }

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
    padding-top: 1.5em;
  }
}
</style>
