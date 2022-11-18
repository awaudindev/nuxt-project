<template>
    <div class="md:fixed flex-col py-10 overflow-y-auto">
            <ul class="w-full h-auto  flex flex-col px-5 text-gray-700 dark:text-gray-200">
                <li class=" w-full" v-for="(menu, index) in menus" :key="index">
                    <button v-if="menu.link"  class="justify-center sm:justify-start relative px-2 sm:px-10 w-full py-3  my-2  flex items-center rounded-lg text-gray-700 dark:text-gray-200 font-bold dark:hover:bg-gray-600 dark:hover:text-gray-300 hover:bg-sky-100 hover:text-sky-700 transition-colors">
                      <p class="hidden sm:block">
                        {{menu.label}}
                      </p>
                      <div v-show="menu.unread != null"  class="w-7 h-7 flex flex-col items-center justify-center bg-gray-200 dark:bg-gray-800 rounded-md absolute -right-4 sm:right-4 ">
                        {{menu.unread}}
                      </div>
                    </button>
                    <div v-else class=" uppercase text-gray-400 font-bold w-full border-t dark:border-gray-800  py-2 px-2 sm:px-10 w-full" >
                    </div>
                </li>
            </ul>
    </div>
</template>

<script>
export default {
    data(){
        return{
            menus:[
                {
                    label:"Beranda",
                    link:"#"
                },
                {
                    label:"Pesan",
                    link:"#"
                },
                {
                    label:"Following",
                    link:"#"
                },
                {
                    label:"Border"
                },
                {
                    label:"Profil",
                    link:"#"
                },
                {
                    label:"Pengaturan",
                    link:"#"
                },
                {
                    label:"Border"
                },
                {
                    label:"Keluar",
                    link:"#"
                }
            ]
        }
    }
}
</script>