<template>
    <button class="Armada__ButtonSmall RegularFontFamily">
        <slot></slot>
    </button>
</template>

<script>
    export default{
        name: 'armada-button-small'
    }
</script>

<style scoped lang="scss">
    .Armada__ButtonSmall{
        display: flex;
        flex-direction: column;
        align-items: center;

        color: #FFFFFF;
        border: solid #469597 1px;
        border-radius: 4px;
        background: #469597;
        
        padding: 0px 20px;
        
        font-style: normal;
        font-weight: 700;
        font-size: 12px;
        line-height: 36px;
        letter-spacing: 0.5px;

        transition: 0.3s;
        cursor: pointer;
    }

    .Armada__ButtonSmall:hover{
        background: #4BCCCF;
        border: solid #4BCCCF 1px;
    }

    .Armada__ButtonSmall:active{
        background: #5BA199;
        border: solid #5BA199 1px;
    }

    .Armada__ButtonSmall:disabled{
        background: #469597;
        border: solid #469597 1px;
        opacity: 0.5;
    }
</style>