<script setup>
</script>

<template>
    <div class="slidev-layout">
        <div class="spezi-two-cols-header h-full">
            <div class="spezi-header">
                <slot name="header" />
            </div>
            <div class="spezi-left">
                <slot name="left" />
            </div>
            <div class="spezi-right">
                <slot name="right" />
            </div>
        </div>
    </div>
</template>

<style>
.spezi-two-cols-header {
    display: grid;
    grid-template-areas:
        "header header"
        "left right";
    grid-template-rows: auto 1fr;
    grid-template-columns: 1fr 1fr;
}

.spezi-header {
    grid-area: header;
}

.spezi-left {
    grid-area: left;
}

.spezi-right {
    grid-area: right;
}
</style>