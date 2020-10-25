<template>
  <div class="Resources__Container">
    <h1 class="title is-1 Title__Text">The Ultimate Nuxt Starter Kit</h1>
    <div class="Card__Container">
      <div class="card" v-for="post in posts" :key="post.title">
        <div class="card-image">
          <figure class="image">
            <img :src="post.splashImg" :alt="post.splashAlt" />
          </figure>
        </div>
        <div class="card-content">
          <div class="media">
            <div class="media-left">
              <figure class="image is-48x48">
                <img :src="post.authorImg" :alt="post.authorAlt" />
              </figure>
            </div>
            <div class="media-content">
              <p class="title is-4">{{ post.title }}</p>
              <p class="subtitle is-6">{{ post.subtitle }}</p>
            </div>
          </div>

          <div class="content">
            {{ post.content }}
            <a :href="post.refUrl" target="_blank">{{ post.refUrlText }}</a>
            <br />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {
          splashImg:
            "https://pbs.twimg.com/profile_images/1114309924551417856/FKA4cm2x.png",
          splashAlt: "AWS Amplify",
          authorImg:
            "https://res.cloudinary.com/practicaldev/image/fetch/s--hn1gu1_d--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/126437/fc030cc4-9f95-4dd2-812e-ffadd8fb4207.jpg",
          authorAlt: "Image of the Author",
          title: "AWS Amplify",
          subtitle: "How to Setup Auth",
          content:
            "Awesome article involving setting up AWS Amplify with Auth. See our notes for fixes for the tutorials code.",
          refUrl:
            "https://dev.to/aws/adding-authentication-to-a-nuxt-app-with-aws-amplify-2n84",
          refUrlText: "@Full Tutorial"
        },
        {
          splashImg:
            "https://www.saashub.com/images/app/service_logos/6/4ad2b9991817/large.png?1525414082",
          splashAlt: "Bulma CSS Library",
          authorImg:
            "https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/643d2790-867f-4622-bf0d-b3ba85156900/dchbge7-30609e93-0fea-4598-b96d-07adf3d72b43.png/v1/fill/w_200,h_200,q_80,strp/another_random_profile_pic_by_thelightning1_dchbge7-fullview.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOiIsImlzcyI6InVybjphcHA6Iiwib2JqIjpbW3siaGVpZ2h0IjoiPD0yMDAiLCJwYXRoIjoiXC9mXC82NDNkMjc5MC04NjdmLTQ2MjItYmYwZC1iM2JhODUxNTY5MDBcL2RjaGJnZTctMzA2MDllOTMtMGZlYS00NTk4LWI5NmQtMDdhZGYzZDcyYjQzLnBuZyIsIndpZHRoIjoiPD0yMDAifV1dLCJhdWQiOlsidXJuOnNlcnZpY2U6aW1hZ2Uub3BlcmF0aW9ucyJdfQ.0Yw9AnKswmKeVutz-DC_Tis8BoHGAapYytz27u3TVAU",
          authorAlt: "Authors image",
          title: "Bulma Docs",
          subtitle: "Bulma's RTFM!",
          content:
            "Looking for components and other nicely styled CSS things? Look no further",
          refUrl: "https://bulma.io/documentation/",
          refUrlText: "@Bulma"
        }
      ]
    };
  }
};
</script>

<style scoped>
.Title__Text {
  text-align: center;
  margin: 15px;
}
.card {
  width: 300px;
  height: 550px;
  margin: 10px;
}
.Card__Container {
  display: flex;
  justify-content: space-evenly;
  flex-flow: wrap row;
  align-items: center;
  padding: 15px;
}
</style>
