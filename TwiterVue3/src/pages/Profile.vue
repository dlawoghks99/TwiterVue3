<template>
  <div class="flex-1 flex">
    <!--프로필 섹션-->
    <div class="flex-1 flex flex-col border-r border-gray-100">
        <!--타이틀-->
        <div class="px-3 py-1 flex border-b border-gray-100">
            <button class="mr-4">
                <i class="fas fa-arrow-left text-primary p-3 rounded-full hover:bg-blue-50"></i>
            </button>
            <div>
                <div class="font-extrabold text-lg">김민수</div>
                <div class="text-xs text-gray-500">393 트윗</div>
            </div>
        </div>
        <!-- background 이미지-->
        <div class="bg-gray-300 h-40 relative flex-none">
            <!--프로필 이미지-->
            <div class="border-4 border-white bg-gray-100 w-28 h-28 rounded-full absolute -bottom-14 left-2">
                <img src="http://picsum.photos/100" class="rounded-full opacity-90 hover:opacity-100 cursor-pointer">
            </div>
        </div>
        <!-- 프로필 수정버튼 -->
        <div class="text-right mt-2 mr-2">
            <button class="border text-sm border-primary text-primary px-3 py-2
            hover:bg-blue-50 font-bold rounded-full">프로필 수정</button>
        </div>
        <!-- 사용자 정보-->
        <div class="mx-3 mt-2">
            <div class="font-extrabold text-lg">김민수</div>
            <div class="text-gray-500 ">@minsu-kim</div>
            <div>
                <span class="text-gray-500 ">가입일:</span>
                <span class="text-gray-500 ">2011년10월</span>
            </div>
            <div>
                <span class="font-bold mr-1">28</span>
                <span class="text-gray-500 mr-3">팔로우중</span>
                <span class="font-bold mr-1">7</span>
                <span class="text-gray-500 ">팔로워</span>
            </div>
        </div>
        <!-- tabs-->
        <div class="flex border-b border-gray-100 mt-3">
            <div class="py-3 w-1/4 font-bold text-primary border-b border-primary text-center
                        hover:bg-blue-50 hover:text-primary cursor-pointer">트윗</div>
            <div class="py-3 w-1/4 font-bold  text-center
                        hover:bg-blue-50 text-gray-500 hover:text-primary cursor-pointer">트윗</div>
            <div class="py-3 w-1/4 font-bold  text-center
                        hover:bg-blue-50 text-gray-500 hover:text-primary cursor-pointer">트윗</div>
            <div class="py-3 w-1/4 font-bold  text-center
                        hover:bg-blue-50 text-gray-500 hover:text-primary cursor-pointer">트윗</div>
        </div>
        <!--트윗-->
        <div class="overflow-y-scroll">
            <tweet v-for="tweet in 10" :key="tweet"/>
        </div>
    </div>
    <!--트렌드 섹션-->
    <trends/>
  </div>
</template>

<script>
import Trends from '../components/Trends.vue'
import Tweet from '../components/Tweet.vue'
export default {
  components: { Trends, Tweet },

}
</script>

<style>

</style>