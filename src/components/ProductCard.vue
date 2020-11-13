<template>
  <v-card
    :loading="loading"
    class="mx-auto my-4"
    max-width="1100"
  >
  <v-container>
    <v-row dense> 
      <v-col 
      v-for="(product, i) in products"
      :key="i"
      :cols="product.flex"
      >
      <v-img
        height="235"
        :src="product.src"
      ></v-img>

    <v-card-title :title="product.name">{{ product.name }}</v-card-title>

    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="4.5"
          color="amber"
          dense
          half-increments
          readonly
          size="14"
        ></v-rating>

        <div class="grey--text ml-4">
          4.5 (413)
        </div>
      </v-row>

      <div class="my-4 subtitle-1">
        $ • Maceió, Alagoas
      </div>

      <div>{{ product.description }}</div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>

    <v-card-actions>
      <v-btn color="#67afb9" text> Eu quero! </v-btn>
    </v-card-actions>
      </v-col>
    </v-row>
  </v-container>
 
  </v-card>
</template>

<script>
  export default {
    name: 'ProductCard',
    data: () => ({
      products: [
        {
          name: 'Ninho Cremoso',
          description: 'Delicioso Brownie de Ninho Cremoso com pedaços de morango. Vale a pena experimentar essa delícia!',
          src: require('../assets/brownie1.jpeg'),
          flex: 4
        },
        {
          name: 'KitKat',
          description: 'O famoso Brownie de chocolate só que ainda melhor! Vem com pedaçoes de KitKat e é de dar água na boca.',
          src: require('../assets/brownie2.jpeg'),
          flex: 4
        },
        {
          name: 'Tradicional com Sorvete',
          description: 'Brownie tradicional acompanha bola de sorvete e calda de sua preferência. Vem se refrescar com a gente!',
          src: require('../assets/brownie3.jpeg'),
          flex: 4
        },
        {
          name: 'Doce de leite',
          description: 'Nessa versão do brownie, a cobertura é doce de leite argentino. Não preciso dizer mais nada né?',
          src: require('../assets/brownie4.jpeg'),
          flex: 3
        },
        {
          name: 'Morango',
          description: 'Brownie com cobertura e pedaços de morango porque, afinal de contas, morango nunca é demais.',
          src: require('../assets/brownie5.jpeg'),
          flex: 3
        },
        {
          name: 'Ovomaltine',
          description: 'A crocância do ovomaltine com a maciez dos nossos brownies = não tinha como dar errado!',
          src: require('../assets/brownie6.jpeg'),
          flex: 3
        },
        {
          name: 'Chocolate com Morango',
          description: 'Apenas uma palavra define nosso brownie de chocolate com morango: UAU! A harmonia é de outro mundo!',
          src: require('../assets/brownie7.jpeg'),
          flex: 3
        },
      ],
    }),
  }
</script>
