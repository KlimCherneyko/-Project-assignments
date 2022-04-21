<template>
<div class="container">
  <div class="up-container">
    <div class="TAKE-YOUR-TIME">TAKE YOUR TIME</div>
    <div class="little-line"></div>
  </div>
  <div class="center-container">
    <div class="center12">
      <div class="story">STORY</div>
      <div class="content">
        <div class="img-222">
          <img src="https://source.unsplash.com/X4RJG4aNi8o/1920x1080" class="img-2">
        </div>
      <div class="text-center">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean varius eget arcu quis cursus. Nunc id tortor imperdiet, vestibulum orci sed, gravida orci. Cras a enim ac elit eleifend euismod. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Praesent mattis ultrices est, congue ullamcorper erat bibendum pulvinar. In accumsan dapibus accumsan. 
    Maecenas semper est ut nunc feugiat, vel ultrices ligula commodo. Donec eget pulvinar nunc, eget pharetra risus.
      </div>
    </div>
    </div>
  </div>
  <div class="bottom-container">
    <div class="story">BLOG</div>
    <div class="bot32">
      <karta v-for="card in cards" :kartochka="card" :key="card.id"/>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'IndexPage',

  data() {
    return {
      cards: [
        {
          id: 1,
          title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean varius eget arcu quis cursus. Nunc id tortor imperdiet, vestibulum orci sed, gravida orci. Cras a enim ac elit eleifend euismod.',
          author: {
            name:'Daily Coffee News',
            photo: 'https://source.unsplash.com/CSQQ6_T0sks/1920x1080',
          },
        },  
        {
          id: 2,
          title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean varius eget arcu quis cursus. Nunc id tortor imperdiet, vestibulum orci sed, gravida orci. Cras a enim ac elit eleifend euismod.',
          author: {
            name:'Dutch Coffee Chains',
            photo: 'https://source.unsplash.com/TYIzeCiZ_60/1920x1080',
          },
        },
        {
          id: 3,
          title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean varius eget arcu quis cursus. Nunc id tortor imperdiet, vestibulum orci sed, gravida orci. Cras a enim ac elit eleifend euismod.',
          author: {
            name:'Start Up In Minneapolis',
            photo: 'https://source.unsplash.com/9rTEwV_G0Do/1920x1080',
          },
        }
      ]
    }
  }
}
</script>

<style >
.container{
  width: 100%;
  max-width: 1442px;
  display:flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
}

.up-container{
  width: 100%;
  height: 812px;
  flex-direction: column;
  display: flex;
  justify-content: center;
  align-items: center;
  align-self: center;
  background:center/cover no-repeat url(https://source.unsplash.com/vSuQJKZkt4U/1920x1080);
}


.TAKE-YOUR-TIME{
  font-weight: 700;
  font-size: 60px;
  line-height: 89px;
  display: flex;
  justify-content: center;
  align-content: center;
  color: #FFFFFF;
  padding-top: 80px;
}

.little-line{
  width: 80px;
  height: 10px;
  background: #817070;
}

.center-container{
  width: 1440px;
  height: 632px;
  color: #FFFFFF;
  display:flex;
  flex-direction: column;
  padding: 60px;
}

.img-2{
  width: 600px;
  height: 400px;
  display: flex;
  align-self: center;
}

.img-222{
  padding: 40px;
}

.text-center{
  font-weight: 300;
  font-size: 20px;
  line-height: 30px;
  display: flex;
  align-self: center;
  color: #000000;
}

.story{
  width: 91px;
  height: 53px;
  font-weight: 500;
  font-size: 36px;
  line-height: 53px;
  text-transform: uppercase;
  color: #000000;
  display: flex;
  justify-content: center;
  align-self: center;
}

.content{
  height: 380px;
  display: flex;
  flex-direction: row;
}

.bot32{
  display: flex;
  flex-direction: row;

}

.center12{
  padding: 60px;
  display: flex;
  flex-direction:column;
}

.bottom-container {
  background: #EFEFEF;
  padding: 60px;
  display: flex;
  flex-direction: column;
}

</style>