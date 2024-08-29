<template lang="">
    <div class="card">
        <!-- <img src="https://4kwallpapers.com/images/wallpapers/windows-11-dark-mode-blue-stock-official-1920x1080-5630.jpg" alt="Avatar" style="width:100%">
            <div class="container">
                <h4><b>John Doe</b></h4> 
                <p>Architect & Engineer</p> 
            </div> -->
            <img :src="image" alt="profile" style="width:100%">
            <div class="container">
                <h2><b>{{ name }}</b></h2> 
                <p>{{ tel }}</p> 
            </div>    
    </div>
</template>

<script>
export default {
  // props: ['id', 'name', 'nickname', 'tel', 'email', 'image']
  props: ['id', 'name', 'tel', 'image']

}
</script>

<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  /* width: 40%; */
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
}
</style>