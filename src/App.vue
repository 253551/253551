<template>
  <header class="header">
    <section class="main">
      <h1>
        <img src="./assets/images/logo.webp" />
        PayQrcode
      </h1>
      <h2>二合一收款码物理合并版</h2>
    </section>
  </header>
  <main>
    <t-space direction="vertical">
      <t-alert theme="info">
        <template #message>
          开源：
          <t-link
            theme="primary"
            underline
            href="https://github.com/uxiaohan/PayQrcode"
            target="_blank"
          >
            PayQrcode
          </t-link>
          ，技术支持：
          <t-link theme="primary" underline href="https://www.longs.cn" target="_blank">
            心动次元
          </t-link>
        </template>
      </t-alert>
      <t-alert theme="success">
        <template #icon></template>
        <template #message>
          <p>
            ✅ 物理合并，直接将
            图片合并成一张图片，无需服务器，不怕被篡改，可打印使用，稳定，绿色，安全！
          </p>
          <p>⚠️全程离线运行，二维码解析合并无任何更改，且项目开源，请放心食用！</p>
        </template>
      </t-alert>
      <t-alert theme="warning" message="请尽量把非二维码区域裁剪后上传，以提升识别准确性！" />
    </t-space>
    <Main />
  </main>
</template>
<script lang="ts" setup>
import Main from '@/components/Main/Main.vue'
</script>
