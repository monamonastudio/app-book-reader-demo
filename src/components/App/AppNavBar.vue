<script lang="ts" setup>
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { library } from "@fortawesome/fontawesome-svg-core";
import { faArrowLeft, faArrowUpFromBracket, faEllipsisVertical } from "@fortawesome/free-solid-svg-icons";

library.add(faArrowLeft, faArrowUpFromBracket, faEllipsisVertical);
</script>
<template>
  <div class="h-16 border-b flex items-center p-4 justify-between fixed max-w-[400px] w-full bg-white">
    <div>
      <FontAwesomeIcon class="h-6" icon="fa-solid fa-arrow-left" />
    </div>
    <div class="flex items-center gap-4">
      <FontAwesomeIcon class="h-6" icon="fa-solid fa-arrow-up-from-bracket" />
      <span class="text-red-600 text-sm">Telecharger</span>
      <FontAwesomeIcon class="h-6" icon="fa-solid fa-ellipsis-vertical" />
    </div>
  </div>
</template>