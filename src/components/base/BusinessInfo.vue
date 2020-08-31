<template>
  <v-theme-provider :dark="dark">
    <div>
      <base-info-card
        title="KEEP IN TOUCH WITH US"
        pace="6"
      >
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illo pariatur quidem, quis modi iure nihil commodi suscipit, corporis dicta adipisci, voluptatum quia cupiditate. Nulla minus voluptatum nostrum deleniti, asperiores facere.
      </base-info-card>

      <base-business-contact dense />
    </div>
  </v-theme-provider>
</template>

<script>
  export default {
    name: 'BaseBusinessInfo',

    props: { dark: Boolean },

    data: () => ({
      business: [
        {
          icon: 'mdi-map-marker-outline',
          title: 'Address',
          text: '1227 Hawthorne Ave.<br>Columbus, Ohio 43203',
        },
        {
          icon: 'mdi-cellphone',
          title: 'Phone',
          text: '614.400.4356',
        },
        {
          icon: 'mdi-email',
          title: 'Email',
          text: 'contact@elementalblockchain.com<br>heather@vuetifyjs.com',
        },
      ],
    }),
  }
</script>
