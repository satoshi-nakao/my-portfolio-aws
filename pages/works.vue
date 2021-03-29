<template>
  <v-layout row>
    <v-flex xs12>
      <v-card>
        <v-card-title class="headline">
          作品
        </v-card-title>
        <v-card-text>
          <p>
            学習のアウトプットして作成したものです。
          </p>
          <v-layout row wrap>
            <v-flex v-for="(product, i) in products" :key="i" d-flex md4>
              <v-card>
                <v-img :src="product.image" aspect-ratio="2.75"></v-img>
                <v-card-title class="headline">
                  {{ product.name }}
                </v-card-title>
                <v-card-text>
                  {{ product.description }}
                </v-card-text>
                <v-card-actions>
                  <v-btn color="primary" :href="product.url" target="_blank">
                    詳細
                  </v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
          </v-layout>
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {
     products:[
            // {
            //  name: 'My-portfolio-site',
            //  description: '最初に作ったポートフォリオサイト',
            //  image: '/my-portfolio.icon.jpg',
            //  url: 'https://satoshi-portfolio-site.netlify.app/'
            // },
            // {
            //  name: 'My-portfolio-site2',
            //  description: '二つ目に作ったポートフォリオサイト',
            //  image: '/my-portfolio.icon2.jpg',
            //  url: 'https://satoshi-nakao-myportfolio-ver2.netlify.app/'
            // },
            {
             name: 'My-portfolio-pwa',
             description: 'ポートフォリオサイトをPWA化しました。',
             image: 'my-portfolio-site-pwa.jpg',
             url: 'https://satoshi-nakao-protfolio-pwa.netlify.app/'
            },
      ]
    }
  }
}
</script>