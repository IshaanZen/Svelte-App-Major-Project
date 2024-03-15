<script>
    import logo from "../images/voice-sense.png"
</script>

<header class="flex flex-col relative z-20">
    <div class="max-w-[1400] w-full flex item-centre justify-between py-4 ">
        <a href="/" class="flex ">
            <img class="w-12" src={logo} alt="Logo">
            <h1 id="vs-logo" class=" my-2 mx-3 font text-white text-lg">Voice <span class="  text-white border-2 rounded-3xl p-1 px-5 mx-0">Sense</span></h1>
        </a>
        <button class="md:hidden grid place-items-center">
            <i class="fa-sharp fa-solid fa-bars fa-xl" ></i>
        </button>
        <nav class="hidden md:flex items-center gap-4 lg:gap-4 text-lg">
            <a href="/" class="relative text-lg w-fit block after:block after:content-[''] after:absolute after:h-[3px]
            after:bg-white after:w-full after:scale-x-0 after:hover:scale-x-100 after:transition after:duration-300 after:origin-left my-2 cursor-pointer">Home</a>
            <a href="/about-us" class="relative text-lg w-fit block after:block after:content-[''] after:absolute after:h-[3px]
            after:bg-white after:w-full after:scale-x-0 after:hover:scale-x-100 after:transition after:duration-300 after:origin-left my-2 mx-5 cursor-pointer">About Us</a>
            
            <button class="specialBtn">
                Contact Us
            </button>
        </nav>
    </div>
</header>

<style>
    

    #vs-logo{
        font-family: "Space Mono", monospace;
    }
</style>