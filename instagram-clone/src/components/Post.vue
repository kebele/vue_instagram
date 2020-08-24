<template>
  <div class="post">
      <!-- header -->
    <header class="header">
        <div class="header-author">
        <Avatar size=40 />
        <div class="header-author-info">
            <div>
            <CustomText tag="b">kemalBeler</CustomText>

            </div>
            <div>

            <CustomText size="xsmall">Orlando, Florida</CustomText>
            </div>
        </div>
        </div>
        <div class="header-more">
            <button type="button">
                <IconMore/>
            </button>
        </div>
    </header>


      <!-- media -->
    <div class="post-media">
        <img src="https://fox26medford.com/wp-content/uploads/2020/04/AprilShoe-720x399-1.jpg" alt="">
    </div>

      <!-- action buttons -->



      <!-- view count -->


      <!-- comments list -->




    <!-- date time -->



    <!-- comment form -->
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
import Avatar from '@/components/Avatar'
import IconMore from '@/icons/more.svg' 
export default {
    name : "Post",
    components : {
        Avatar,
        CustomText,
        IconMore,

    }
}
</script>

<style lang="postcss" scoped>
    .post{
        border : 1px solid rgb(var(--b6a));
        border-radius: 3px;
    }
    
    .header{
        height: 60px;
        display: flex;
        align-items: center;

        &-author{
            display: flex;
        align-items: center;
        }
        &-author-info{
            margin-left: 16px;
            /* border : 2px solid black; */
        }
        &-more{
            margin-left: auto;
        }
    }
</style>