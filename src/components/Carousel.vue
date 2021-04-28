<template>
   <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active change_slide" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" class="change_slide" aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" class="change_slide" aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/img/index_bg.png" class="d-block w-100" alt="...">
        <div class="carousel-caption d-none d-md-block">
          <div class="row d-flex justify-content-center">
            <div class="col-md-12 title">120 Anastasia Avenue, Coral Gables</div>
            <div class="col-md-2 price">$650,000</div>
            <div class="col-md-2 button d-flex align-items-center"><button class="btn btn-primary">MORE INFO</button></div>
          </div>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/img/index_bg.png" class="d-block w-100" alt="...">
        <div class="carousel-caption d-none d-md-block">
          <div class="row d-flex justify-content-center">
            <div class="col-md-12 title">120 Anastasia Avenue, Coral Gables</div>
            <div class="col-md-2 price">$600,000</div>
            <div class="col-md-2 button d-flex align-items-center"><button class="btn btn-primary">MORE INFO</button></div>
          </div>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/img/index_bg.png" class="d-block w-100" alt="...">
        <div class="carousel-caption d-none d-md-block">
          <div class="row d-flex justify-content-center">
            <div class="col-md-12 title">120 Anastasia Avenue, Coral Gables</div>
            <div class="col-md-2 price">$800,000</div>
            <div class="col-md-2 button d-flex align-items-center"><button class="btn btn-primary">MORE INFO</button></div>
          </div>
        </div>
      </div>
  </div>
</div>
</template>


<style lang="scss" scoped>
.carousel-item {
    max-height: calc(100vh - 80px);
    position: relative;
    .row {
      position: absolute;
      top: -700%;
      left: 10%;
      button {
        background-color: rgba(128, 128, 128, 0.5);
        border: none;
      
      }
    }
}
.change_slide {
  border: 1px solid white;
  background: none;
  border-radius: 50%;
  width: 13px;
  height: 13px;
    &.active {
      background-color: white;
    }
}
.title {
  font-family: Raleway;
  font-size: 48px;
  font-weight: 700;
  color: #ffffff;
}
.price {
  font-size: 36px;
  font-weight: 300;
  color: #ffffff;
}
.button {
  font-size: 16px;
  font-weight: 700;
  color: #ffffff;
  margin-left: 20px;
}



  
</style>