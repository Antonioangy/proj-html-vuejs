<template>
  <main>
    <div class="container">
        <h5 class="verde section">ABOUT ME</h5>
        <div class="row align-items-center">
            <div class="col-6">
                <p class="font class">How to be an Alpha <br> Male: The 15 Habits of <br> True Alphas</p>
            </div>
            <div class="col-6 d-flex ">
                <p>
                    <strong class="text mb-2"> Want to learn how to be <span class="verde">an alpha male?</span>  how to be more masculine? <br> How to be the man you've always wanted to be? <br></strong>
                    Your goal is to show the consistency of bsiness, core values, and customer care. Punctuality, responsability, individuality, accuracy, enthusiasm -  you have to clearly expalin how these qualities are applicable to your work. And the important Thing is you do love what you do.
                </p>
            </div>
        </div>
    </div>
    <!-- video yt -->
    <div class="container" id="videosection">
        <div class="row">
            <div class="col-7">
                <img src="@/assets/home-movation-video-poster-670x450.jpg">
                <img src="@/assets/icon-youtube-play.png" id="youtube">
            </div>
            <div class="col-5">
                <p class="display-6">
                    "Every morning you have two <br> choices: continue to sleep with <br> your dreams, or wake up and <br>chase them."
                </p>
                <img src="@/assets/home-movation-shape-01.png" class="m-3">
                <h5 >Kaixa Stark</h5>
                <div class="grey">WINGMAN</div>
            </div>
        </div>
    </div>
    <!-- corsi -->
    <div class="container">
        <div class="text-center">
            <div class="section grey">
                BEGIN YOUR JOURNEY AT MAXCOACH
            </div>
            <h1 class="font">Latest <span class="verde">Online Courses</span></h1>
        </div>
        <div class="row">
            <div class="col-4" v-for="(course, i) in courses" :key="i">
                <div class="d-flex justify-content-center course">
                    <img :src="require(`../assets/${course.image}`)"/>
                </div>
                <div class="sx">
                    <div class="verde m-2">
                        <strong>{{course.price}}</strong>
                    </div>
                    <h4 class="title m-2">
                        {{course.text}}
                    </h4>
                </div>
                <div class="d-flex sx">
                    <div class="col-4">
                        <i class="far fa-file m-2"></i> {{course.lessons}}
                    </div>
                    <div class="col-4">
                        <i class="far fa-user m-2"></i> {{course.students}}
                    </div>
                    <div class="col-4">
                    </div>
                </div>
            </div>
        </div>
        <div class="d-flex justify-content-center" id="viewbtn">
            <a class="btn px-3" href="#" role="button">View all Courses <i class="fas fa-arrow-right"></i></a>
        </div>
    </div>
    <!-- libri -->
    <div class="container" id="books">
        <div class="row">
            <div class="col-6">
                <div>
                    Book Store Online
                </div>
                <h2 class="font">
                    Be Alpha With <br>
                    <div class="verde">Wingman's book</div>
                </h2>
                <ul class="list-unstyled">
                    <li><i class="fas fa-check verde"></i> Help you understant yourself better</li>
                    <li><i class="fas fa-check verde"></i> Revealing mature tips</li>
                    <li><i class="fas fa-check verde"></i> Give the right advice</li>
                    <li><i class="fas fa-check verde"></i> Fascinating examples of alpha man</li>
                </ul>
                <a class="btn" href="#" role="button">Get Free Ebook</a>
            </div>
            <div class="col-3 text-center">
                <img src="@/assets/product-book-11-400x400.jpg" alt="" class="bookcover">
                <div class="title">
                    Alpha man by Maxcoach
                </div>
                <div class="title">
                    $29.00
                </div>
            </div>
            <div class="col-3 text-center">
                <img src="@/assets/product-book-10-400x400.jpg" alt="" class="bookcover">
                <div class="bookname">
                    Real man 4.0 by Maxcoach
                </div>
                <div class="bookcost">
                    $39.00
                </div>
            </div>
        </div>
        <!-- sponsor -->
    </div>
    <div class="container" id="sponsors">
        <div class="row" >
            <div class="col-2" v-for="(sponsor, i) in sponsors" :key="i">
                <div class="opacity d-flex justify-content-center">
                    <img :src="require(`../assets/${sponsor.image}`)"/>
                </div>
            </div>
        </div>
    </div>
    <!-- Real stories -->
    <div id="realstories">
        <div class="row text-center">
            <div class="col-6">
                <div class="verde">
                    Real Stories
                </div>
            </div>
            <div class="col-6">
                <div>
                    <img src="@/assets/home-movation-testimonial-image-768x562.jpg" alt="smiling-man">
                </div>
            </div>
        </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Main',
  data () {
    return {
      courses: [
        {
          price: '$30.00',
          text: 'How to be Successful:Create A Growth Mindset For Success',
          image: 'motivation-course-06-480x298.jpg',
          lessons: '3 Lessons',
          students: '50 students'
        },
        {
          price: '$30.00',
          text: 'How to Build Confidence in Your Abilities',
          image: 'motivation-course-05-480x298.jpg',
          lessons: '1 Lesson',
          students: '50 students'
        },
        {
          price: '$20.00',
          text: 'Productivity Machine - Focus in a Distracted World',
          image: 'motivation-course-04-480x298.jpg',
          lessons: '5 Lessons',
          students: '50 students'
        },
        {
          price: '$20.00',
          text: 'Effective Time Management Mastery - Complete Guide',
          image: 'motivation-course-03-480x298.jpg',
          lessons: '18 Lessons',
          students: '50 students'
        },
        {
          price: '$25.99',
          text: 'Body Language Secrets for Entrepreneurs',
          image: 'motivation-course-02-480x298.jpg',
          lessons: '19 Lessons',
          students: '50 students'
        },
        {
          price: '$19.99',
          text: 'Management Skills: The Science of Leadership',
          image: 'motivation-course-01-480x298.jpg',
          lessons: '17 Lessons',
          students: '50 students'
        }
      ],
      sponsors: [
        {
          image: 'client-logo-05-primary.png'
        },
        {
          image: 'client-logo-06-primary.png'
        },
        {
          image: 'client-logo-07-primary.png'
        },
        {
          image: 'client-logo-04-primary.png'
        },
        {
          image: 'client-logo-03-primary.png'
        },
        {
          image: 'client-logo-02-primary.png'
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#videosection{
    margin-top: 100px;
}
.class{
    font-size: 40px;
}
#youtube{
    position: relative;
    bottom: 50%;
    left: 260px;
}
i{
    line-height: 2.8;
}
#books{
    margin-top: 100px;
    height: 500px;
}
.bookcover{
    height: 70%;
}
.sx{
    margin-left: 20px;
}
#realstories{
    height: 600px;
}
#sponsors{
    height: 200px;
}
.opacity{
    opacity: 0.5;
}
.section{
    font-size: 15px;
    margin: 10px 0;
}
.grey{
    color: #9cb7c4;
}
.text{
    margin-bottom: 40px;
}

.course{
    height: 250px;
    margin: 20px 0;
}
#viewbtn{
    margin-top: 50px;
}
</style>
