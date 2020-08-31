<template>
  <base-section id="theme-features">
    <base-section-heading title="Two Problems, One Solution">
      Two key variables that impact the profitability of mining Bitcoin are the price of the cryptocurrency and the price of energy.
    </base-section-heading>

    <v-container>
      <v-row>
        <v-col
          v-for="(feature, i) in features"
          :key="i"
          cols="12"
          md="6"
        >
          <base-avatar-card
            v-bind="feature"
            align="left"
            horizontal
          >
            {{ feature.text }}
          </base-avatar-card>
        </v-col>
      </v-row>
    </v-container>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionThemeFeatures',

    data: () => ({
      features: [
        {
          color: 'warning',
          dark: true,
          title: 'Fixed Price',
          icon: 'mdi-fountain-pen-tip',
          text: 'Two key variables that impact the profitability of mining Bitcoin are the price of the cryptocurrency and the price of energy.  Although the price of Bitcoin is a fixed, energy costs are controllable behind the meter for energy producers.',
        },
        {
          color: 'success',
          dark: true,
          title: 'Excess Supply',
          icon: 'mdi-cellphone',
          text: 'In normal times, much uncertainty exists in the energy production industry, and the COVID-19 pandemic has exacerbated this issue.  More and more U.S. energy producers are filing for bankruptcy or are sitting on excess supply, with a reasonable expectation of demand becoming increasingly uncertain.',

        },
        {
          color: 'warning',
          dark: true,
          title: 'Profit',
          icon: 'mdi-pencil-box-outline',
          text: 'At current commercial rates, blockchain mining is not as profitable and is much more reliant on the price of Bitcoin.',

        },
        {
          color: 'success',
          dark: true,
          title: 'Crypto-asset Mining',
          icon: 'mdi-image-size-select-actual',
          text: 'Crypto-asset mining is the future of the mining industry.  Instead of solely mining  for oil and other natural resources, energy output can easily serve as a key driver to this new era of technological innovation.',

        },
        {
          color: 'warning',
          dark: true,
          title: 'Volatility',
          icon: 'mdi-ice-pop',
          text: 'When controlling for energy costs, the volatility in cryptocurrency prices becomes far less of an issue.  Additionally, this creates a unique strategic competitive advantage for energy producers who want to break into the crypto-asset mining space. ',

        },
        {
          color: 'success',
          dark: true,
          title: 'Leveraging output',
          icon: 'mdi-help-circle-outline',
          text: 'Leveraging output that is currently not being demanded toward mining with Elemental Blockchain provides a hedge against increasing uncertainty, and allows the energy industry to thrive and grow with profit margins much higher than what are currently being realized. ',
        },
      ],
    }),
  }
</script>
