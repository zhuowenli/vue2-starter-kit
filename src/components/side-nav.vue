<template>
    <el-menu class="side-nav" default-active="/" router="router">
        <el-menu-item index="/"><i class="material-icons">home</i>首页</el-menu-item>
        <el-submenu index="1">
            <template slot="title"><i class="material-icons">menu</i>导航一</template>
            <el-menu-item index="1-1">选项1</el-menu-item>
            <el-menu-item index="1-2">选项2</el-menu-item>
            <el-menu-item index="1-3">选项3</el-menu-item>
        </el-submenu>
        <el-submenu index="2">
            <template slot="title"><i class="material-icons">message</i>导航二</template>
            <el-menu-item index="2-1">选项1</el-menu-item>
            <el-menu-item index="2-2">选项2</el-menu-item>
            <el-menu-item index="2-3">选项3</el-menu-item>
        </el-submenu>
        <el-submenu index="3">
            <template slot="title"><i class="material-icons">settings</i>导航三</template>
            <el-menu-item index="3-1">选项1</el-menu-item>
            <el-menu-item index="3-2">选项2</el-menu-item>
            <el-menu-item index="3-3">选项3</el-menu-item>
        </el-submenu>
    </el-menu>
</template>

<script>
    export default {
        name: 'side-nav',
        data() {
            return {
                router: true
            }
        }
    }
</script>

<style lang="scss">
    @import "../stylesheets/common";

    .side-nav{
        width: 250px;
        @include user-select(none);
    }
</style>