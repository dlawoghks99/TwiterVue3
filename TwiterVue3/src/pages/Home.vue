<template>
  <!-- 메인 섹션-->
  <div class="flex-1 border-r border-gray-100 overflow-y-auto">
          <div class="flex flex-col">
            <!-- 페이지 타이틀-->
            <div class="border-b border-gray-100 px-3 py-2 font-bold text-lg">홈</div>
            <!-- 트위팅 섹션-->
            <div class="flex px-3 py-3 border-b-8 border-gray-200">
              <img src="http://picsum.photos/200" class="w-10 h-10 rounded-full hover:opacity-80 cursor-pointer" />
              <div class="ml-2 flex-1 flex flex-col">
                <textarea placeholder="무슨 일이 일어나고 있나요?"
                class="w-full text-lg font-bold focus:outline-none mb-3 resize-none "></textarea>
                <div class="text-right">
                  <button class="bg-primary hover:bg-dark text-sm font-bold text-white px-4 py-1 rounded-full">트윗</button>
                </div>
              </div>
            </div>
            <!-- 트위츠-->
            <tweet/>
          </div>
        </div>
        <!-- 트렌드 섹션-->
        <Trands />
</template>

<script>
import Trands from '../components/Trends.vue'
import Tweet from '../components/Tweet.vue'

export default {
    components : { Trands, Tweet},
    setup(){},
}
</script>

<style>

</style>