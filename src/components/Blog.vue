<template>
    <div class="container" id="blog">
        <div>
            Blog Updated
        </div>
        <h1 class="mt-2 mb-2 font">interesting <span class="verde">articles updated daily</span></h1>
        <div class="row">
            <div class="col-3 mt-2" v-for="(blog, i) in blogs" :key="i">
                <div class="d-flex justify-content-center">
                    <img :src="require(`../assets/${blog.image}`)"/>
                </div>
                <div id="date">
                    <i class="far fa-calendar"></i> {{blog.date}}
                </div>
                <div>
                    <h4 class="title">{{blog.text}}</h4>
                </div>
                <div>
                    {{blog.subtext}}
                </div>
            </div>
        </div>
        <div class="text-center" id="viewall">
            <a href="" class="verde">VIEW ALL POST</a>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Blog',
  data () {
    return {
      blogs: [
        {
          image: 'motivation-blog-04-480x325.jpg',
          date: 'May 13, 2020',
          text: 'How to Stay True to Your Personal Brand',
          subtext: 'When it comes to your business or career, you want..'
        },
        {
          image: 'motivation-blog-03-480x325.jpg',
          date: 'May 13, 2020',
          text: '5 Vital Lessons in 5 Years of Freelancing',
          subtext: 'Being self-employed and working from home, its easy to get..'
        },
        {
          image: 'motivation-blog-02-480x325.jpg',
          date: 'May 13, 2020',
          text: '11 Super Useful Tips for Small-Business Owners',
          subtext: 'Being a small-business owner poses a ton of challenges. We..'
        },
        {
          image: 'motivation-blog-01-480x325.jpg',
          date: 'May 13, 2020',
          text: 'How to Give Yourself Grace to Start Again',
          subtext: 'Forgive yourself for bad habits you may have started or..'
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#blog{
    height: 700px;
}
img{
    height: 200px;
    margin-top: 40px;
}
#date{
    margin: 20px 0;
    margin-left: 5px;
}
#viewall{
    margin-top: 50px;
}
</style>
