<template>
  <aside class="menu-context">
    <div class="modal has-dflex flow-nw-col justify-between">
      <div class="top">
        <div class="head">
          <div class="row">
            <div class="col">
              <ProviderAdminUserMenu
                userImage="user/userimage.jpg"
                userName="São Luiz"
              />
            </div>
          </div>
        </div>
        <div class="main">
          <ProviderMenuList />
        </div>
      </div>
      <div class="foot">
        <provider-admin-menu-item>
          <template v-slot:content>
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M6 3C5.20435 3 4.44129 3.31607 3.87868 3.87868C3.31607 4.44129 3 5.20435 3 6V18C3 18.7956 3.31607 19.5587 3.87868 20.1213C4.44129 20.6839 5.20435 21 6 21H11C11.2652 21 11.5196 20.8946 11.7071 20.7071C11.8946 20.5196 12 20.2652 12 20C12 19.7348 11.8946 19.4804 11.7071 19.2929C11.5196 19.1054 11.2652 19 11 19H6C5.73478 19 5.48043 18.8946 5.29289 18.7071C5.10536 18.5196 5 18.2652 5 18V6C5 5.73478 5.10536 5.48043 5.29289 5.29289C5.48043 5.10536 5.73478 5 6 5H11C11.2652 5 11.5196 4.89464 11.7071 4.70711C11.8946 4.51957 12 4.26522 12 4C12 3.73478 11.8946 3.48043 11.7071 3.29289C11.5196 3.10536 11.2652 3 11 3H6Z"
                fill="#7E1A44"
              />
              <path
                d="M15.293 7.29279C15.4805 7.10532 15.7348 7 16 7C16.2652 7 16.5195 7.10532 16.707 7.29279L20.707 11.2928C20.8945 11.4803 20.9998 11.7346 20.9998 11.9998C20.9998 12.265 20.8945 12.5193 20.707 12.7068L16.707 16.7068C16.5184 16.8889 16.2658 16.9897 16.0036 16.9875C15.7414 16.9852 15.4906 16.88 15.3052 16.6946C15.1198 16.5092 15.0146 16.2584 15.0123 15.9962C15.01 15.734 15.1108 15.4814 15.293 15.2928L17.586 12.9998H10C9.73478 12.9998 9.48043 12.8944 9.29289 12.7069C9.10536 12.5194 9 12.265 9 11.9998C9 11.7346 9.10536 11.4802 9.29289 11.2927C9.48043 11.1051 9.73478 10.9998 10 10.9998H17.586L15.293 8.70679C15.1055 8.51926 15.0002 8.26495 15.0002 7.99979C15.0002 7.73462 15.1055 7.48031 15.293 7.29279V7.29279Z"
                fill="#7E1A44"
              />
            </svg>
            <p>Sair</p>
          </template>
        </provider-admin-menu-item>
      </div>
    </div>
    <div class="bg" @click="removeActive"></div>
  </aside>
</template>

<script>
export default {
  methods: {
    removeActive() {
      document.querySelector('.menu-context').classList.remove('active')
    },
  },
}
</script>

<style lang="scss" scoped>
.menu-context {
  z-index: -1;
  width: 100%;
  height: 100vh;
  position: fixed;
  top: 0;
  right: 0;

  .modal {
    z-index: 2;
    width: 100%;
    max-width: 18.75rem;
    height: 100%;
    position: relative;
    padding: 2rem 1.5rem 0 1.5rem;
    background-color: $pri-d;
    transform: translateX(-100%);
    transition-duration: $tsd;
    transition-property: transform;
    transition-timing-function: $ttf;

    .main {
      padding: 20% 0 0 0;
    }

    .foot {
      padding: 0 0 40% 0;
    }
  }

  .bg {
    z-index: 1;
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    transition-duration: $tsd;
    transition-property: background-color;
    transition-timing-function: $ttf;
  }

  &.active {
    z-index: 10;
    .modal {
      transform: translate(0);
    }
    .bg {
      background-color: rgba(0, 0, 0, 0.5);
    }
  }
}

// iPad - 768px
@media screen and (max-width: 48rem) {
  .context-cart {
    .modal {
      max-width: 85%;
    }
  }
}
</style>
