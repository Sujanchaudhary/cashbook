<template>
    <section class="py-28">
        <div class="max-w-screen-xl mx-auto px-4 gap-16 justify-between md:px-8 lg:flex">
            <div>
                <div class="max-w-xl space-y-3">
                    <h3 class="text-indigo-600 font-semibold">
                        Features
                    </h3>
                    <p class="text-gray-800 text-3xl font-semibold sm:text-4xl">
                        Simple solutions for complex issues
                    </p>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec congue, nisl eget molestie varius, enim ex faucibus purus
                    </p>
                </div>
                <div class="mt-12 max-w-lg lg:max-w-none">
                    <ul class="space-y-8">
                        <li v-for="(item, idx) in features" :key="idx" class="flex gap-x-4">
                            <div class="flex-none w-12 h-12 bg-indigo-50 text-indigo-600 rounded-lg flex items-center justify-center" v-html="item.icon">
                            </div>
                            <div>
                                <h4 class="text-lg text-gray-800 font-semibold">
                                    {{ item.title }}
                                </h4>
                                <p class="mt-3">
                                    {{ item.desc }}
                                </p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="mt-12 lg:mt-0">
                <img src="https://raw.githubusercontent.com/sidiDev/remote-assets/main/Safari%20(Big%20Sur)%20-%20Light.png" class="w-full shadow-lg rounded-lg border" />
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            features: [
                {
                    icon: `<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6"><path stroke-linecap="round" stroke-linejoin="round" d="M3 13.125C3 12.504 3.504 12 4.125 12h2.25c.621 0 1.125.504 1.125 1.125v6.75C7.5 20.496 6.996 21 6.375 21h-2.25A1.125 1.125 0 013 19.875v-6.75zM9.75 8.625c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125v11.25c0 .621-.504 1.125-1.125 1.125h-2.25a1.125 1.125 0 01-1.125-1.125V8.625zM16.5 4.125c0-.621.504-1.125 1.125-1.125h2.25C20.496 3 21 3.504 21 4.125v15.75c0 .621-.504 1.125-1.125 1.125h-2.25a1.125 1.125 0 01-1.125-1.125V4.125z"/></svg>`,
                    title: "Analytics",
                    desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec congue, nisl eget molestie varius, enim ex faucibus purus."
                },
                {
                    icon: `<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6"><path stroke-linecap="round" stroke-linejoin="round" d="M16.5 10.5V6.75a4.5 4.5 0 10-9 0v3.75m-.75 11.25h10.5a2.25 2.25 0 002.25-2.25v-6.75a2.25 2.25 0 00-2.25-2.25H6.75a2.25 2.25 0 00-2.25 2.25v6.75a2.25 2.25 0 002.25 2.25z"/></svg>`,
                    title: "Datacenter security",
                    desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec congue, nisl eget molestie varius, enim ex faucibus purus."
                }
            ]
        };
    }
}
</script>