<template>
  <base-section
    id="features"
    class="secondary"
  >
    <v-responsive
      class="mx-auto"
      max-width="1350"
    >
      <v-container fluid>
        <v-row>
          <v-col
            v-for="card in cards"
            :key="card.title"
            cols="12"
            sm="4"
            md="3"
          >
            <base-info-card
              align="center"
              dark
              v-bind="card"
            />
          </v-col>
        </v-row>
      </v-container>
    </v-responsive>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionFeatures',

    data: () => ({
      cards: [
        {
          icon: 'mdi-keyboard-outline',
          title: 'Crypto Currency',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt porta elit, ac scelerisque eros ullamcorper vitae.',
        },
        {
          icon: 'mdi-camera-outline',
          title: 'Decentralized',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt porta elit, ac scelerisque eros ullamcorper vitae.',
        },
        {
          icon: 'mdi-pencil-outline',
          title: 'Immutability',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt porta elit, ac scelerisque eros ullamcorper vitae.',
        },
        {
          icon: 'mdi-puzzle-outline',
          title: '24/7 Support',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tincidunt porta elit, ac scelerisque eros ullamcorper vitae.',
        },
      ],
    }),
  }
</script>
