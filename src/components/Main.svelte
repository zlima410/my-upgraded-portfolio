<script>
  import Step from './Step.svelte';

  let steps = [
    {name: 'Vector Class Implementation in C++', icon: 'fa-solid fa-circle-nodes', href: 'https://github.com/zlima410/COP4530-DataStructures'},
    {name: 'LC3100 Processor Simulator', icon: 'fa-solid fa-microchip', href: 'https://github.com/zlima410/CDA-processor-simulator'},
    {name: 'LC3100 Cache Simulator', icon: 'fa-solid fa-memory', href: 'https://github.com/zlima410/CDA-cache-simulator'},
  ];

  let benefits = [
    {name: 'a 3.35 GPA student', description: 'Crafting a 3.35 GPA as a Computer Science student at Florida State University was a testament to my disciplined approach to learning. Through unwavering commitment, I diligently balanced theoretical coursework with hands-on projects, leveraging resources like coding boot camps and peer study groups.  This GPA embodies not just academic success but also the dedication and perseverance integral to my journey as a computer scientist.'},
    {name: 'a problem solver', description: "My strength in problem-solving spans various domains, notably in computer science, where my analytical abilities truly thrive. I approach challenges methodically, adapting seamlessly to dissect complex issues and strategize solutions effectively. Whether it's debugging intricate code or tackling real-world problems, my talent lies in breaking down complexities into manageable parts, allowing me to innovate solutions across diverse fields."},
    {name: 'an excellent communicator', description: 'My communication skills allow me to articulate complex technical concepts with clarity and precision. Beyond technical language, I excel in breaking down intricate ideas into easily understandable terms, fostering collaboration among diverse teams. Through active listening, empathy, and effective expression, I not only enhance team dynamics within computer science but also navigate various interpersonal and professional scenarios with ease.'},
  ]
</script>

<main class="flex flex-col flex-1 p-4">
  <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="poppins text-[#F9013F]">Zachary</span> Lima <br/>Full Stack
        <span class="poppins text-[#F9013F]">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-[#F9013F]">favorite tech</span> includes C, C++, Python, Java, JavaScript 
        (SvelteKit, Node.js), TailwindCSS, and Git
      </p>
      <div class="flex flex-row lg:justify-start text-center lg:text-left gap-4 md:gap-6 lg:gap-10">
        <a
        href="mailto:zacharylima2021@gmail.com"
        target="_blank"
        class="redShadow mx-auto lg:mr-0 lg:ml-0 text-base sm:text-lg md:text-xl poppins 
        relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950
        cursor-pointer"
      >
        <div 
          class="absolute top-0 right-full w-full h-full bg-[#F9013F] opacity-20 
          group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative z-9">Get in touch &rarr;</h4>
      </a>
      <a
        href="assets/resume.pdf"
        target="_blank"
        class="redShadow mx-auto lg:mr-0 lg:ml-0 text-base sm:text-lg md:text-xl poppins 
        relative overflow-hidden px-6 py-3 group rounded-full bg-slate-900 text-white
        cursor-pointer"
      >
        <div 
          class="absolute top-0 right-full w-full h-full bg-[#F9013F] opacity-20 
          group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative z-9">Download CV</h4>
      </a>
      </div>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img 
        src={"images/profile-pic.png"} 
        alt="Profile image" 
        class="object-cover z-[2] max-h-[70vh]"/>
    </div>
  </section>

  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text-xl md:text-2xl">
        A few of my creative endeavors.
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="poppins text-[#F9013F]">see</span> my
        work?
      </h3>
    </div>
    <!-- <a 
        href=""
        target="_blank"
        class="mx-auto px-4 py-2 rounded-md border
        border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 
        -mt-10 hover:border-[#F9013F] duration-200">
          <i class="fa-regular fa-circle-play"></i>
          <p>Watch the video</p>
      </a> -->
      <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
        <Step step={steps[0]}>
          <p>An implementation of the standard library vector class and iterator in
            <strong class="text-[#F9013F]">C++! </strong>The class was implemented using the C++11 Big Five.
            The Big Five allow for the dynamic resizing of the vector, as well as the ability to copy and move elements.
          </p>
        </Step>
        <Step step={steps[1]}>
          <p>A processor simulator that simulates the execution of the resulting machine code 
            representation of a program using <strong class="text-[#F9013F]">C!</strong>
            The LC3100 is an 8-register, 32-bit computer. All addresses are word-addresses. 
            The LC3100 has 65536 words of memory.
          </p>
        </Step>
        <Step step={steps[2]}>
          <p>As the processor simulator executes a program, it will access instructions and data. 
            These accesses will be serviced by this cache simulator, which will transfer data to/from memory as needed. 
            This simulator was made with <strong class="text-[#F9013F]">C!</strong>
          </p>
        </Step>
      </div>
  </section>

  <section 
    id="about" 
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col 
    gap-16 sm:gap-20 md:gap-24 relative">
      <div 
        class="flex flex-col gap-2 text-center relative before:absolute before:top-0
        before:left-0 before:w-2/3 before:h-1.5 before:bg-[#F9013F] after:absolute 
        after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-[#F9013F] py-4">
          <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
          <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
            A bit <span class="poppins text-[#F9013F]">about</span> me.
          </h3>
      </div>
      <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am . . .</p>
      <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
        {#each benefits as benefit, index}
        <div class="flex gap-6 sm:gap-8">
          <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
            0{index+1}
          </p>
          <div class="flex flex-col gap-6 sm:gap-8">
            <h3 class="text-2xl sm:text-3xl md:text-5xl">
              {benefit.name}
            </h3>
            <p>{benefit.description}</p>
          </div>
        </div>
        {/each}
      </div>
      <h5 
        class="text-2xl sm:text-3xl font-semibold text-center poppins">
        The <span class="poppins text-[#F9013F]">Complete</span> Package
      </h5>
      <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
        <table class="bg-white text-slate-700 rounded text-center">
          <thead class="border-b border-solid border-slate-200">
            <tr class="">
              <th />
              <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
              <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
              <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
              <th class="whitespace-nowrap bg-[#F9013F] text-white p-4 px-8">Me</th>
            </tr>
          </thead>
          <tbody>
            <tr class="border-b border-solid border-slate-200">
              <td 
                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold 
                text-sm whitespace-nowrap">
                  Dedication
              </td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-green-500"></i></td>
            </tr>
            <tr class="border-b border-solid border-slate-200">
              <td 
                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold 
                text-sm whitespace-nowrap">
                  Critical Thought
              </td>
              <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-green-500"></i></td>
            </tr>
            <tr class="border-b border-solid border-slate-200">
              <td 
                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold 
                text-sm whitespace-nowrap">
                  Interpersonal Skills
              </td>
              <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-green-500"></i></td>
            </tr>
            <tr class="border-b border-solid border-slate-200">
              <td 
                class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold 
                text-sm whitespace-nowrap">
                  Programming Ability
              </td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-slate-500"></i></td>
              <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
              <td><i class="fa-solid fa-check text-green-500"></i></td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
        <p>Scroll to see more &rarr;</p>
      </div>
      <p class="mx-auto">So why not invest?</p>
  </section>
</main>