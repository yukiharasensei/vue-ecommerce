<template>
  <fwb-card>
    <div class="p-5">
      <fwb-rating :rating="props.rating" />
      <div class="flex items-center justify-start">
        <h5 class="mr-2 text-xl font-bold tracking-tight text-gray-900 dark:text-white">
          {{ props.name }}
        </h5>
        <div>
          <svg width="24" height="24" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <g data-name="Layer 2">
              <path fill="#49adf4"
                d="M21.187 10.007a3.457 3.457 0 0 1-.864-.712 3.378 3.378 0 0 1 .277-1.141c.291-.821.62-1.751.092-2.474s-1.525-.7-2.4-.68a3.422 3.422 0 0 1-1.155-.078 3.369 3.369 0 0 1-.425-1.063c-.248-.845-.531-1.8-1.4-2.086-.838-.27-1.614.324-2.3.846A3.285 3.285 0 0 1 12 3.25a3.285 3.285 0 0 1-1.023-.631C10.293 2.1 9.52 1.5 8.678 1.774c-.867.282-1.15 1.24-1.4 2.085a3.418 3.418 0 0 1-.421 1.061A3.482 3.482 0 0 1 5.7 5c-.878-.024-1.867-.05-2.4.68s-.2 1.653.092 2.473a3.336 3.336 0 0 1 .281 1.141 3.449 3.449 0 0 1-.863.713c-.732.5-1.563 1.069-1.563 1.993s.831 1.491 1.563 1.993a3.449 3.449 0 0 1 .863.712 3.335 3.335 0 0 1-.273 1.142c-.29.82-.618 1.75-.091 2.473s1.521.7 2.4.68a3.426 3.426 0 0 1 1.156.078 3.4 3.4 0 0 1 .424 1.063c.248.845.531 1.8 1.4 2.086a1.424 1.424 0 0 0 .431.068 3.382 3.382 0 0 0 1.868-.914A3.285 3.285 0 0 1 12 20.75a3.285 3.285 0 0 1 1.023.631c.685.523 1.461 1.12 2.3.845.867-.282 1.15-1.24 1.4-2.084a3.388 3.388 0 0 1 .424-1.062A3.425 3.425 0 0 1 18.3 19c.878.021 1.867.05 2.4-.68s.2-1.653-.092-2.474a3.38 3.38 0 0 1-.281-1.139 3.436 3.436 0 0 1 .864-.713c.732-.5 1.563-1.07 1.563-1.994s-.834-1.492-1.567-1.993Z"
                class="color49adf4 svgShape"></path>
              <path fill="#ffffff"
                d="M11 14.75a.745.745 0 0 1-.53-.22l-2-2a.75.75 0 0 1 1.06-1.06l1.54 1.54 3.48-2.61a.75.75 0 0 1 .9 1.2l-4 3a.751.751 0 0 1-.45.15Z"
                class="colorfff svgShape"></path>
            </g>
          </svg>
        </div>
      </div>
      <p class="font-thin text-gray-700 dark:text-gray-400">
        "{{ props.content }}"
      </p>
    </div>
  </fwb-card>
</template>

<script setup>
import { FwbCard, FwbRating } from "flowbite-vue";
import { defineProps } from "vue";

const props = defineProps({
  rating: {
    type: Number,
  },
  name: {
    type: String,
  },
  content: {
    type: String,
  }
});
</script>