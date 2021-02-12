<template>
    <form @submit.prevent="submit" autoComplete="off">
        <div class="flex flex-col mb-2">
            <input-component label="Email" placeholder="Ingrese Email" v-model="form.email" />
        </div>
        <div class="flex flex-col mb-6">
            <input-component
                label="Password"
                placeholder="Ingrese Contraseña"
                v-model="form.password"
            />
        </div>
        <div class="flex w-full">
            <button
                type="submit"
                class="py-2 px-4  bg-blue-900 hover:bg-blue-700 focus:ring-purple-500 focus:ring-offset-blue-200 text-white w-full transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2  rounded-lg "
            >
                Acceder
            </button>
        </div>
    </form>
</template>

<script>
import InputComponent from "./InputComponent.vue";
export default {
    components: { InputComponent },
    data() {
        return {
            form: this.$inertia.form({
                email: "",
                password: "",
                remember: false
            })
        };
    },
    methods: {
        submit() {
            this.form
                .transform(data => ({
                    ...data
                }))
                .post(this.route("login"), {
                    onFinish: () => this.form.reset("password")
                });
        }
    }
};
</script>

<style></style>
