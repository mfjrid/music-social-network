<template>
    <div id="Register">
        <div class="w-full p-6 flex justify-center items-center">
            <div class="w-full max-w-xs">
                <div class="bg-black p-8 shadow rounded mb-6 text-start">
                    <h1 class="mb-6 text-lg text-gray-100 font-thin">Let's Register</h1>
                    <div class="mb-4">
                        <TextInput label="First Name" labelColor="false" placeholder="John" v-model:input="firstName"
                            inputType="text" error="First name error" />
                    </div>
                    <div class="mb-4">
                        <TextInput label="Last Name" labelColor="false" placeholder="Watson" v-model:input="lastName"
                            inputType="text" error="Last name error" />
                    </div>
                    <div class="mb-4">
                        <TextInput label="Email" labelColor="false" placeholder="john@watson.com" v-model:input="email"
                            inputType="text" error="Email error" />
                    </div>
                    <div class="mb-4">
                        <TextInput label="Password" labelColor="false" placeholder="" v-model:input="password"
                            inputType="password" error="Password error" />
                    </div>
                    <div class="mb-4">
                        <TextInput label="Confirm Password" labelColor="false" placeholder=""
                            v-model:input="confirmPassword" inputType="password" error="Confirm Password error" />
                    </div>
                    <button class="block w-full bg-green-500 text-white rounded-sm py-3 text-sm tracking-wide"
                        type="submit">Register</button>
                </div>
                <p class="text-center text-md text-gray-900">
                    Already have an Account?
                    <router-link to="/login" class="text-blue-500 no-underline hover:underline">
                        Login
                    </router-link>
                </p>
            </div>
        </div>
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    import TextInput from '../components/global/TextInput.vue'
    let firstName = ref(null)
    let lastName = ref(null)
    let email = ref(null)
    let password = ref(null)
    let confirmPassword = ref(null)
</script>