<script setup>
import { CheckCircleIcon } from "@heroicons/vue/24/solid"
import { ClockIcon, ListBulletIcon, ChartBarIcon } from "@heroicons/vue/24/outline"
const navIteams = ["timeline","activities","progress",]
</script>
<template>
  <header class="sticky top-0 z-20 flex items-center justify-between border-b bg-white p-3">
    <a href="#">
      <img src="./assets/logo.png" alt="Logo" class="h-9" />
    </a>
    <a href="#" class="text-sm">
      <div v-if="false" class="flex items-center gap-1">
        Day complete!
        <CheckCircleIcon class="h-7 text-green-500" />
      </div>
      <div v-else class="flex items-center gap-1">
        <div>Progress: <span class="font-mono">20%</span></div>
        <div class="h-3 w-3 rounded-full bg-red-500"></div>
      </div>
    </a>
  </header>
  <main class="flex flex-grow flex-col">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime nemo rerum, vitae et culpa
    exercitationem aliquam neque alias porro, asperiores error! Rerum, ipsam odit. Doloremque
    voluptas, aut beatae hic labore excepturi in nemo quidem vero iusto ab accusamus sint
    consequuntur voluptatem nulla minus nam facere omnis pariatur? Qui, ratione nisi maxime magnam,
    debitis numquam error iusto voluptates nesciunt corporis quidem. Earum ipsa incidunt odio odit
    voluptatum, facilis modi animi illum nemo ab aperiam? Numquam quam eaque reiciendis provident
    quas soluta! Quasi, placeat dolorum ducimus atque vero modi cum commodi maxime, perspiciatis
    natus officia nostrum doloribus. Iste, incidunt repellendus earum quos quas libero quasi ab,
    molestias fuga totam enim? Eum reiciendis maxime impedit ad commodi sint ut error aut vitae,
    pariatur reprehenderit dolor tempore unde delectus qui laborum enim veritatis. Molestiae iure,
    possimus suscipit architecto illo aspernatur maxime deserunt ipsum obcaecati accusamus molestias
    laborum quos, unde soluta ad id est praesentium aperiam, accusantium veniam incidunt. Qui
    veritatis doloribus expedita eos minus ad doloremque officia, ratione distinctio corporis
    suscipit reiciendis magni obcaecati sed incidunt sequi in omnis dolorem corrupti molestias quas
    iusto! Eum assumenda deleniti ipsam tenetur? Doloribus impedit harum facilis magnam odio a eaque
    nam dolor iste explicabo consequatur eos quas molestiae ratione id aspernatur hic minus magni
    atque omnis, voluptates dolore? Necessitatibus sint quisquam ab, ipsam hic unde, rem velit
    mollitia dolor ea sequi non voluptas obcaecati esse quos aliquam labore cupiditate dolores
    maxime deleniti. Minima blanditiis, voluptatibus repellat dolor ad expedita totam impedit
    assumenda ullam libero molestias ipsa dolore, dicta, atque velit voluptas qui. Ut suscipit
    accusantium exercitationem labore. Inventore ducimus vitae in labore autem error ab impedit cum
    tenetur expedita magni fugit repellat officiis sunt eaque quo, earum laudantium beatae, ex
    voluptate veritatis vero cumque voluptatem quasi. Impedit at minima temporibus necessitatibus,
    sint minus. Fugit facilis temporibus enim molestias soluta itaque unde, eum ex omnis
    voluptatibus aspernatur deleniti blanditiis hic tempora possimus cum quia ab beatae maxime
    voluptatum corrupti error. Repudiandae velit veritatis nostrum repellat amet at et labore
    corrupti voluptatem sed fuga nemo illum, nesciunt magni debitis, ipsa vitae natus nobis eveniet
    explicabo quibusdam eligendi magnam. Repellat, fugiat. Molestiae accusantium facilis non soluta
    odit alias aliquam voluptatibus maxime aut id temporibus at, beatae quia dolores? Fugit officiis
    aperiam fuga necessitatibus sed alias modi magni temporibus id recusandae, voluptatibus odio
    exercitationem dolor eius nulla mollitia? Quis inventore praesentium doloribus et accusamus
    eaque veritatis eum nobis distinctio? Veritatis tenetur repudiandae eum ipsam aliquid molestiae
    illum accusamus, aut voluptas alias sequi, ut sapiente aspernatur adipisci optio fuga
    cupiditate? Necessitatibus sequi a veniam possimus? Nulla, rem reiciendis deleniti quam
    molestias, repellat quis error sapiente minima, autem magni ad commodi explicabo tempora
    similique optio quia quas consequatur temporibus nostrum asperiores mollitia. Eligendi
    praesentium impedit doloribus assumenda mollitia, maiores suscipit qui illum provident enim non
    facilis ad quae tenetur atque vel maxime nam. Temporibus, commodi tenetur inventore sed cum
    eveniet! Aut facere accusamus dicta ipsum, neque totam ullam inventore, quidem error natus,
    sequi officiis perspiciatis cumque ducimus quam ut eveniet. Ratione, iure eos?
  </main>
  <nav class="sticky bottom-0 z-10 bg-white text-3xl">
    <ul class="flex items-center justify-around border-t">
      <li v-for="page in navIteams" :key="page" class="flex-1">
        <a :href="`#{page}`" class="flex flex-col items-center p-2 text-xs capitalize">
          <ClockIcon v-if="page === 'timeline' " class="h-6 w-6"/> 
          <ListBulletIcon v-else-if=" page === 'activities'" class="h-6 w-6" /> 
          <ChartBarIcon v-else="" class="h-6 w-6" />  {{ page }}
          </a>
      </li>
    </ul>
  </nav>
</template>
