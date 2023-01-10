<template>
    <div class="border">
        <slot name="flower"></slot>
    </div>
</template>

<style scoped>
    div.border {
        border: 1px solid #ccc;
        background-color: red;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>