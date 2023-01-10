<template>
    <div class="border">
        <slot name="title"></slot>
    </div>
</template>

<style scoped>
    div.border {
        border: 1px solid #ccc;
        background-color: lightgreen;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>