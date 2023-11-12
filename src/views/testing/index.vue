
<script lang="ts" setup>
import draggable from "vuedraggable";
import { ref } from "vue";

const list1 = ref([
    { name: "John", id: 1 },
    { name: "Joao", id: 2 },
    { name: "Jean", id: 3 },
    { name: "Gerard", id: 4 }
])

const list2 = ref([
    { name: "John", id: 1 },
    { name: "Joao", id: 2 },
    { name: "Jean", id: 3 },
    { name: "Gerard", id: 4 }
])

// function add() {
//     list.value.push({ name: "Juan" });
// }
// function replace() {
//     this.list = [{ name: "Edgard" }];
// }
// function clone(el) {
//     return {
//         name: el.name + " cloned"
//     };
// }
function log(evt: any) {
    window.console.log(evt);
}
</script>

<template>
    <!-- <h1>hello</h1> -->
    <div class="grid grid-cols-2 gap-4">
        <div class="">
            <h3>Draggable 1</h3>
            <draggable class="list-group" :list="list1" group="people" @change="log" itemKey="name">
                <template #item="{ element, index }">
                    <div class="list-group-item">{{ element.name }} {{ index }}</div>
                </template>
            </draggable>
        </div>

        <div class="">
            <h3>Draggable 2</h3>
            <draggable class="list-group" :list="list2" group="people" @change="log" itemKey="name">
                <template #item="{ element, index }">
                    <div class="list-group-item">{{ element.name }} {{ index }}</div>
                </template>
            </draggable>
        </div>
    </div>
</template>

<style scoped></style>