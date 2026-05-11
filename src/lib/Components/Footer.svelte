<script>
    let contactInfo = [
        {link:"mailto:gdvbhbhb@gmail.com?subject=Inquiry from Portfolio", icon:"fa-solid fa-envelope", name:"Email"},
        {link:"https://www.facebook.com/profile.php?id=100067398461657", icon:"fa-brands fa-facebook", name: "Facebook"},
        {link:"https://github.com/Farhad8797/", icon:"fa-solid fa-code-branch", name:"Github"},
        {link:"https://leetcode.com/u/Md_Farhad_Hossain/", icon:"fa-solid fa-code", name:"Leetcode"}
    ]
</script>
<h1 class="text-center text-3xl lg:text-4xl py-5">Contact Me</h1>
<section id="Contact Me" class="flex items-center gap-5 lg:gap-8 justify-center p-10">
    {#each contactInfo as {link, icon, name}}
        <a href={link} target="_blank" aria-label={name} class="text-2xl lg:text-3xl hover:text-yellow-400 transition duration-500"><span><i class={icon}></i></span></a>
    {/each}
</section>