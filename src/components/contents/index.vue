// 页面内容区域
<script setup>
import { ref, reactive } from "vue";

import draggable from "vuedraggable";

let drag = ref(true);
let pageArray = reactive([
  {
    columns: [
      {
        "grid-columns": 12,
        modules: [],
        style: {
          "background-color": "transparent",
          "border-bottom": "0px solid transparent",
          "border-left": "0px solid transparent",
          "border-right": "0px solid transparent",
          "border-top": "0px solid transparent",
          "padding-bottom": "5px",
          "padding-left": "0px",
          "padding-right": "0px",
          "padding-top": "5px",
        },
      },
    ],
    container: {
      style: {
        "background-color": "rgba(0, 0, 0, 10%)",
        "background-image": "none",
        "background-position": "top left",
        "background-repeat": "no-repeat",
        "text-align": "center",
      },
    },
    content: {
      style: {
        "background-color": "transparent",
        "background-image": "none",
        "background-position": "top left",
        "background-repeat": "no-repeat",
        color: "#000000",
        width: "500px",
      },
    },
    uuid: "26018671-564f-41fd-a5f0-2e22db0b7d37",
  },
  {
    columns: [
      {
        "grid-columns": 3,
        modules: [],
        style: {
          "background-color": "transparent",
          "border-bottom": "0px solid transparent",
          "border-left": "0px solid transparent",
          "border-right": "0px solid transparent",
          "border-top": "0px solid transparent",
          "padding-bottom": "5px",
          "padding-left": "0px",
          "padding-right": "0px",
          "padding-top": "5px",
        },
      },
      {
        "grid-columns": 3,
        modules: [],
        style: {
          "background-color": "transparent",
          "border-bottom": "0px solid transparent",
          "border-left": "0px solid transparent",
          "border-right": "0px solid transparent",
          "border-top": "0px solid transparent",
          "padding-bottom": "5px",
          "padding-left": "0px",
          "padding-right": "0px",
          "padding-top": "5px",
        },
      },
    ],
    container: {
      style: {
        "background-color": "transparent",
        "background-image": "none",
        "background-position": "top left",
        "background-repeat": "no-repeat",
        "text-align": "center",
      },
    },
    content: {
      style: {
        "background-color": "transparent",
        "background-image": "none",
        "background-position": "top left",
        "background-repeat": "no-repeat",
        color: "#000000",
        width: "500px",
      },
    },
    uuid: "769db1f8-e443-4d23-a71c-bdc8118e13b7",
  },
]);

const log = () => {
  console.log(drag.value);
};
</script>

<template>
  <draggable group="rows" v-model="pageArray" item-key="id" @start="log">
    <template #item="{ element }">
      <div :style="element.container.style" class="container-486a">
        <div>
          <div>
            <div
              style="display: flex; margin: auto"
              :style="element.content.style"
            >
              <div style="padding: 5px 0; height: 100%; width: 100%">
                <div
                  class="StageModuleEmpty_sidebarModule__35e6N"
                  data-label="No content here. Drag new from 'Content' panel."
                ></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </template>
  </draggable>
</template>

<style>
.container-486a {
  outline: none;
  position: relative;
  padding-left: 15px;
  padding-right: 15px;
  -webkit-tap-highlight-color: rgb(0, 0, 0 / 0%);
}
.StageModuleEmpty_sidebarModule__35e6N {
  text-align: center;
  outline-offset: -1px;
  min-height: 50px;
  word-break: break-word;
  background: rgba(222, 242, 250, 0.85);
  outline: rgb(47, 170, 222) dashed 1px;
}

.StageModuleEmpty_sidebarModule__35e6N::before {
  content: attr(data-label);
  font-size: 13px;
  color: rgb(47, 170, 222);
  display: block;
  line-height: 20px;
  padding: 20px;
}
</style>
