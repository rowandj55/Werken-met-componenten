<template>
    <br />
</template>

<script setup>
import {ref, computed} from 'vue';
</script>

<!-- <template>
    <br />
    <input v-model="newName" placeholder="Fill in your name" />
    <input v-model.number="newAge" placeholder="Fill in your age" type="number" />
    <button @click="addPerson">Add</button>
    <h3>People</h3>
    <ul>
        <li v-for="(person, index) in people" :key="index">{{ person.name }}: {{ person.age }}</li>
    </ul>
    <h3>Adults</h3>
    <ul>
        <li v-for="(adult, index) in adults" :key="index">{{ adult.name }}: {{ adult.age }}</li>
    </ul>
    <h3>Children</h3>
    <ul>
        <li v-for="(child, index) in children" :key="index">{{ child.name }}: {{ child.age }}</li>
    </ul>
    <br />
    <p>
        <strong>Total people:</strong>
        {{ totalPeople }}
    </p>
    <p>
        <strong>Total adults:</strong>
        {{ numberOfAdults }}
    </p>
    <p>
        <strong>Total children:</strong>
        {{ numberOfChildren }}
    </p>
</template>

<script setup>
import {ref, computed} from 'vue';

const people = ref([
    {name: 'Jan', age: 12},
    {name: 'Piet', age: 20},
]);

const newAge = ref(null);
const newName = ref(null);

const children = computed(() => {
    return people.value.filter(person => person.age < 18);
});

const adults = computed(() => {
    return people.value.filter(person => person.age > 17);
});

const totalPeople = computed(() => {
    return people.value.length;
});

const numberOfChildren = computed(() => {
    return children.value.length;
});

const numberOfAdults = computed(() => {
    return adults.value.length;
});

function addPerson() {
    if (newName.value && newAge.value) {
        people.value.push({
            name: newName.value,
            age: newAge.value,
        });
        newName.value = null;
        newAge.value = null;
    }
}
</script> -->
