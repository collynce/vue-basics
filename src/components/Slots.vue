<template>
    <div class="slots">
        <slot></slot>
        <div>
            <p>
                <slot name="paragraph"></slot>
            </p>
            <h3>
                <slot name="header"></slot>
            </h3>
            <span>
                <slot name="span"></slot>
            </span>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Slots"
    }
</script>

<style scoped>
.slots{
    background: aquamarine;
    padding: 8px;
    margin: 20px 0 0 0;
}
</style>


