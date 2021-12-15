<template>
  <header>
      <div id="color">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-2">
                    <img src="@/assets/dark-logo.png" alt="" id="logo">
                </div>
                <div class="col-8 d-flex" id="nav">
                    <div>Home <i class="fas fa-angle-down"></i></div>
                    <div>Pages <i class="fas fa-angle-down"></i></div>
                    <div>Courses <i class="fas fa-angle-down"></i></div>
                    <div>Features <i class="fas fa-angle-down"></i></div>
                    <div>Blog <i class="fas fa-angle-down"></i></div>
                    <div>Shop <i class="fas fa-angle-down"></i></div>
                </div>
                <div class="col-2 d-flex ">
                    <div>
                        <a href=""><i class="fab fa-twitter px-2 text-dark"></i></a>
                        <a href=""><i class="fab fa-facebook-f px-2 text-dark"></i> </a>
                        <a href=""><i class="fab fa-instagram px-2 text-dark"></i></a>
                        <a href=""><i class="fab fa-linkedin px-2 text-dark"></i> </a>
                    </div>
                </div>
            </div>
        </div>
        <div class="container" id="jumbo">
            <div class="row">
                <div class="col-6">
                    <h5 class="name">I'M WINGMAN</h5>
                    <h1 class="font">Peace On Earth A <br> Wonderful Wish <br> But No Way</h1>
                    <p>success isn't overmight. it's when everyday you get a little <br> better than the day before it all adds up.</p>
                    <a class="btn" href="#" role="button">Get Started for Free <i class="fas fa-arrow-right"></i></a>
                </div>
                <div class="col-6">
                    <img src="@/assets/home-movation-hero-image.png" alt="man" id="man">
                </div>
            </div>
        </div>
      </div>
    <div class="container col-12 d-flex text-center " id="dati">
        <div class="row col-12 d-flex" style="align-items: center">
            <div class="col-3">
                <div class="d-flex justify-content-center statistics" >
                    1.926
                </div>
                FINISHED SESSION
            </div>
            <div class="col-3">
                <div class="d-flex justify-content-center statistics">
                    100%
                </div>
                SATISFACTION RATE
            </div>
            <div class="col-3">
                <div class="d-flex justify-content-center statistics">
                    3092+
                </div>
                ENROLLED LEARNERS
            </div>
            <div class="col-3" >
                <div class="d-flex justify-content-center statistics">
                    200
                </div>
                ONLINE INSTRUCTORS
            </div>
        </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #logo{
        height: 30px;
    }
    #nav{
        justify-content: space-evenly
    }
    #jumbo{
        height: 500px;
        margin-top: 70px;
    }
    #color{
        background-color: #f7f7fd;
    }
    #man{
        height: 500px;
    }
    .name{
        font-size: 15px;
        margin-top: 40px;
    }
    #dati{
        height: 200px;
    }
    .statistics{
        font-size: 40px;
        color: #38b6a1;
    }
</style>
