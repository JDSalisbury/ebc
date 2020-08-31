<template>
  <base-section id="about-our-product">
    <base-section-heading
      color="grey lighten-2"
      icon="mdi-lightbulb-on-outline"
      title="Services"
    />

    <v-container>
      <v-row>
        <v-col
          v-for="card in cards"
          :key="card.title"
          cols="12"
          md="4"
        >
          <base-info-card v-bind="card" />
        </v-col>
      </v-row>
    </v-container>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionAboutOurProduct',

    data: () => ({
      cards: [
        {
          title: 'Customize',
          subtitle: 'Best Productivity',
          text: 'Customize a crypto-asset mining operation based on your behind the meter costs and available space to maximize profitability.',
          callout: '01',
        },
        {
          title: 'Installation',
          subtitle: 'Special Offers',
          text: 'Our team of experts will manage the end to end process of procurement, installation, and ongoing maintenance of mining equipment and technology so that you don’t have to.',
          callout: '02',
        },
        {
          title: 'Liquidate',
          subtitle: 'Income Flow',
          text: 'Develop a plan of action to ensure we liquidate newly mined Bitcoins at the most optimally profitable times, but also according to your cashflow needs.',
          callout: '03',
        },
      ],
    }),
  }
</script>
