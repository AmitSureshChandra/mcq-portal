<template>
  <v-layout>
    <v-flex class="text-center">
      <VList two-line>
        <VListTile v-for="i in [1, 1, 1, 1, 1, 1, 11, 1, 1]">
          <VListTileContent>
            <question
              question="Hi ?"
              :qno="1"
              :options="['A', 'B', 'C', 'D']"
              ans="A"
            />
          </VListTileContent>
        </VListTile>
      </VList>
    </v-flex>
  </v-layout>
</template>
