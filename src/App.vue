<template>
    <div id="app">
        <el-container class="app-out-pannel">
            <el-header class="sys-header">一张图系统</el-header>
            <el-container class="app-contebt-pannel">
                <el-aside width="200px" class="sys-menu">左侧标题</el-aside>
                <el-main class="sys-content">
                    <mapview />
                </el-main>
            </el-container>
        </el-container>
    </div>
</template>

<script>
import mapview from './components/common/mapview.vue';

export default {
    name: 'App',
    components: { mapview },
};
</script>

<style>
html,
body,
#app {
    position: relative;
    width: 100%;
    height: 100%;
    margin: 0%;
}
.app-out-pannel,
.app-contebt-pannel {
    height: 100%;
}
.sys-header {
    background-color: #409eff;
    line-height: 60px;
    color: aliceblue;
    font-size: 20px;
}
.sys-menu {
    background-color: beige;
}
.sys-content {
    padding: 5px !important;
}
</style>
