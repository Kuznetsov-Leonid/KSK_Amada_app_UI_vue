<template>
    <button class="Armada__ButtonLarge_Out RegularFontFamily">
        <slot></slot>
    </button>
</template>

<script>
    export default{
        name: 'armada-button-large-out'
    }
</script>

<style scoped lang="scss">
    .Armada__ButtonLarge_Out{
        display: flex;
        flex-direction: column;
        align-items: center;

        color: #469597;
        border: solid #469597 1px;
        border-radius: 4px;
        background: none;
        
        padding: 0px 40px;
        
        font-style: normal;
        font-weight: 700;
        font-size: 16px;
        line-height: 52px;
        letter-spacing: 0.5px;

        transition: 0.3s;
        cursor: pointer;
    }
    .Armada__ButtonLarge_Out:hover{
        color: #FFFFFF;
        background: #4BCCCF;
        border: solid #4BCCCF 1px;
    }

    .Armada__ButtonLarge_Out:active{
        color: #FFFFFF;
        background: #5BA199;
        border: solid #5BA199 1px;
    }

    .Armada__ButtonLarge_Out:disabled{
        background: none;
        border: solid #469597 1px;
        opacity: 0.5;
    }
</style>