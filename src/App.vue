<template>
  <div class="title">
    <h1>GPT平台</h1>
  </div>
  <v-container class="background-container">
    <v-row>
      <v-col cols="12" md="4">
        <v-card class="mx-auto" max-width="344">
          <v-img src="https://esay.579878700.xyz//i/2023/12/17/y1b88l.png" height="200px" cover></v-img>

          <v-card-title>ChatGPT Next Web</v-card-title>
          <v-card-text>
            跨平台 ChatGPT 应用，支持多模型。
          </v-card-text>
          <v-card-actions>
            <v-btn color="primary" @click="goToBlog">进入</v-btn>
            <v-spacer></v-spacer>
            <v-btn :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show = !show"></v-btn>
          </v-card-actions>
        </v-card>
      </v-col>

      <v-col cols="12" md="4">
        <v-card class="mx-auto" max-width="344">
          <v-img src="https://esay.579878700.xyz//i/2023/12/17/xzl1xj.png" height="200px" cover></v-img>

          <v-card-title>Pandora-Next(官方账号登录网页版)</v-card-title>
          <v-card-text> 更强大，但还是那个让你呼吸顺畅的ChatGPT。支持GPTs，最新UI。 </v-card-text>
          <v-card-actions>
            <v-btn color="primary" @click="goToGitHub">进入</v-btn>
            <v-spacer></v-spacer>
            <v-btn :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show = !show"></v-btn>
          </v-card-actions>
        </v-card>
      </v-col>

      <v-col cols="12" md="4">
        <v-card class="mx-auto" max-width="344">
          <v-img src="https://esay.579878700.xyz//i/2023/12/17/xwv4uj.png" height="200px" cover></v-img>

          <v-card-title>Lobe Chat</v-card-title>
          <v-card-text> 更多功能的GPT，支持语音合成、多模态和可扩展的函数调用插件系统。 </v-card-text>
          <v-card-actions>
            <v-btn color="primary" @click="goToResume">进入</v-btn>
            <v-spacer></v-spacer>
            <v-btn :icon="show3 ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show3 = !show3"></v-btn>
          </v-card-actions>
        </v-card>
        <v-expand-transition>
          <v-card v-show="show3" class="mx-auto" max-width="344">
            <v-divider></v-divider>
            <v-card-text>
              🤖 Lobe Chat - 一个开源、高性能的聊天机器人框架，支持语音合成、多模态和可扩展的函数调用插件系统。支持一键免费部署您的私人 ChatGPT/LLM Web 应用程序。
            </v-card-text>
          </v-card>
        </v-expand-transition>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      // Make sure to define the "show" property in the data section
      show3: false,
    };
  },
  methods: {
    goToBlog() {
      window.location.href = 'https://gptnext.wakaplus.com';
    },
    goToGitHub() {
      // 跳转到 GitHub 页面
      window.location.href = 'https://pandora-next.wakaplus.com';
    },
    goToResume() {
      // 跳转到简历页面
      window.location.href = 'https://lobe.wakaplus.com';
    },
  },
};
</script>

<style>
.title {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  margin-top: 50px;
}

body {
  background: url('https://w.wallhaven.cc/full/7p/wallhaven-7pmgey.jpg') no-repeat center center fixed;
  background-size: cover;
}

/* Add a white background to the expanded content */
.v-expand-transition-enter-active,
.v-expand-transition-leave-active {
  transition: opacity 0.5s;
}

.v-expand-transition-enter, .v-expand-transition-leave-to /* .v-expand-transition-leave-active in <2.1.8 */ {
  opacity: 0;
  background-color: white;
}
</style>
