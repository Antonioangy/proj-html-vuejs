<template>
  <footer>
        <div class="container">
            <div class="row">
                <div class="col-6 mt-3">
                    <p class="text-white main-info">
                        Address
                    </p>
                    <div class="info text-muted">
                        <ul class="list-unstyled">
                            <li >
                                382 NE 191st # 87394 Miami, FL 33179-3899
                            </li>
                            <li>
                                +1(305) 547-9909(9am-5pm EST,Monday-Friday)
                            </li>
                            <li>
                                support@maxcoach.com
                            </li>
                        </ul>
                        <div>
                            <a href=""><i class="fab fa-twitter text-muted"></i></a>
                            <a href=""><i class="fab fa-facebook-f text-muted"></i> </a>
                            <a href=""><i class="fab fa-instagram text-muted"></i></a>
                            <a href=""><i class="fab fa-linkedin text-muted"></i> </a>
                        </div>
                    </div>
                </div>
                <div class="col-5 mt-3 d-flex" >
                    <div class="col-4">
                        <p class="text-white main-info ">
                            Explore
                        </p>
                        <ul class="list-unstyled info text-muted">
                            <li>
                                Start Here
                            </li>
                            <li>
                                Blog
                            </li>
                            <li>
                                About us
                            </li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <p class="text-white main-info ">
                            <br>
                        </p>
                        <ul class="list-unstyled info text-muted">
                            <li>
                                Success story
                            </li>
                            <li>
                                Courses
                            </li>
                            <li>
                                Contact us
                            </li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <p class="text-white main-info ">
                            Information
                        </p>
                        <ul class="list-unstyled info text-muted">
                            <li>
                                Membership
                            </li>
                            <li>
                                Purchase Guide
                            </li>
                            <li>
                                Privacy policy
                            </li>
                            <li>
                                Terms of service
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12 text-muted text-center mt-3">
                    ©2020 Maxcoach. All Rights Reserved
                </div>
            </div>
        </div>
        <div class="col-12">
            <div class="btn"><a href="#"><i class="fas fa-arrow-up text-white"></i></a></div>
        </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer{
        background-color: #171621;
        height: 300px;
        font-size: 15px;
        .btn{
            float: right;
            align-items: flex-end;
            margin-right: 0px;
            font-family: Arial, Helvetica, sans-serif;
            font-size: 12px;
            height:50px;
            width: 50px;
            border-radius: 50%;
            margin-right: 30px;
            margin-top: -30px;
        }
    }
    .info{
        display: block;
    }
    .main-info{
        font-size: 25px;
        margin-top: 20px;
    }
    i{
        margin-right: 40px;
        font-size: 25px;
    }
    li{
        margin-top: 10px;
    }
</style>
