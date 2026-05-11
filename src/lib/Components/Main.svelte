<script>
    import Header from '../Components/Header.svelte';
    import Footer from '../Components/Footer.svelte';
    import {onMount} from 'svelte';
    let menu_items = ['About', 'Projects', 'Contact Me'];
    onMount(() => {
        document.documentElement.classList.add('scroll-smooth');
    })
</script>
<nav id="header" class="fixed top-0 left-0 w-full z-50 bg-black/80 backdrop-blur-md flex justify-between sm:p-3 md:p-4 lg:p-5 p-3">
    <h1>Md Farhad Hossain</h1> 
    <div id="menu" class="flex gap-3 sm:gap-x-3 lg:gap-x-4 px-2">
        {#each menu_items as menu_item}
        <a class="border-b-2 border-transparent hover:border-amber-200 transition-all duration-300 pb-1 cursor-pointer" href={'#' + menu_item}>{menu_item}</a>
        {/each}
    </div>
</nav>
<Header/>
<Footer/>
