<template>
  <div class="Resources__Container">
    <h1 class="title is-1 Title__Text">The Ultimate Nuxt Starter Kit</h1>
    <div class="Card__Container">
      <div class="card">
        <div class="card-image">
          <figure class="image">
            <img
              src="https://pbs.twimg.com/profile_images/1114309924551417856/FKA4cm2x.png"
              alt="AWS Amplify"
            />
          </figure>
        </div>
        <div class="card-content">
          <div class="media">
            <div class="media-left">
              <figure class="image is-48x48">
                <img
                  src="https://res.cloudinary.com/practicaldev/image/fetch/s--hn1gu1_d--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/126437/fc030cc4-9f95-4dd2-812e-ffadd8fb4207.jpg"
                  alt="Placeholder image"
                />
              </figure>
            </div>
            <div class="media-content">
              <p class="title is-4">AWS Amplify</p>
              <p class="subtitle is-6">How to Setup Auth</p>
            </div>
          </div>

          <div class="content">
            Awesome article involving setting up AWS Amplify with Auth. See our
            notes for fixes for the tutorials code.
            <a href="https://aws.amazon.com/amplify/" target="_blank"
              >@AWS Amplify</a
            >.
            <a
              href="https://dev.to/aws/adding-authentication-to-a-nuxt-app-with-aws-amplify-2n84"
              target="_blank"
              >@Full Tutorial</a
            >
            <br />
            <time datetime="2020-10-14"></time>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-image">
          <figure class="image">
            <img
              src="https://www.saashub.com/images/app/service_logos/6/4ad2b9991817/large.png?1525414082"
              alt="Bulma CSS Library"
            />
          </figure>
        </div>
        <div class="card-content">
          <div class="media">
            <div class="media-left">
              <figure class="image is-48x48">
                <img
                  src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/643d2790-867f-4622-bf0d-b3ba85156900/dchbge7-30609e93-0fea-4598-b96d-07adf3d72b43.png/v1/fill/w_200,h_200,q_80,strp/another_random_profile_pic_by_thelightning1_dchbge7-fullview.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOiIsImlzcyI6InVybjphcHA6Iiwib2JqIjpbW3siaGVpZ2h0IjoiPD0yMDAiLCJwYXRoIjoiXC9mXC82NDNkMjc5MC04NjdmLTQ2MjItYmYwZC1iM2JhODUxNTY5MDBcL2RjaGJnZTctMzA2MDllOTMtMGZlYS00NTk4LWI5NmQtMDdhZGYzZDcyYjQzLnBuZyIsIndpZHRoIjoiPD0yMDAifV1dLCJhdWQiOlsidXJuOnNlcnZpY2U6aW1hZ2Uub3BlcmF0aW9ucyJdfQ.0Yw9AnKswmKeVutz-DC_Tis8BoHGAapYytz27u3TVAU"
                  alt="Placeholder image"
                />
              </figure>
            </div>
            <div class="media-content">
              <p class="title is-4">Bulma Docs</p>
              <p class="subtitle is-6">Bulma's RTFM!</p>
            </div>
          </div>

          <div class="content">
            Looking for components and other nicely styled CSS things? Look no
            further
            <a href="https://bulma.io/documentation/" target="_blank">@Bulma</a>
            <br />
            <time datetime="2020-10-23"></time>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
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
