<script setup lang="ts">


import Des_label2 from './use/des_label2.vue';
import { useRouter } from 'vue-router';

const router = useRouter()

function To_jishu() {
    router.push("/Mob_jishu_recruit")
}
function back() {
    router.push("/Mob_join")
}
</script>

<template>
    <!-- 组件内容 -->
    <Nav_bar2 page_now="4"></Nav_bar2>
    <div style="height: 70px;"></div>
    <div class="mob_label_1">长期招新</div>
    <div class="mob_box">
        <Des_label2 content="开发部"></Des_label2>
        <div class="jishu_content">
            <div class="jishu_00">招新范围：</div>
            <div class="jishu_01">浙工大全体学院、全体年级的学生</div>
            <br />
            <div class="jishu_10">能力要求：</div>
            <div class="jishu_11">1)能够独立开发api或使用前端框架</div>
            <div class="jishu_21">2)能够独立撰写说明文档</div>
            <div class="jishu_31">3)能够使用git进行团队协作交互</div>
        </div>
        <div class="mob_button1" @click="To_jishu">报名</div>
    </div>

    <div class="mob_button1" @click="back">返回</div>
</template>

<style>
/* 样式 */
.jishu_content {
    margin: 10px;
    text-align: left;

    font-size: 10px;
    display: grid;
    grid-template-rows: repeat(4, 30px);
    grid-template-columns: 60px;
    /* grid-gap: 50px 100px; */
}
.jishu_00 {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 1;
    grid-row-end: 2;
}
.jishu_01 {
    grid-column-start: 2;
    grid-column-end: 2;
    grid-row-start: 1;
    grid-row-end: 2;
}
.jishu_10 {
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 3;
    grid-row-end: 4;
}
.jishu_11 {
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 3;
    grid-row-end: 4;
}
.jishu_21 {
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 4;
    grid-row-end: 5;
}
.jishu_31 {
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 5;
    grid-row-end: 6;
}
</style>