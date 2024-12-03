<script lang="ts" setup>
const { userName, userPhone } = toRefs(useUserStore())
</script>

<template>
  <div h-full w-full flex p-5 class="bg-#ffffff">
    <div class="basis-1/3 bg-#ff4757" h-full flex flex-col items-center p-3>
      <div flex items-center>
        <el-avatar :size="60" src="https://www.file.local-server.website/image/1729827948873.jpg" />
        <div>
          <span>{{ userName }}</span>
          <span>{{ userPhone }}</span>
        </div>
      </div>
    </div>
    <div class="bg-#747d8c" h-full flex-1 rounded-2xl />
  </div>
</template>
