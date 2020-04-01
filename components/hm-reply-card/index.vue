<template>
  <div class="hm-reply-card">
    <div class="box">
      <div class="hd">
        <text class="newComments">{{ options.newComments }}</text>
        <div class="block">
          <image class="dot" :src="options.dot" />
          <image class="dot_2" :src="options.dot_2" />
          <image class="dot_3" :src="options.dot_3" />
        </div>
      </div>
      <div class="bd">
        <div class="shopCreditWrap">
          <image class="shopCreditLv1" :src="options.shopCreditLv1" />
          <text class="desc">{{ options.desc }}</text>
        </div>
        <text class="twoDaysAgo">{{ options.twoDaysAgo }}</text>
      </div>
      <div class="row">
        <div class="creditWrap">
          <image class="creditLv1" :src="options.creditLv1" />
          <text class="desc_2">{{ options.desc_2 }}</text>
        </div>
        <div class="outer">
          <text class="num">{{ options.num }}</text>
          <text class="daysAgo">{{ options.daysAgo }}</text>
        </div>
      </div>
      <div class="submain">
        <div class="lanzuanWrap">
          <image class="lanzuanLv1" :src="options.lanzuanLv1" />
          <text class="desc_3">{{ options.desc_3 }}</text>
        </div>
        <div class="block_2">
          <text class="num_2">{{ options.num_2 }}</text>
          <text class="daysAgo_2">{{ options.daysAgo_2 }}</text>
        </div>
      </div>
      <div class="main">
        <div class="huangzuanWrap">
          <image class="huangzuanLv1" :src="options.huangzuanLv1" />
          <text class="desc_4">{{ options.desc_4 }}</text>
        </div>
        <div class="container">
          <text class="num_3">{{ options.num_3 }}</text>
          <text class="daysAgo_3">{{ options.daysAgo_3 }}</text>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmReplyCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-reply-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          newComments: '新评论',
          dot:
            './images/img_26225_0_4.png',
          dot_2:
            './images/img_26225_0_5.png',
          dot_3:
            './images/img_26225_0_6.png',
          shopCreditLv1:
            './images/img_26225_0_3.png',
          desc: '张三已经回答了你对他的设计的评论',
          twoDaysAgo: '两天前',
          creditLv1:
            './images/img_26225_0_2.png',
          desc_2: '李四回答了你对她的项目的评论…',
          num: '3',
          daysAgo: '天前',
          lanzuanLv1:
            './images/img_26225_0_1.png',
          desc_3: '王五已经回答了你对他的计划的评论',
          num_2: '4',
          daysAgo_2: '天前',
          huangzuanLv1:
            './images/img_26225_0_0.png',
          desc_4: '赵六已经回答了你对她的设计的评论',
          num_3: '5',
          daysAgo_3: '天前'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
