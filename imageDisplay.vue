<template>
    <div>
    <!-- we are assuming we are having a css class call modalCard that will display the card -->
    <div v-for="(image, index) in images" :key="index" 
        class="modalCard">
        <img :src="image" width="50" height="50" 
            @click="displayImage(index)">
    </div>
</div>
</template>

<script>
    
    export default {
        data() {
            return {
                // the modal display is initially set to false which will be bind to div element
                modalDispaly: false,
                
                // images array
                images: [
                    {
                        image1,
                        image2,
                        image3,
                        image4
                    }
                ]
            }
        },

        methods: {
            displayImage(index) 
            {
                this.modalDispaly(index) = true;
            }
        }
    }
    
</script>

<style>

</style>
