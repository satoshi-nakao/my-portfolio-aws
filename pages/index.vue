<template>
<!--トップページ-->
  <v-row color="primary" justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
    <v-card>
      　<v-card-title class="headline">
          ようこそこのサイトへ！
        </v-card-title>
        <v-card-text>
          <p>
            私のコードを載せてます。<a
              href="https://github.com/satoshi-nakao"
              target="_blank"
              rel="noopener noreferrer"
            >
              My GitHub
            </a>.
          </p>
          <p>
            学習用に作成しました。<a
              href="https://twitter.com/ksQcRkD1DNl98WE"
              target="_blank"
              rel="noopener noreferrer"
              
            >
              twitter
            </a>.
          </p>
          <p>
            街歩き、建築物の写真を載せてます。<a
              href="https://www.instagram.com/uzisubmachineguhand/"
              target="_blank"
              rel="noopener noreferrer"
              title="contribute"
            >
              instagram
            </a>.
          </p>
        
         
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>


export default {
  data(){
    return{
      drawer: false,
      items: [
        {name: 'Profile',to: '/profile'},
        {name: 'Skill',to: '/skill'},
        {name: 'Like',to: '/like'},
        {name: 'Want',to: '/want'}
      ],
      title: "My Page"
    }
  }
}
</script>
