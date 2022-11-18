<template>
    <div class=" flex flex-col relative w-full h-full p-2 md:p-10 text-white">
        <ul class="flex flex-col h-auto">
            <li v-for="(list, index) in lists" :key="index" class="flex flex-col rounded-lg transition-shadow cursor-pointer hover:shadow-2xl hover:shadow-blue-300 dark:hover:shadow-gray-900 w-full p-5 bg-white dark:bg-gray-700 mb-4" >
                <div class="flex items-center gap-x-4 mb-5">
                    <div class="relative  w-10 h-10">
                        <img :src="list.picture" class="  rounded-full bg-sky-300 w-full h-full object-cover" alt="">
                    </div>
                    <strong class="font-bold" >
                        {{list.author}}
                    </strong>
                </div>
                <div class="w-full flex flex-col px-2">
                    <img :src="list.picture" class="  rounded bg-sky-300 w-full h-auto" alt="">
                    <div class="flex my-2">
                     <h1 class="font-bold text-[24px]">{{list.title}}</h1>
                    </div>
                    <p>
                        {{list.content}}
                    </p>
                </div>
            </li>
         </ul>
    </div>
</template>

<script>
export default {
    data(){
        return{
            lists:[
                {
                    author:"Filipe Lukebana",
                    title:"Some Random Title",
                    content:"Do laboris consequat ut aute. Dolor minim ea excepteur officia et anim nulla proident nisi non et eu culpa consequat.. ",
                    picture:"https://picsum.photos/200/300"
                },
                {
                    author:"Rita Naomi",
                    title:"Some Random Title from Rita",
                    content:"Do laboris consequat ut aute. Dolor minim ea excepteur officia et anim nulla proident nisi non et eu culpa consequat.. ",
                    picture:"https://picsum.photos/201/300"
                },
                {
                    author:"Alexandre",
                    title:"Some Random Title from Alexandre",
                    content:"Do laboris consequat ut aute. Dolor minim ea excepteur officia et anim nulla proident nisi non et eu culpa consequat.. ",
                    picture:"https://picsum.photos/202/300"
                },
                {
                    author:"Daniel Tomás",
                    title:"Some Random Title from Daniel",
                    content:"Do laboris consequat ut aute. Dolor minim ea excepteur officia et anim nulla proident nisi non et eu culpa consequat.. ",
                    picture:"https://picsum.photos/203/300"
                },
            ]
        }
    }
}
</script>