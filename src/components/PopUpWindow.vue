<template>
    <div>
        <div class="window">
            <slot></slot>
        </div>
        <img class="window-arrow" src="https://r-ak.bstatic.com/static/img/uc_top_arrow/8a5c8d0c06b0bd0775c01108dabf8784316cf2db.png" alt="">
    </div>
</template>

<script>
    export default {
        name: "PopUpWindow"
    }
</script>

<style scoped lang="scss">
    .window {
        position: fixed;
        transform: translateY(50%) translateX(-47.5%);
        background: #fff;
        border: 1px solid #5bbaff;
        -webkit-box-shadow: 0 0 8px #5bbaff;
        box-shadow: 0 0 8px #5bbaff;
        border-radius: 3px;

    &-arrow {
         position: fixed;
         transform: translateY(70%);
     }
    }
</style>
