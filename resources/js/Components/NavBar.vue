<template>
    <nav
        class="flex bg-blue-900 flex-wrap items-center justify-between p-8 border-b border-white shadow-2xl"
    >
        <div class="lg:order-2 w-auto lg:w-1/5 lg:text-center">
            <a
                class="text-xl text-blue-100 font-semibold font-heading"
                href="#"
            >
                <img
                    alt="profil"
                    src="/Images/logoAdan.png"
                    class="mx-auto object-cover"
                />
            </a>
        </div>
        <div class="block lg:hidden">
            <button
                class="navbar-burger flex items-center py-2 px-3 text-indigo-500 rounded border border-indigo-500"
            >
                <svg
                    class="fill-current h-3 w-3"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <title>
                        Menu
                    </title>
                    <path
                        d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"
                    ></path>
                </svg>
            </button>
        </div>
        <div
            class="navbar-menu font-mono hidden lg:order-1 lg:block w-full lg:w-2/5"
        >
            <a
                class="transform hover:scale-110 motion-reduce:transform-none block lg:inline-block mt-4 lg:mt-0 mr-10 text-blue-100 hover:text-blue-300"
                href="#"
            >
                Inicio
            </a>
            <a
                class="transform hover:scale-110 motion-reduce:transform-none block lg:inline-block mt-4 lg:mt-0 mr-10 text-blue-100 hover:text-blue-300"
                href="#"
            >
                Inmuebles
            </a>
            <a
                class="transform hover:scale-110 motion-reduce:transform-none block lg:inline-block mt-4 lg:mt-0 text-blue-100 hover:text-blue-300"
                href="#"
            >
                Tasación
            </a>
        </div>
        <div
            class="navbar-menu font-mono hidden lg:order-3 lg:block w-full lg:w-2/5 lg:text-right"
        >
            <a
                class="transform hover:scale-110 motion-reduce:transform-none block lg:inline-block mt-4 lg:mt-0 mr-10 text-blue-100 hover:text-blue-300"
                href="#"
            >
                Quien soy?
            </a>
            <a
                class="transform hover:scale-110 motion-reduce:transform-none block lg:inline-block mt-4 lg:mt-0 mr-10 text-blue-100 hover:text-blue-300"
                href="#"
            >
                Contacto
            </a>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar'
};
</script>

<style></style>
