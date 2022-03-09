<script setup>
import { NTabs, NTabPane } from "naive-ui";
import ROWS from "@/components/rows/index.vue";
import CONTENTS from "@/components/contents/index.vue";
</script>

<template>
  <div class="temp-left">
    <n-tabs type="segment" pane-style="padding-top: 18px;">
      <n-tab-pane name="chap1" tab="ROWS">
        <ROWS></ROWS>
      </n-tab-pane>
      <n-tab-pane name="chap2" tab="CONTENT">
        “威尔！着火了！快来帮忙！”我听到女朋友大喊。现在一个难题在我面前——是恢复一个重要的
        Amazon 服务，还是救公寓的火。<br /><br />
        我的脑海中忽然出现了 Amazon
        著名的领导力准则”客户至上“，有很多的客户还依赖我们的服务，我不能让他们失望！所以着火也不管了，女朋友喊我也无所谓，我开始
        debug 这个线上问题。
      </n-tab-pane>
      <n-tab-pane name="chap3" tab="SETTING">
        但是忽然，公寓的烟味消失，火警也停了。我的女朋友走进了房间，让我震惊的是，她摘下了自己的假发，她是
        Jeff Bezos（Amazon 老板）假扮的！<br /><br />
        “我对你坚持顾客至上的原则感到十分骄傲”，说完，他递给我一张五美金的亚马逊礼品卡，从我家窗户翻了出去，跳上了一辆
        Amazon 会员服务的小货车，一溜烟离开了。<br /><br />虽然现在我已不在
        Amazon
        工作，但我还是非常感激在哪里学的到的经验，这些经验我终身难忘。你们同意么？
      </n-tab-pane>
    </n-tabs>
  </div>
  <div class="temp-right">
    <CONTENTS></CONTENTS>
  </div>
</template>

<style>
.temp-left {
  padding: 10px;
  background-color: var(--vt-c-white-soft);
}

.temp-right {
  padding: 10px;
  background-color: var(--vt-c-white-mute);
}
</style>
