---
layout: page
sidebar: false
title: "page"

head:
  - - meta
    - name: "description"
      content: "page"
  - - meta
    - name: "keywords"
      content: "page"
---

<script setup>
import { ref } from "vue";
import { VPTeamMembers } from 'vitepress/theme';

const team = ref([
  {
    avatar: "https://avatars.githubusercontent.com/u/11247099?v=4",
    name: "Mike",
    title: "Developer",
    links: [
      { icon: "github", link: "https://github.com/mike-koch" },
    ]

  }
]);
const title = ref("1")
</script>

<div>{{title}}</div>
<button @click="title++">++++</button>

<VPTeamMembers size="small" :members="team"></VPTeamMembers>