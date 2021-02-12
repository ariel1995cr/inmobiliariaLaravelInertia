<template>
    <div>
        <label for="required-email" class="text-gray-700">
            {{ label }}
            <span class="text-red-500 required-dot" v-if="isRequired">
                *
            </span>
        </label>
        <input
            v-bind="$attrs"
            class=" rounded-lg flex-1 appearance-none border border-gray-300 w-full py-2 px-4 bg-white text-gray-700 placeholder-gray-400 shadow-sm text-base focus:outline-none focus:ring-2 focus:ring-purple-600 focus:border-transparent"
            :placeholder="placeholder"
            v-on="$listeners"
            :value="value"
            @input="$emit('update', $event.target.value)"
        />
    </div>
</template>

<script>
export default {
    inheritAttrs: true,
    props: {
        isRequired: {
            required: false,
            default: false,
            type: Boolean
        },
        label: {
            required: true,
            type: String
        },
        placeholder: {
            required: true,
            type: String
        },
        value:{

        }
    },
    model: {
        prop: "value",
        event: "update"
    }
};
</script>

<style></style>
