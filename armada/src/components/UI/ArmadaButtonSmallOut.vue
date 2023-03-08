<template>
    <button class="Armada__ButtonSmall_Out RegularFontFamily">
        <slot></slot>
    </button>
</template>

<script>
    export default{
        name: 'armada-button-small-out'
    }
</script>

<style scoped lang="scss">
    .Armada__ButtonSmall_Out{
        display: flex;
        flex-direction: column;
        align-items: center;

        color: #469597;
        border: solid #469597 1px;
        border-radius: 4px;
        background: none;
        
        padding: 0px 20px;
        
        font-style: normal;
        font-weight: 700;
        font-size: 12px;
        line-height: 36px;
        letter-spacing: 0.5px;

        transition: 0.3s;
        cursor: pointer;
    }
    .Armada__ButtonSmall_Out:hover{
        color: #FFFFFF;
        background: #4BCCCF;
        border: solid #4BCCCF 1px;
    }

    .Armada__ButtonSmall_Out:active{
        color: #FFFFFF;
        background: #5BA199;
        border: solid #5BA199 1px;
    }

    .Armada__ButtonSmall_Out:disabled{
        background: none;
        border: solid #469597 1px;
        opacity: 0.5;
    }
</style>