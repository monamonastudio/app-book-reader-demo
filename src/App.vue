<script setup lang="ts">
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { library } from "@fortawesome/fontawesome-svg-core";
import { faArrowLeft, faArrowUpFromBracket, faEllipsisVertical, faList, faChevronLeft, faChevronRight } from "@fortawesome/free-solid-svg-icons";

library.add(faArrowLeft, faArrowUpFromBracket, faEllipsisVertical, faList, faChevronLeft, faChevronRight);

import IconBrightness from "@/components/Icon/IconBrightness.vue";
import IconFontCase from "./components/Icon/IconFontCase.vue";
</script>

<template>
  <div class="border w-fit">
    <div class="max-w-[400px] top-0 h-screen relative">
      <div class="h-8 bg-black fixed">
      </div>
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
      <div class="overflow-auto pt-16 pb-48 font-serif">
        <RouterView />
      </div>
      <div class="fixed bottom-0 w-full max-w-[400px] bg-white border-t">
        <div class="flex justify-between p-8 items-center">
          <div class="flex flex-col">
            <FontAwesomeIcon class="h-4" icon="fa-solid fa-chevron-left" />
          </div>
          <div class="flex flex-col">
            Prologue
          </div>
          <div class="flex flex-col">
            <FontAwesomeIcon class="h-4" icon="fa-solid fa-chevron-right" />
          </div>
        </div>
        <div class="grid grid-cols-3 p-4 gap-4 items-center justify-center">
          <div class="flex flex-col items-center justify-between h-14">
            <FontAwesomeIcon class="h-6 mx-auto" icon="fa-solid fa-list" />
            Contenu
          </div>
          <div class="flex flex-col items-center justify-between h-14">
            <IconBrightness class="mx-auto h-8" />
            Fonce
          </div>
          <div class="flex flex-col items-center justify-between h-14">
            <IconFontCase class="h-6 mx-auto" />
            Reglages
          </div>
        </div>
      </div>
    </div>
  </div>
</template>./components/Icon/IconFontCase.vue