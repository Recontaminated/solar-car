<script>
    import Header from "$lib/components/Header.svelte";
</script>

<Header/>
<div class="big">
    <main class="container mx-auto px-6 py-8">
    <section class="w-full py-12 md:py-24 lg:py-32">
        <div class="container grid items-center justify-center gap-4 px-4 text-center md:px-6 lg:gap-10">
            <div class="space-y-3">
                <h2 class="text-lg sm:text-xl md:text-2xl lg:text-3xl xl:text-4xl 2xl:text-5xl font-bold tracking-tighter sm:text-4xl md:text-5xl">
                    Our Sponsors
                </h2>
                <p class="mx-auto max-w-[700px] text-xs sm:text-sm md:text-base lg:text-lg xl:text-xl 2xl:text-2xl text-gray-500 md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed dark:text-gray-400">
                   Our goals would not be possible without the support of our generous sponsors.
                </p>
            </div>
            <!-- Premier Sponsors -->
            <div class="grid grid-cols-1 md:grid-cols-2 divide-x gap-4 sm:overflow-auto">

                    <div class="rounded-lg border bg-card text-card-foreground shadow-sm flex items-center justify-center p-4 sm:p-5">
                        <div class="flex flex-col space-y-1.5 p-4 w-1/2">
                            <img src="https://images.duckarmada.com/31zBPlPfBtMh/direct.png" width="800"
                                 alt="Premier Sponsor Logo"
                                 class="aspect-[2/1] overflow-hidden rounded-lg object-contain object-center">
                        </div>
                        <div class="p-3 w-1/2">
                            <h4 class="text-sm sm:text-base md:text-lg m-1.5 2xl:text-2xl font-bold">Acuity Eye Group</h4>
                            <p class=" text-gray-500 overflow-hidden overflow-ellipsis ">At Acuity Eye Group, we are committed to helping ophthalmologists and optometrists realize their full potential while providing best-in-class patient care to all those in need. We are experts in the business of ophthalmology with years of experience in the industry, a world-class surgeon as our founder, and an unwavering commitment to helping both established practice owners and young professionals further their ophthalmology careers.</p>
<!--                            <button class="inline-flex items-center justify-center rounded-md text-xs sm:text-sm md:text-base lg:text-lg xl:text-xl 2xl:text-2xl font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 text-primary underline-offset-4 hover:underline h-10 px-4 py-2">-->
<!--                                Learn more-->
<!--                            </button>-->
                        </div>
                    </div>

                <div class="rounded-lg border bg-card text-card-foreground shadow-sm flex items-center justify-center p-4 sm:p-5">
                    <div class="flex flex-col space-y-1.5 p-4 w-1/2">
                        <img src="https://images.duckarmada.com/LtJ2xWhuJqA6/direct.png" width="900"
                             alt="Premier Sponsor Logo"
                             class="aspect-[2/1] overflow-hidden rounded-lg object-contain object-center">
                    </div>
                    <div class="p-3 w-1/2">
                        <h4 class="text-sm sm:text-base md:text-lg m-1.5 lg:text-xl 2xl:text-2xl font-bold">East West Bank</h4>
                        <p class=" text-gray-500">For the past 50 years, we’ve built bridges of opportunity for the people, businesses and communities we’ve served and will continue to serve for years to come.</p>
                        <!--                            <button class="inline-flex items-center justify-center rounded-md text-xs sm:text-sm md:text-base lg:text-lg xl:text-xl 2xl:text-2xl font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 text-primary underline-offset-4 hover:underline h-10 px-4 py-2">-->
                        <!--                                Learn more-->
                        <!--                            </button>-->
                    </div>
                </div>

            </div>
            <!-- Standard Sponsors -->
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 divide-x gap-4 sm:overflow-auto">
                {#each [1,2,3,4,5] as _}
                    <div class="rounded-lg border bg-card text-card-foreground shadow-sm flex items-center justify-center p-4 sm:p-8">
                        <div class="flex flex-col space-y-1.5 p-6">
                            <img src="/placeholder.svg" width="140" height="70"
                                 alt="Standard Sponsor Logo"
                                 class="aspect-[2/1] overflow-hidden rounded-lg object-contain object-center">
                        </div>
                        <div class="p-6">
                            <h4 class="text-sm sm:text-base md:text-lg lg:text-xl 2xl:text-2xl font-bold">Standard Sponsor</h4>
                            <button class="inline-flex items-center justify-center rounded-md text-xs sm:text-sm md:text-base lg:text-lg xl:text-xl 2xl:text-2xl font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 text-primary underline-offset-4 hover:underline h-10 px-4 py-2">
                                Learn more
                            </button>
                        </div>
                    </div>
                {/each}
            </div>
        </div>
    </section>
</main>
</div>
<style>
    .big {
        /*background-image: linear-gradient(rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.9)), url("https://images.duckarmada.com/kVIY0CZPaxhd/direct.png");*/
    background-color: #FBFAF5
    }


</style>