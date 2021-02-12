<template>
    <div class="flex flex-col">
        <h1
            class="font-light w-full uppercase text-center text-4xl sm:text-5xl dark:text-white text-gray-800"
        >
            Inmuebles Destacados
        </h1>
        <div class="flex items-center justify-center mt-4">
            <div
                class="flex max-w-md bg-white shadow-lg rounded-lg overflow-hidden"
            >
                <div class="w-2/3 bg-cover bg-landscape">
                    <img
                        class="max-h-96"
                        src="https://static.tokkobroker.com/pictures/103886652664854807232307881592667184598824308648136770725351888012998610199616.jpg"
                    />
                </div>
                <div class="w-2/3 p-4">
                    <h1 class="text-gray-900 font-bold text-2xl">
                        CASA
                    </h1>
                    <p class="mt-2 text-gray-600 text-sm ">
                        La misma está en un barrio que se encuentra en una
                        ubicación privilegiada de la zona norte de nuestra
                        ciudad por encontrarse en cercanías del mar y de la Ruta
                        que conecta.
                    </p>
                    <div class="flex item-center mt-2"></div>
                    <div class="flex item-center justify-between mt-3">
                        <h1 class="text-gray-700 font-bold text-xl">
                            Precio
                        </h1>
                        <button
                            class="px-3 py-2 bg-gray-700 text-white text-xs font-bold uppercase rounded"
                        >
                            Me interesa
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.bg-gray-100 {
    background-color: #f7fafc;
    background-color: rgba(247, 250, 252, var(--tw-bg-opacity));
}

.border-gray-200 {
    border-color: #edf2f7;
    border-color: rgba(237, 242, 247, var(--tw-border-opacity));
}

.text-gray-400 {
    color: #cbd5e0;
    color: rgba(203, 213, 224, var(--tw-text-opacity));
}

.text-gray-500 {
    color: #a0aec0;
    color: rgba(160, 174, 192, var(--tw-text-opacity));
}

.text-gray-600 {
    color: #718096;
    color: rgba(113, 128, 150, var(--tw-text-opacity));
}

.text-gray-700 {
    color: #4a5568;
    color: rgba(74, 85, 104, var(--tw-text-opacity));
}

.text-gray-900 {
    color: #1a202c;
    color: rgba(26, 32, 44, var(--tw-text-opacity));
}

@media (prefers-color-scheme: dark) {
    .dark\:bg-gray-800 {
        background-color: #2d3748;
        background-color: rgba(45, 55, 72, var(--tw-bg-opacity));
    }

    .dark\:bg-gray-900 {
        background-color: #1a202c;
        background-color: rgba(26, 32, 44, var(--tw-bg-opacity));
    }

    .dark\:border-gray-700 {
        border-color: #4a5568;
        border-color: rgba(74, 85, 104, var(--tw-border-opacity));
    }

    .dark\:text-white {
        color: #fff;
        color: rgba(255, 255, 255, var(--tw-text-opacity));
    }

    .dark\:text-gray-400 {
        color: #cbd5e0;
        color: rgba(203, 213, 224, var(--tw-text-opacity));
    }
}
</style>

<script>
import HomeLayout from "../Layouts/HomeLayout.vue";
export default {
    layout: [HomeLayout],
    props: {
        canLogin: Boolean,
        canRegister: Boolean,
        laravelVersion: String,
        phpVersion: String
    }
};
</script>
