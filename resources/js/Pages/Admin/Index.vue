<template>
    <div class="flex flex-col h-screen justify-center">
        <div class="bg-blue-900 flex-grow">
            <div
                class="flex flex-col mt-5 items-center m-auto w-full max-w-md px-4 py-8 bg-white rounded-lg shadow dark:bg-gray-800 sm:px-6 md:px-8 lg:px-10"
            >
                <div
                    class="self-center mb-6 text-xl font-light text-gray-600 sm:text-2xl dark:text-white"
                >
                    Acceder a la cuenta
                </div>
                <div class="mt-8">
                    <FormLogin />
                </div>
            </div>
        </div>
        <div class="bg-blue-800 text-center py-3">
            <span class="text-2xl italic m-auto text-blue-200">
                Powered by Ariel Triviño💙
            </span>
        </div>
    </div>
</template>

<script>
import FormLogin from '../../Components/FormLogin.vue';
export default {
  components: { FormLogin },
    name: "IndexAdmin"
};
</script>

<style></style>
