<template>
  
    <router-view />
  
  
</template>

 <script>
 export default {
     name: 'App',
     data() {
        return {
            map: null,
         
        }
    },
        methods: {
            initMap: () => {
    this.map = new google.maps.Map(document.getElementById("map"), {
        center: { lat: -34.397, lng: 150.644 },
        zoom: 8,
    });
}
        }
    
 }
 </script>