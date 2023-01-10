<template>
    <div>
        <div class="border">
            <slot ></slot>
        </div>
    </div>
    
</template>

<style scoped>
    div.border {
        border: 1px solid #ccc;
        background-color: lightblue;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>