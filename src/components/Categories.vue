<template>
  <v-card tile>
    <v-list dense>
      <CategoryItem categoryTitle="CPU">
        <HoverList title="AMD" :rows="rows_CPU_AMD" />
        <HoverList title="Intel" :rows="rows_CPU_Intel" />
      </CategoryItem>
      <CategoryItem categoryTitle="显卡">
        <HoverList title="AMD" :rows="rows_CPU_AMD" />
        <HoverList title="Nvidia" :rows="rows_CPU_Intel" />
      </CategoryItem>
      <v-list-item-group>
        <HoverList categoryTitle="显示器" :rows="rows_CPU_Intel" />
        <HoverList categoryTitle="内存" :rows="rows_CPU_Intel" />
        <HoverList categoryTitle="电源" :rows="rows_CPU_Intel" />
        <HoverList categoryTitle="硬盘" :rows="rows_CPU_Intel" />
        <HoverList categoryTitle="键鼠" :rows="rows_CPU_Intel" />
      </v-list-item-group>
    </v-list>
  </v-card>
</template>

<script>
  import CategoryItem from "./CategoryItem.vue";
  import HoverList from "./HoverList.vue";

  export default {
    name: "Categories",
    components: { CategoryItem, HoverList },
    data: () => ({
      rows_CPU_AMD: {
        row1: [1, 2, 3, 4],
        row2: [5, 6, 7, 8],
        row3: [9, 10, 11, 12],
      },
      rows_CPU_Intel: {
        row1: [1, 2, 3, 4],
        row2: [5, 6, 7, 8],
        row3: [9, 10, 11, 12],
      },
    }),
  };
</script>
