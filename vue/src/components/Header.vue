<template>
    <div style="height: 50px; line-height:50px; border-bottom: 1px solid #cccccc; display: flex">
        <div style="width: 200px; padding-left:30px; font-weight: bold; color: dodgerblue">后台管理</div>
        <div style="flex: 1"></div>
        <div style="width: 100px">
            <el-dropdown>
                <span class="el-dropdown-link">
                  <br>张三
                  <el-icon class="el-icon--right">
                    <arrow-down/>
                  </el-icon>
                </span>
                <template #dropdown>
                    <el-dropdown-menu>
                        <el-dropdown-item>个人中心</el-dropdown-item>
                        <el-dropdown-item @click.native="$router.push('/login')">退出</el-dropdown-item>
                    </el-dropdown-menu>
                </template>
            </el-dropdown>
        </div>
    </div>
</template>

<script>



    export default {
        name: "Header"
    }
</script>


<style scoped>

</style>

