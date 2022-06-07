<template>
  <div class="bg-white align-middle text-slate-900 font-['open_sans'] text-center">
    <div id="nav bar" class="grid grid-cols-2 py-8 bg-slate-500">
      <span id="logo" class="text-2xl font-bold"> Shi Yun Khoo </span>
      <ul id="navigation-items" class="flex flex-row gap-x-5 px-5 text-xl">
        <li><NuxtLink to="/aboutMe">About Me </NuxtLink></li>
        <li><NuxtLink to="/projects">Projects</NuxtLink></li>
        <li><NuxtLink to="/skills">Skills</NuxtLink></li>
        <li><NuxtLInk to="/contact">Contact</NuxtLink></li>
      </ul>
    </div>
    <div id="about me" class="grid grid-cols-2 my-10 px-12">
      <div id="text" class="mx-auto m-5">
        <h5 class="text-left p-5 text-3xl font-bold"> About Me </h5>
        <div class="text-left px-5 text-lg">
          <p> Hello!!!!! It's me. </p>
          <p> Fun fact! I've been programming for xxxx seconds. </p>
        </div>
      </div>
      <div id="pic">
        <img src="" alt="" class="m-5 rounded-md h-96 w-96" />
      </div>
    </div>
    <div id="projects" class="mx-auto m-5 w-3/4">
      <h5 class="text-left p-5 text-3xl font-bold"> Projects </h5>
      <div id="search">
        <div id="search">
          <div id="simple-search" class="mb-10">
            <form class="flex items-center">
              <label for="simple-search" class="sr-only">Simple Search</label>
              <div class="relative w-full">
                <div class="flex absolute inset-y-0 left-0 items-center pl-3 pointer-events-none">
                  <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="h-6 w-6"
                      fill="none"
                      viewBox="0 0 24 24"
                      stroke="currentColor"
                      stroke-width="2"
                  >
                  <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                  />
                  </svg>
                </div>
                <input
                      id="simple-search"
                      v-model="searchInput"
                      type="text"
                      class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5  dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
                      placeholder="Search"
                      required
                >
              </div>
              <button type="submit" class="p-2.5 ml-2 text-sm font-medium text-white bg-blue-700 rounded-lg border border-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                  <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="h-6 w-6"
                      fill="none"
                      viewBox="0 0 24 24"
                      stroke="currentColor"
                      stroke-width="2"
                  >
                  <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                  />
                  </svg>
              </button>
            </form>
          </div>
        </div>
        <div class="mb-10 py-2">
          <p>search by: technology/skill</p>
          <p>search by: project criteria and type</p>
          <p>search by: industry/domain</p>
          <p>sort by: date</p>
        </div>
      </div>
      <hr>
      <div id="current-and-recent" class="my-10">
        <h5 class="text-xl font-bold m-2 p-5 uppercase">Current and Recent</h5>
        <div class="grid grid-cols-3 gap-8">
          <div id="mood music" class="mx-auto">
            <a href="https://mood-music-syk.netlify.app">
            <p class="font-bold">Mood Music</p>
            <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="testos-burgers" class="mx-auto">
            <a href="https://ztm-student-syk.netlify.app">
              <p class="font-bold">Testos Burgers (class project)</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="tonejs-starter" class="mx-auto">
            <a href="">
              <p class="font-bold">ToneJS starter project</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="pollution-monitor" class="mx-auto">
            <a href="">
              <p class="font-bold">Pollution Monitor</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="draw-app" class="mx-auto">
            <a href="https://draw-syk.netlify.app">
              <p class="font-bold">Draw</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="world-clock" class="mx-auto">
            <a href="https://world-clock-syk.netlify.app">
              <p class="font-bold">World Clock</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="tipsod" class="mx-auto">
            <a href="">
              <p class="font-bold">TIPSOD</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="conlang" class="mx-auto">
            <a href="">
              <p class="font-bold">ConLang</p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
          <div id="violate-my-privacy" class="mx-auto">
            <a href="">
              <p class="font-bold">VIOLATE my privacy </p>
              <img src="" alt="" class="h-48 w-48" />
            </a>
          </div>
        </div>
      </div>
      <hr>
      <div id="featured" class="m-10 text-left">
        <h5 class="my-10 text-center text-xl font-bold uppercase">Featured</h5>
        <div id="web development" class="my-5">
          <h3 class="text-lg font-bold uppercase"> Web Development </h3>
          <div id="front-end">
            <h5 class="font-bold">Front Ends and Web Design </h5>
            <p> front ends and web design </p>
            <p> styles e.g. minimalist, neumorphic </p>
            <p> animated, webGL </p>
            <p> showcase variety and understanding of common requirements and your ability to hit them</p>
            <p> add explanation of your processes and about the project </p>
          </div>
          <div id="vue-projects">
            <p class="font-bold"> Vue projects </p>
          </div>
          <div id="firebase-projects">
            <p class="font-bold"> Firebase projects </p>
          </div>
          <div id="audio-programming">
            <p class="font-bold">audio programming</p>
            <p> synthesizers, audiovisualizers, spectrograms, audio analyzers, generative music, signal processing, fluid dynamics</p>
          </div>
          <div id="web-gl">
            <p class="font-bold">webGL projects</p>
          </div>

          <div id="media" class="my-5">
            <p class="font-bold">web audio, web media ...</p>
          </div>
          <div id="personal-projects" class="my-5">
            <p>personal and class projects, e.g. standard curriculum projects + personal interests</p>
            <p> matterJS, toneJS </p>
            <p> do something about SEO </p>
            <p> do something about cybersecurity </p>
            <p> wordpress, SSGs etc.</p>
          </div>
        </div>
        <div id="creative-coding-and-generative-art" class="my-5">
          <p class="text-lg font-bold uppercase">creative coding</p>
        </div>
        <div id="data-science" class="my-5">
          <p class="text-lg font-bold uppercase">data science projects</p>
          <p>visualizations, scraping, machine learning</p>
          <p>classification by industry and field, methods</p>
        </div>
         <div id="data-science" class="my-5">
          <p class="text-lg font-bold uppercase">python projects</p>
        </div>
        <div id="IoT-projects" class="my-5">
          <p class="text-lg font-bold uppercase">internet of things/physical computing</p>
        </div>
        <div id="other" class="my-5">
          <p class="text-lg font-bold uppercase">other</p>
          <p> projects with: go, dart, swift, flutter, firebase, AWS, Azure, PHP, Ruby on Rails, C, C++, Python</p>
          <p> projects with operating systems, electronics, networks ... </p>
          <p> actual scientific research or other research projects or field projects </p>
        </div>
      </div>
      <div class="m-10 text-left">
        <div id="infographics-videos-courses">
          <p class="text-lg font-bold">infographics, videos, courses, teaching</p>
        </div>
        <div id="qualifications-and-certifications">
          <p class="text-lg font-bold">qualifications and certifications and events attended</p>
        </div>
        <div id="proficiency-and-experience">
          <p class="text-lg font-bold">proficiency and experience with different platforms, technologies, languages</p>
        </div>
        <div id="other skills">
          <p class="text-lg font-bold"> e.g. project management, digital marketing, sales, accounting ... audio production </p>
        </div>
        <div id="domain-knowledge">
          <p class="text-lg font-bold"> drop some slides or videos or write some articles or something </p>
        </div>
        <div id="soft skills">
          <p class="text-lg font-bold">something to demonstrate soft skills</p>
        </div>
        <!-- clarify objectives. monitor, assess, repeat. Visit frequently. Be seen for who you really are, let your personality come through, meet all core competencies, demonstrate experience and core strengths -->
      </div>
    </div>
    <hr>
    <div id="skills" class="mb-10">
      <h5 class="my-10 text-3xl font-bold"> Skills </h5>
      <table class="mx-auto w-2/3 border-2 border-black">
        <thead class="font-bold border-2 border-black">
          <td>Skill</td>
          <td>Level</td>
          <td>Experience</td>
        </thead>
        <tr>
          <td>JavaScript</td>
          <td>a</td>
          <td>b</td>
        </tr>
        <tr>
          <td>JavaScript</td>
          <td>a</td>
          <td>b</td>
        </tr>
        <tr>
          <td>JavaScript</td>
          <td>a</td>
          <td>b</td>
        </tr>
      </table>
    </div>
    <hr>
    <div id="references" class="m-10">
      <p class="text-xl font-bold m-2 uppercase">references</p>
    </div>
    <hr>
    <div id="links" class="m-10">
      <p class="text-xl font-bold m-2 uppercase">links</p>
      <p class="font-bold">Personal home page</p>
      <p class="font-bold">General resume</p>
      <p class="font-bold">Social media accounts</p>
      <ul class="grid grid-cols-4 w-3/4 mx-auto">
        <li>Facebook</li>
        <li>Instagram</li>
        <li>Pinterest</li>
        <li>YouTube</li>
      </ul>
    </div>
    <hr>
    <footer class="mx-auto my-10 text-md">
      <p class="py-1">Last updated: Sunday, 5th June 2022</p>
      <p class="py-1">Made with ❤️ in Malaysia</p>
    </footer>
  </div>
</template>
