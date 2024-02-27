<template>
  <div class="flex-1 flex">
    <!-- 채팅리스트-->
    <div class="w-2/5 border-r border-gray-100 overflow-y-scroll">
        <div class="flex flex-col">
            <div class="p-3 font-bold text-lg border-b border-gray-100">쪽지</div>
            <!-- 채팅-->
            <div class="flex px-3 py-4 hover:bg-gray-50 border-b border-gray-100"
            v-for="message in 5" :key="message">
                <img src="http://picsum.photos/100" class="w-10 h-10 rounded-full cursor-pointer mr-2"/>
                <div>
                    <div class="flex space-x-1">
                        <div class="font-bold">김수진</div>
                        <div class="text-gray-500">sujin123</div>
                        <div class="text-gray-500">2월27일</div>
                    </div>
                    <div class="text-gray-500">메시지</div>
                </div>
            </div>
            <div class="flex px-3 py-4 hover:bg-gray-200 border-b ">
                <img src="http://picsum.photos/100" class="w-10 h-10 rounded-full cursor-pointer mr-2"/>
                <div>
                    <div class="flex space-x-1">
                        <div class="font-bold">김수진</div>
                        <div class="text-gray-500">sujin123</div>
                        <div class="text-gray-500">2월27일</div>
                    </div>
                    <div class="text-gray-500">메시지</div>
                </div>
            </div>
        </div>
    </div>

    <!-- chatting-->
    <div class="w-3/5 border-r border-gray-100">

    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>