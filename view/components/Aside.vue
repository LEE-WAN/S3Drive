<template>
  <el-menu default-active="2" class="el-menu-vertical-demo" style="height:100%">
    <el-menu-item>
      <i class="el-icon-caret-left"></i>
      <span>Collapse</span>
    </el-menu-item>

    <el-submenu index="1">
      <template slot="title">
        <i class="el-icon-folder"></i>
        <span>{{ $store.state.auth.id }}</span>
      </template>
      <el-menu-item-group title="Group One">
        <el-menu-item index="1-1">item one</el-menu-item>
        <el-menu-item index="1-2">item one</el-menu-item>
      </el-menu-item-group>
      <el-menu-item-group title="Group Two">
        <el-menu-item index="1-3">item three</el-menu-item>
      </el-menu-item-group>
      <el-submenu index="1-4">
        <template slot="title">item four</template>
        <el-menu-item index="1-4-1">item one</el-menu-item>
      </el-submenu>
    </el-submenu>
    <el-menu-item index="2">
      <i class="el-icon-menu"></i>
      <span>Application</span>
    </el-menu-item>
  </el-menu>
</template>
