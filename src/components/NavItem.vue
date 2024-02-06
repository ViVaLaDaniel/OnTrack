<template>
   <li class="flex-1">
        <a :href="`#{page}`" class="flex flex-col items-center p-2 text-xs capitalize">
          <slot></slot>
        </a>
      </li>
</template>