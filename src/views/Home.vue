<script setup lang="ts">
import { Button, CardBody, CardFooter, Accordion } from "@swarmakit/vue"
</script>

<template>
    <CardBody class="bg-[#7067cf] w-10/12 rounded-lg lg:rounded-xl h-[40vh] mx-auto mt-4 lg:mt-10">
        <div class="py-4 lg:py-10 text-center">
            <p class="text-white text-xl lg:text-3xl font-bold"> Hello my name is valentina👋🏼, I'm a software
                developer</p>
        </div>
        <CardFooter  alignment='center' class="flex items-center text-white">
            <Button class=" bg-[#37336a] py-2 px-1 text-sm lg:px-5 lg:py-3  rounded-lg text-white">
                <router-link to="https://valentinabuoro.com">
                    View my portfolio
                </router-link>
            </Button>
        </CardFooter>
    </CardBody>

    <Accordion class="bg-[#37336a] w-10/12 mx-auto py-3 text-white font-medium mt-4 lg:mt-10 rounded px-4">
        <template v-slot:header>
            <h2>Programming Language</h2>

        </template>
        <template v-slot:content >
            <p class="bg-[#fefae0] text-[#37336a] py-2">
                Typescript, Javascript,
            </p>
        </template>

    </Accordion>
    <Accordion class="bg-[#37336a] w-10/12 mx-auto py-3 text-white font-medium mt-4 lg:mt-10 rounded px-4">
        <template v-slot:header>
            <h2>Frontend Frameworks</h2>

        </template>
        <template v-slot:content >
            <p class="bg-[#fefae0] text-[#37336a] py-2">
                React, Vue

            </p>
        </template>

    </Accordion>
    <Accordion class="bg-[#37336a] w-10/12 mx-auto py-3 text-white font-medium mt-4 lg:mt-10 rounded px-4">
        <template v-slot:header>
            <h2>Backend Frameworks</h2>

        </template>
        <template v-slot:content >
            <p class="bg-[#fefae0] text-[#37336a] py-2">
            Nodejs, Express
            </p>
        </template>

    </Accordion>
</template>