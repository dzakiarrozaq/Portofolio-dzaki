<script>
export default {
  data() {
    return {
      activeTab: 1,
      tech: [
        {
          id: 1,
          name: 'Kotlin',
          imageUrl: 'https://www.logo.wine/a/logo/Kotlin_(programming_language)/Kotlin_(programming_language)-Logo.wine.svg',
          status: 'Advanced'
        },
        {
          id: 2,
          name: 'Flutter',
          imageUrl: 'https://img.icons8.com/?size=100&id=7I3BjCqe9rjG&format=png&color=000000',
          status: 'Intermediate'
        },
        {
          id: 3,
          name: 'Compose',
          imageUrl: 'https://miro.medium.com/v2/resize:fit:1400/0*By3pK69IFk_RqbF3.png',
          status: 'Intermediate'
        },
        {
          id: 4,
          name: 'Java',
          imageUrl: 'https://cdn4.iconfinder.com/data/icons/logos-and-brands/512/181_Java_logo_logos-512.png',
          status: 'Intermediate'
        },
        {
          id: 5,
          name: 'Firebase',
          imageUrl: 'https://avatars.githubusercontent.com/u/1335026?s=200&v=4',
          status: 'Beginner'
        },
        {
          id: 6,
          name: 'TF Lite',
          imageUrl: 'https://codelabs.tf.wiki/codelabs/recognize-flowers-with-tensorflow-on-android/img/657431be3173fa86.png',
          status: 'Beginner'
        }
      ],
      tools: [
        {
          id: 1,
          name: 'Android Studio',
          imageUrl: 'https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/android-studio-icon.png',
          status: 'Code Editor'
        },
        {
          id: 2,
          name: 'Figma',
          imageUrl: 'https://seekvectors.com/storage/images/Figma-01.svg',
          status: 'Design Tool '
        },
        {
          id: 3,
          name: 'GitHub',
          imageUrl: 'https://static-00.iconduck.com/assets.00/github-icon-512x497-oppthre2.png',
          status: 'Git Hosting'
        },
        {
          id: 4,
          name: 'Git',
          imageUrl: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png',
          status: 'Version Control'
        }
      ],
      socials: [
        {
          name: 'LinkedIn',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-linkedin-logo-icon-download-in-svg-png-gif-file-formats--social-media-pack-logos-icons-498418.png?f=webp&w=256',
          link: 'https://www.linkedin.com/in/muhammad-dzaki-arrozaq'
        },
        {
          name: 'Instagram',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Instagram_icon.png/600px-Instagram_icon.png',
          link: 'https://instagram.com/dzakijoo'
        },
        {
          name: 'Spotify',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-spotify-logo-icon-download-in-svg-png-gif-file-formats--social-media-technology-pack-logos-icons-3147690.png?f=webp&w=128',
          link: 'https://open.spotify.com/user/31tdh6aq4to2ng3bfexhvlucc7bm?si=d776e6d7b6e14f70'
        },
        {
          name: 'Email',
          imageUrl: 'https://cdn1.iconfinder.com/data/icons/google-new-logos-1/32/gmail_new_logo-512.png',
          link: 'mailto:dzakiarrozaq21@gmail.com'
        },
      ]
    };
  }
}
</script>
<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Me &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-9/12 max-w-[450px] rounded-full mb-3 fadein-up"
            src="img/protfolio-about.jpg" alt="Foto">
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; Hi everyone! I'm Muhammad Dzaki Arrozaq, a Computer Science student focusing on Information Technology at 
            Universitas Negeri Semarang. I'm passionate about mobile development, especially Android, and I also have a strong interest in 
            UI/UX design. I love creating apps that look great and are easy for people to use.
          </p>
          <p class="mb-3 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp; Collaborating to make impactful, user-friendly apps is what excites me, and I’m known for my fresh ideas 
            and staying calm under pressure. I'm always eager to keep growing in mobile development and connect with others who share similar 
            passions in this fast-moving field!
          </p>
          <div class="flex justify-center gap-8 mt-5 fadein-left fadeins-3">
            <a v-for="social in socials" :key="social.name" :href="social.link" target="_blank" rel="noopener noreferrer"
               class="hover:opacity-80 transition-opacity">
              <img :src="social.imageUrl" :alt="social.name" class="w-8 h-8">
            </a>
          </div>
        </div>

      </section>

    </article>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
          <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Tools</button>
            </li>
          </ul>
        </div>
        <div v-show="activeTab === 1">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tech" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div v-show="activeTab === 2">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tools" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.fadeins-3 {
  animation-delay: 1200ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
