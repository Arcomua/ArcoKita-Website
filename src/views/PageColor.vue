<template>
  <v-container>
    <div class="page-container">
      <div class="page-section-color">
        <h1 class="text-primary float-in-right">颜色代码帮助</h1>
        <p class="subheading my-4 float-in-right">在 Minecraft <b>服务器</b>中，通常可以使用以下颜色代码</p>
      </div>
      <div class="page-section-color">
        <h2 class="text-primary float-in-right">通用颜色代码</h2>
        <br>
        <v-row class="mb-4 float-in-left">
          <ColorBlock colorBg="#be0000" colorText="white" colorValue="&4">&4</ColorBlock>
          <ColorBlock colorBg="#fe3f3f" colorText="white" colorValue="&c">&c</ColorBlock>
          <ColorBlock colorBg="#D9A334" colorText="white" colorValue="&6">&6</ColorBlock>
          <ColorBlock colorBg="#fefe3f" colorText="black" colorValue="&e">&e</ColorBlock>
          <ColorBlock colorBg="#00be00" colorText="white" colorValue="&2">&2</ColorBlock>
          <ColorBlock colorBg="#3ffe3f" colorText="black" colorValue="&a">&a</ColorBlock>
          <ColorBlock colorBg="#00bebe" colorText="white" colorValue="&3">&3</ColorBlock>
          <ColorBlock colorBg="#3ffefe" colorText="black" colorValue="&b">&b</ColorBlock>
          <ColorBlock colorBg="#0000be" colorText="white" colorValue="&1">&1</ColorBlock>
          <ColorBlock colorBg="#3f3ffe" colorText="white" colorValue="&9">&9</ColorBlock>
          <ColorBlock colorBg="#be00be" colorText="white" colorValue="&5">&5</ColorBlock>
          <ColorBlock colorBg="#fe3ffe" colorText="white" colorValue="&d">&d</ColorBlock>
          <ColorBlock colorBg="#bebebe" colorText="black" colorValue="&7">&7</ColorBlock>
          <ColorBlock colorBg="#ffffff" colorText="black" colorValue="&f">&f</ColorBlock>
          <ColorBlock colorBg="#3f3f3f" colorText="white" colorValue="&8">&8</ColorBlock>
          <ColorBlock colorBg="#000000" colorText="white" colorValue="&0">&0</ColorBlock>
        </v-row>
      </div>
      <div class="page-section-color">
        <h2 class="text-primary float-in-right">通用字体格式代码</h2>
        <br>
        <v-row class="mb-4 float-in-left">
          <ColorBlock colorValue="&l">&l - <b>粗体</b></ColorBlock>
          <ColorBlock colorValue="&o">&o - <i>斜体</i></ColorBlock>
          <ColorBlock colorValue="&n">&n - <u>下划线</u></ColorBlock>
          <ColorBlock colorValue="&m">&m - <s>删除线</s></ColorBlock>
          <ColorBlock colorValue="&k">&k - 会乱跳的魔术字</ColorBlock>
          <ColorBlock colorValue="&r">&r - 清除颜色与格式</ColorBlock>
        </v-row>
      </div>
    </div>
  </v-container>
</template>

<script setup>
import ColorBlock from "@/components/ColorBlock.vue"
</script>


<style lang="scss" scoped>
h1,
h2,
p,
th {
  user-select: text;
}

.page-section-color {
  display: flex;
  flex-direction: column;
}
</style>
