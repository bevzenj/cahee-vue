<template>
<main class="main">
    <Intro />
    <About />
    <Services />
    <Gallery />
    <Subscribe />
    <Blog />
    <Contact />
</main>
</template>

<script>
import Intro from '@/components/Intro.vue';
import About from '@/components/About.vue';
import Services from '@/components/Services.vue';
import Gallery from '@/components/Gallery.vue';
import Subscribe from '@/components/Subscribe.vue';
import Blog from '@/components/Blog.vue';
import Contact from '@/components/Contact.vue';

export default {
  name: 'Main',
  components: {
    Intro,
    About,
    Services,
    Gallery,
    Subscribe,
    Blog,
    Contact,
  },
};
</script>
