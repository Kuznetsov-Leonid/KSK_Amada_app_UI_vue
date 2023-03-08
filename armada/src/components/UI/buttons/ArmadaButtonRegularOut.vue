<template>
    <button class="Armada__ButtonRegular_Out RegularFontFamily">
        <slot></slot>
    </button>
</template>

<script>
    export default{
        name: 'armada-button-regular-out'
    }
</script>

<style scoped lang="scss">
    .Armada__ButtonRegular_Out{
        display: flex;
        flex-direction: column;
        align-items: center;

        color: #469597;
        border: solid #469597 1px;
        border-radius: 4px;
        background: none;
        
        padding: 0px 30px;
        
        font-style: normal;
        font-weight: 700;
        font-size: 14px;
        line-height: 44px;
        letter-spacing: 0.5px;

        transition: 0.3s;
        cursor: pointer;
    }
    .Armada__ButtonRegular_Out:hover{
        color: #FFFFFF;
        background: #4BCCCF;
        border: solid #4BCCCF 1px;
    }

    .Armada__ButtonRegular_Out:active{
        color: #FFFFFF;
        background: #5BA199;
        border: solid #5BA199 1px;
    }

    .Armada__ButtonRegular_Out:disabled{
        background: none;
        border: solid #469597 1px;
        opacity: 0.5;
    }
</style>