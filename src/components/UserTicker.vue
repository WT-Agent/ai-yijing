<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了乾卦“潜龙勿用”低谷期韬光养晦解读"
  },
  {
    "text": "用户 189****9900 获得了泰卦否卦阴阳转化哲学思考"
  },
  {
    "text": "用户 131****4455 完成了谦卦在机关为人处事中的应用"
  },
  {
    "text": "用户 156****7788 生成了《周易》居安思危决策思维导图"
  },
  {
    "text": "用户 173****3311 取得了国学易经名言心性修养感悟"
  }
]);
</script>
