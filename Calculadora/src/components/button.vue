<template>
 <button class="button"
        @click="$emit('onClick', label)"
        :class="{ double, triple, operation }">
        {{ label }}
    </button>
</template>

<script>
export default {
  props: {
    label:{},
    operation:{type: Boolean},
    double:{type: Boolean},
    triple:{type: Boolean}
}
}
</script>

<style>
:root {
  --bg-button:white;
  --border-button:solid,1px,grey;
}
.button {
  font-size: 1.4em;
  background-color: var(--bg-button);
  border:solid 0.5px,grey;
  border-right: var(--border-button);
  border-bottom: var(--border-button);
  outline:none;
}
.button:active {
  background-color: aliceblue;
}
.button.double {
  grid-column: span 2;
}
.button.triple {
  grid-column: span 3;
}
.button.operation {
  background-color: rgb(43, 0, 0);
  color:white;
}
.button.operation:active {
  background-color: rgb(10, 2, 2);
}
</style>