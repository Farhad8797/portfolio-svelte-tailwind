<script>
    let contactInfo = [
        {link:"https://www.facebook.com/profile.php?id=100067398461657", icon:"fa-brands fa-facebook", name: "Facebook"},
        {link:"https://github.com/Farhad8797/", icon:"fa-solid fa-code-branch", name:"Github"},
        {link:"https://leetcode.com/u/Md_Farhad_Hossain/", icon:"fa-solid fa-code", name:"Leetcode"}
    ]
</script>
<h1 class="text-center text-3xl lg:text-4xl py-5">Contact Me</h1>
<section id="Contact Me" class="flex items-center gap-5 lg:gap-8 justify-center p-5">
    <p class="text-2xl">Check out my profiles:</p>
    {#each contactInfo as {link, icon, name}}
        <a href={link} target="_blank" aria-label={name} class="text-2xl lg:text-3xl hover:text-yellow-400 transition duration-500"><span><i class={icon}></i></span></a>
    {/each}
</section>
<h1 class="text-center p-5 text-2xl">Mail me: <span class="italic">gdvbhbhb@gmail.com</span></h1>