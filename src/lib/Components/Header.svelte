<script>
   import humanImg from '../assets/human.png';
    let projects = [
        {name: "PyQT6 Weather App", icon: "fa-solid fa-cloud", link: "https://github.com/Farhad8797/simple-weather-app.git", description: "A sophisticated desktop application built with Python and PyQt6 that provides real-time weather information and historical/forecast data visualization. The app features dynamic UI updates, asynchronous-style API integration, and interactive data plotting with Matplotlib."},
        {name: "Employee management API", icon:"fa-brands fa-confluence",link:"https://github.com/Farhad8797/employee-management-api.git", description: "A scalable Node.js backend built with Express, MongoDB, and Redis. This project features a multi-layer security system and optimized data retrieval using a Cache-Aside strategy."}
    ];
</script>


<section id="About" class="grid place-items-center py-[20vh] px-10 lg:flex lg:justify-between lg:py-[5vh] lg:px-10">
    <div id="intro" class="grid place-items-center space-y-3 lg:place-items-start lg:w-1/2">
        <h1 class="text-3xl lg:text-4xl font-bold">I'm <span class="text-amber-300">Farhad</span></h1>
        <p class="text-center lg:text-start">
            As a self taught developer and designer, I'm skilled in 
            <span class="text-lime-400 italic">HTML, CSS, JS, MERN stack, Django, DRF, PyQT6, Figma, Illustrator, Photoshop, Canva.</span>
        </p>
        <p>I can also make content for blogs.</p>
    </div>
    <div id="img" class="mt-10 lg:mt-0">
        <img src={humanImg} alt="Img">
    </div>
</section>

<hr class="m-5 border-green-500">
<p id="Projects" class="text-4xl text-center">My projects</p>

<section class="grid m-10 gap-y-2 place-items-center lg:grid-cols-2 lg:gap-x-2 lg:gap-y-2 lg:place-items-center">
    {#each projects as {name, icon,link, description}}
        <div class="border border-amber-50 p-5 m-5 w-[80vw] grid place-items-center bg-black lg:w-auto lg:h-[40vh]">
            <span><i class={icon}></i></span>
            <a href={link} target="_blank" class="text-2xl text-amber-300 cursor-pointer font-bold p border-b-2 border-transparent hover:border-amber-700 transition duration-300">{name}</a>
            <p class="italic py-2">{description}</p>
        </div>
    {/each}
</section>

<hr class="m-5 border-green-500">
