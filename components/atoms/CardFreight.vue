<template>
  <div class="card">
    <div class="header has-dflex flow-nw-row justify-between align-center">
      <p class="name">{{ name }}</p>
      <a href="#" class="choice">Escolher este</a>
    </div>
    <div class="content">
      <div class="prices">
        <p class="price">R$ 34,90</p>
        <span class="division"> em 2x de R$ 17,45 </span>
      </div>
      <div class="value has-dflex flow-row-nw align-center">
        <div class="icon has-dflex-center">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M2 8C2 7.20435 2.31607 6.44129 2.87868 5.87868C3.44129 5.31607 4.20435 5 5 5H11C11.7956 5 12.5587 5.31607 13.1213 5.87868C13.6839 6.44129 14 7.20435 14 8V16C14 16.2652 13.8946 16.5196 13.7071 16.7071C13.5196 16.8946 13.2652 17 13 17H9C8.73478 17 8.48043 16.8946 8.29289 16.7071C8.10536 16.5196 8 16.2652 8 16C8 15.7348 8.10536 15.4804 8.29289 15.2929C8.48043 15.1054 8.73478 15 9 15H12V8C12 7.73478 11.8946 7.48043 11.7071 7.29289C11.5196 7.10536 11.2652 7 11 7H5C4.73478 7 4.48043 7.10536 4.29289 7.29289C4.10536 7.48043 4 7.73478 4 8V14C4 14.2652 4.10536 14.5196 4.29289 14.7071C4.48043 14.8946 4.73478 15 5 15V17C4.20435 17 3.44129 16.6839 2.87868 16.1213C2.31607 15.5587 2 14.7956 2 14V8Z"
              fill="#7E1A44"
            />
            <path
              d="M12 9C12 8.73478 12.1054 8.48043 12.2929 8.29289C12.4804 8.10536 12.7348 8 13 8H17C17.2652 8.00006 17.5195 8.10545 17.707 8.293L21.121 11.707C21.6836 12.2695 21.9998 13.0324 22 13.828V14C22 14.7956 21.6839 15.5587 21.1213 16.1213C20.5587 16.6839 19.7956 17 19 17V15C19.2652 15 19.5196 14.8946 19.7071 14.7071C19.8946 14.5196 20 14.2652 20 14V13.828C19.9999 13.5628 19.8946 13.3085 19.707 13.121L16.586 10H14V15H15C15.2652 15 15.5196 15.1054 15.7071 15.2929C15.8946 15.4804 16 15.7348 16 16C16 16.2652 15.8946 16.5196 15.7071 16.7071C15.5196 16.8946 15.2652 17 15 17H13C12.7348 17 12.4804 16.8946 12.2929 16.7071C12.1054 16.5196 12 16.2652 12 16V9ZM7 15C6.73478 15 6.48043 15.1054 6.29289 15.2929C6.10536 15.4804 6 15.7348 6 16C6 16.2652 6.10536 16.5196 6.29289 16.7071C6.48043 16.8946 6.73478 17 7 17C7.26522 17 7.51957 16.8946 7.70711 16.7071C7.89464 16.5196 8 16.2652 8 16C8 15.7348 7.89464 15.4804 7.70711 15.2929C7.51957 15.1054 7.26522 15 7 15ZM4 16C4 15.606 4.0776 15.2159 4.22836 14.8519C4.37913 14.488 4.6001 14.1573 4.87868 13.8787C5.15726 13.6001 5.48797 13.3791 5.85195 13.2284C6.21593 13.0776 6.60603 13 7 13C7.39397 13 7.78407 13.0776 8.14805 13.2284C8.51203 13.3791 8.84274 13.6001 9.12132 13.8787C9.3999 14.1573 9.62087 14.488 9.77164 14.8519C9.9224 15.2159 10 15.606 10 16C10 16.7956 9.68393 17.5587 9.12132 18.1213C8.55871 18.6839 7.79565 19 7 19C6.20435 19 5.44129 18.6839 4.87868 18.1213C4.31607 17.5587 4 16.7956 4 16Z"
              fill="#7E1A44"
            />
            <path
              d="M17 15C16.7348 15 16.4804 15.1054 16.2929 15.2929C16.1054 15.4804 16 15.7348 16 16C16 16.2652 16.1054 16.5196 16.2929 16.7071C16.4804 16.8946 16.7348 17 17 17C17.2652 17 17.5196 16.8946 17.7071 16.7071C17.8946 16.5196 18 16.2652 18 16C18 15.7348 17.8946 15.4804 17.7071 15.2929C17.5196 15.1054 17.2652 15 17 15ZM14 16C14 15.2044 14.3161 14.4413 14.8787 13.8787C15.4413 13.3161 16.2044 13 17 13C17.7956 13 18.5587 13.3161 19.1213 13.8787C19.6839 14.4413 20 15.2044 20 16C20 16.7956 19.6839 17.5587 19.1213 18.1213C18.5587 18.6839 17.7956 19 17 19C16.2044 19 15.4413 18.6839 14.8787 18.1213C14.3161 17.5587 14 16.7956 14 16Z"
              fill="#7E1A44"
            />
          </svg>
        </div>
        <p>Frete: R$ 9,90 <span>(estimado) em até 15 dias úteis</span></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
  },
}
</script>

<style lang="scss" scoped>
.card {
  padding: 0 1rem;
  box-shadow: 0px 0px 0px 1px $gray-06;
  border-radius: $bdr-small;

  .header {
    padding: 1rem 0 0.75rem 0;
    border-bottom: 1px solid $gray-08;

    .name {
      font-weight: 600;
      color: $gray-01;
    }

    .choice {
      font-size: 0.75em;
      color: $aux-blue-d;
      line-height: 18px;
      text-decoration: none;
    }
  }

  .content {
    padding: 1rem 0 0.75rem 0;
    gap: 0.5rem;

    .prices {
      .price {
        font-size: 1.125em;
        font-weight: 500;
        line-height: 18px;
        color: $gray-01;
      }

      .division {
        font-size: 0.75em;
        line-height: 18px;
        color: $gray-05;
      }
    }

    .value {
      p {
        font-size: 0.75em;
        line-height: 18px;
        color: $gray-01;

        span {
          color: $gray-05;
        }
      }
    }
  }
}
</style>
