<template>

<div class=" fixed-top header w-100">
  <!-- navigation -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-success ">
    <li class="navbar-brand logo" style="margin-right: 10rem"><img src="../../assets/nysc-logo.png" alt="nysc logo"></li>
    
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item" active-class="active"> <span class="nav-link text-white" >
        Link1 </span><span class="sr-only">(current)</span></li>
        <li class="nav-item" active-class="active"> <span class="nav-link text-white"> News </span></li>
        
      </ul>
    </div>
  </nav>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>

  .logo h3:hover {
    color: orange;
  }

  nav li {
    margin: 0 16px;
    color: white;
  }

  .logo img{
      max-width: 50px;
      max-height: 50px;
  }

  .nav-item{
    text-decoration: none;
    color: white;
    cursor: pointer;
  }

  .nav-link:hover,
  .nav-link:active {
    color: #efff16!important;
  }
  
</style>