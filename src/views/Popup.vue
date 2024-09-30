<template>
    <div class="pop">
        <div class="popup-inner">
            <slot />
            <button class="fechar-popup">
                fechar popup
            </button>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="sccs" scoped>
.popup {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 99;
    background-color: (0, 0, 0, 0.2);
    display: flex; 
    align-items: center;
    justify-content: center;

    .popup-inner{
        
    }
}

</style>