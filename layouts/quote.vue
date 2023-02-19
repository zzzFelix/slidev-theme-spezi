<template>
    <div class="slidev-layout quote">
        <div>
            <slot name="header" />

            <div class="quote-inner">
                <div class="marks">“</div>
                <blockquote :cite="cite">
                    {{ quote }}
                </blockquote>

                <cite v-if="cite"><a :href="cite" target="_blank">{{ author }}</a></cite>
                <cite v-if="!cite">{{ author }}</cite>
            </div>

            <slot></slot>
        </div>
    </div>
</template>
  
<script setup lang="ts">
defineProps({
    quote: {
        type: String,
        required: true
    },
    author: {
        type: String,
        required: true
    },
    cite: {
        type: String,
        required: false
    }
})
</script>

<style>
.slidev-layout.quote {
    text-align: left;

    h1 {
        color: var(--prism-foreground);
    }

    .quote-inner {
        display: grid;
        grid-template-areas:
            "marks quote"
            "cite cite";
        grid-template-columns: auto auto;
        grid-template-rows: auto auto;
        margin-top: 3rem;
    }

    .marks {
        @apply text-9xl leading-20;
        color: var(--slidev-theme-primary);
        grid-area: marks;
        margin-top: 0.9rem;
        margin-right: 1rem;
    }

    blockquote {
        @apply text-4xl leading-20;
        line-height: 120%;
        color: var(--slidev-theme-primary);
        background-color: transparent;
        border-left: none;
        padding: 0;
        grid-area: quote;
    }

    cite {
        text-align: right;
        grid-area: cite;
    }

    h1+p {
        text-align: right;
    }
}
</style>
    