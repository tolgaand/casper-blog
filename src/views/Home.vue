<script>
import BlogPost from "../components/BlogPost.vue";

export default {
  name: "Home",
  components: { BlogPost },
  data() {
    return {
      sampleBlogPosts: [
        {
          title: "Welcome",
          description:
            "Weekly blog articles with all things programming including HTML, CSS, JavaScript and more. Register today to never miss a post!",
          type: "welcome",
          imageUrl: "https://fireblogs-50850.web.app/img/coding.7ab56a95.jpg",
          url: "#",
        },
        {
          title: "DYNAMIC PAGE TITLES WITH THE VUE ROUTER",
          description: "In this video we take a look at creating",
          url: "This is a Fillter Title!",
          imageUrl:
            "https://firebasestorage.googleapis.com/v0/b/fireblogs-50850.appspot.com/o/documents%2FcoverPhoto%2FVue%20Router%20-%20Page%20Titles.png?alt=media&token=3276b1b3-3709-4ff0-bd4a-2de3acd1ad65",
        },
        {
          title: "CSS TRANSFORM: SKEWY | CREATE A SLANTED/SKEWED DIV",
          description: "In this video, we will take a look at the ",
          url: "This is a Fillter Title!",
          imageUrl:
            "https://firebasestorage.googleapis.com/v0/b/fireblogs-50850.appspot.com/o/documents%2FcoverPhoto%2FAccordion-Menu-Vue-js.png?alt=media&token=b784caca-5998-4af3-bb32-51a45f287cb6",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="home">
    <BlogPost
      v-for="(post, index) in sampleBlogPosts"
      :post="post"
      :key="index"
    />
  </div>
</template>
