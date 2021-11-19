<template>
  <el-affix :offset="120">
    <div class="theme-select">
      <theme-select></theme-select>
    </div>
  </el-affix>
  <div class="theme">
    <h1>{{ msg }}</h1>
    <div class="theme-container">

      <div class="theme-container__item">
        <h2>el-button</h2>
        <button2></button2>
      </div>

      <div class="theme-container__item">
        <h2>el-icon</h2>
        <icon2></icon2>
      </div>

      <div class="theme-container__item">
        <h2>Link 链接</h2>
        <link2></link2>
      </div>

      <div class="theme-container__item">
        <h2>Scrollbar 滚动条</h2>
        <scrollbar2></scrollbar2>
      </div>

      <div class="theme-container__item">
        <h2>Typography 排版</h2>
        <typo2></typo2>
      </div>

      <div class="theme-container__item">
        <h2>Cascader 级联选择器</h2>
        <cascader2></cascader2>
      </div>

      <div class="theme-container__item">
        <h2>Checkbox 多选框</h2>
        <checkbox2></checkbox2>
      </div>

      <div class="theme-container__item">
        <h2>ColorPicker 颜色选择器</h2>
        <color-picker2></color-picker2>
      </div>

      <div class="theme-container__item">
        <h2>DatePicker 日期选择器</h2>
        <datepicker2></datepicker2>
      </div>

      <div class="theme-container__item">
        <h2>DateTimePicker 日期时间选择器</h2>
        <date-time-picker2></date-time-picker2>
      </div>

      <div class="theme-container__item">
        <h2>Form 表单</h2>
        <form2></form2>
      </div>

      <div class="theme-container__item">
        <h2>Input 输入框</h2>
        <input2></input2>
      </div>

      <div class="theme-container__item">
        <h2>Input Number 数字输入框</h2>
        <input-number2></input-number2>
      </div>

      <div class="theme-container__item">
        <h2>Avatar 头像</h2>
        <avatar2></avatar2>
      </div>

      <div class="theme-container__item">
        <h2>Calendar 日历</h2>
        <calendar2></calendar2>
      </div>

      <div class="theme-container__item">
        <h2>Descriptions 描述列表</h2>
        <description2></description2>
      </div>

      <div class="theme-container__item">
        <h2>Table 表格</h2>
        <table2></table2>
      </div>

      <div class="theme-container__item">
        <h2>Card 卡片</h2>
        <card2></card2>
      </div>

      <div class="theme-container__item">
        <h2>Carousel 走马灯</h2>
        <carousel2></carousel2>
      </div>

      <div class="theme-container__item">
        <h2>Badge 徽章</h2>
        <badge2></badge2>
      </div>

      <div class="theme-container__item">
        <h2>Breadcrumb 面包屑</h2>
        <breadcrumb2></breadcrumb2>
      </div>

      <div class="theme-container__item">
        <h2>Tag 标签</h2>
        <tag2></tag2>
      </div>

      <div class="theme-container__item">
        <h2>Collapse 折叠面板</h2>
        <collapse2></collapse2>
      </div>

      <div class="theme-container__item">
        <h2>Dialog 对话框</h2>
        <dialog2></dialog2>
      </div>

      <div class="theme-container__item">
        <h2>Divider 分割线</h2>
        <divider2></divider2>
      </div>

      <div class="theme-container__item">
        <h2>Drawer 抽屉</h2>
        <drawer2></drawer2>
      </div>

      <div class="theme-container__item">
        <h2>Dropdown 下拉菜单</h2>
        <dropdown2></dropdown2>
      </div>

      <div class="theme-container__item">
        <h2>Empty 空状态</h2>
        <empty2></empty2>
      </div>

      <div class="theme-container__item">
        <h2>Page Header 页头</h2>
        <header2></header2>
      </div>

      <div class="theme-container__item">
        <h2>Image 图片</h2>
        <image2></image2>
      </div>

      <div class="theme-container__item">
        <h2>Message 消息提示</h2>
        <message2></message2>
      </div>

      <div class="theme-container__item">
        <h2>MessageBox 弹框</h2>
        <messagebox2></messagebox2>
      </div>

      <div class="theme-container__item">
        <h2>Notification 通知</h2>
        <notification2></notification2>
      </div>

      <div class="theme-container__item">
        <h2>Pagination 分页</h2>
        <pagination2></pagination2>
      </div>

      <div class="theme-container__item">
        <h2>Popconfirm 气泡确认框</h2>
        <popconfirm2></popconfirm2>
      </div>

      <div class="theme-container__item">
        <h2>Popover 气泡卡片</h2>
        <popover2></popover2>
      </div>

      <div class="theme-container__item">
        <h2>Progress 进度条</h2>
        <progress2></progress2>
      </div>

      <div class="theme-container__item">
        <h2>Radio 单选框</h2>
        <radio2></radio2>
      </div>

      <div class="theme-container__item">
        <h2>Rate 评分</h2>
        <rate2></rate2>
      </div>

      <div class="theme-container__item">
        <h2>Result 结果</h2>
        <result2></result2>
      </div>

      <div class="theme-container__item">
        <h2>Skeleton 骨架屏</h2>
        <skeleton2></skeleton2>
      </div>

      <div class="theme-container__item">
        <h2>Slider 滑块</h2>
        <slider2></slider2>
      </div>

      <div class="theme-container__item">
        <h2>Loading 加载中</h2>
        <loading2></loading2>
      </div>

      <div class="theme-container__item">
        <h2>Steps 步骤条</h2>
        <step2></step2>
      </div>

      <div class="theme-container__item">
        <h2>Switch 开关</h2>
        <switch2></switch2>
      </div>

      <div class="theme-container__item">
        <h2>Tabs 标签页</h2>
        <tab2></tab2>
      </div>

      <div class="theme-container__item">
        <h2>TimeSelect 时间选择</h2>
        <timeselect2></timeselect2>
      </div>

      <div class="theme-container__item">
        <h2>Timeline 时间线</h2>
        <timeline2></timeline2>
      </div>

      <div class="theme-container__item">
        <h2>Tooltip 文字提示</h2>
        <tooltip2></tooltip2>
      </div>

      <div class="theme-container__item">
        <h2>Transfer 穿梭框</h2>
        <transfer2></transfer2>
      </div>

      <div class="theme-container__item">
        <h2>Tree 树形控件</h2>
        <tree2></tree2>
      </div>

      <div class="theme-container__item">
        <h2>Upload 上传</h2>
        <upload2></upload2>
      </div>

    </div>
  </div>
</template>

<script setup lang="ts">
import Button2 from "~/components/element/button2.vue";
import Icon2 from "~/components/element/icon2.vue";
import Link2 from "~/components/element/link2.vue";
import Scrollbar2 from "~/components/element/scrollbar.vue";
import Typo2 from "~/components/element/typo2.vue";
import Cascader2 from "~/components/element/cascader2.vue"
import Checkbox2 from "~/components/element/checkbox2.vue"
import ColorPicker2 from "~/components/element/colorPicker2.vue";
import Datepicker2 from "~/components/element/datepicker2.vue";
import DateTimePicker2 from "~/components/element/dateTimePicker2.vue";
import Form2 from "~/components/element/form2.vue";
import Input2 from "~/components/element/input2.vue";
import InputNumber2 from "~/components/element/inputNumber2.vue";
import Avatar2 from "~/components/element/avatar2.vue";
import Calendar2 from "~/components/element/calendar2.vue";
import Card2 from "~/components/element/card2.vue";
import Carousel2 from "~/components/element/carousel2.vue";
import Badge2 from "~/components/element/badge2.vue";
import Breadcrumb2 from "~/components/element/breadcrumb2.vue";
import Tag2 from "~/components/element/tag2.vue";
import Collapse2 from "~/components/element/collapse2.vue";
import Description2 from "~/components/element/description2.vue";
import Dialog2 from "~/components/element/dialog2.vue";
import Divider2 from "~/components/element/divider2.vue";
import Drawer2 from "~/components/element/drawer2.vue";
import Dropdown2 from "~/components/element/dropdown2.vue";
import Empty2 from "~/components/element/empty2.vue";
import Header2 from "~/components/element/header2.vue";
import Image2 from "~/components/element/image2.vue";
import Message2 from "~/components/element/message2.vue";
import Messagebox2 from "~/components/element/messagebox2.vue";
import Notification2 from "~/components/element/notification2.vue";
import Pagination2 from "~/components/element/pagination2.vue";
import Popconfirm2 from "~/components/element/popconfirm2.vue";
import Popover2 from "~/components/element/popover2.vue";
import Progress2 from "~/components/element/progress2.vue";
import Radio2 from "~/components/element/radio2.vue";
import Rate2 from "~/components/element/rate2.vue";
import Result2 from "~/components/element/result2.vue";
import Skeleton2 from "~/components/element/skeleton2.vue";
import Slider2 from "~/components/element/slider2.vue";
import Loading2 from "~/components/element/loading2.vue";
import Step2 from "~/components/element/step2.vue";
import Switch2 from "~/components/element/switch2.vue";
import Table2 from "~/components/element/table2.vue";
import Tab2 from "~/components/element/tab2.vue";
import Timeselect2 from "~/components/element/timeselect2.vue";
import Timeline2 from "~/components/element/timeline2.vue";
import Tooltip2 from "~/components/element/tooltip2.vue";
import Transfer2 from "~/components/element/transfer2.vue";
import Tree2 from "~/components/element/tree2.vue";
import Upload2 from "~/components/element/upload2.vue";
import ThemeSelect from "~/components/theme-select.vue";

defineProps<{ msg: string }>();

</script>

<style lang="scss">
.theme-container {
  width: 850px;
  margin: auto;
  background-color: var(--el-color-white);

  .theme-container__item {
    padding: 50px 20px 0 20px;

    h2 {
      height: 40px;
      background: var(--el-text-color-placeholder);
    }
  }
}

.theme-select {
  display: flex;
  justify-content: flex-end;
  padding: 20px;
}
</style>
