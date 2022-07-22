<script setup lang="ts">
import TheHeader from "@/components/TheHeader.vue";
import EntryEditor from "./components/EntryEditor.vue";
import EntryCard from "@/components/EntryCard.vue";
// Importando reactive
import { reactive } from "vue";
// Imporntado interface User
import type User from "./types/User";

const user: User = reactive({
  id: 1,
  username: "rivalcoba",
  settings: [],
});
console.log(user.id);
</script>

<template>
  <main class="container m-auto p-10">
    <TheHeader />
    <EntryEditor />
    <ul>
      <li>
        <EntryCard />
      </li>
    </ul>
  </main>
</template>
