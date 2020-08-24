<template>
  <div class="post">
      <!-- header -->
    <header class="header section">
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
<div class="action-buttons section">
    <button type="button">
                <IconLike/>
            </button>
    <button type="button">
                <IconComment/>
            </button>
    <button type="button">
                <IconDirect/>
            </button>
    <button class="action-save" type="button">
                <IconSave/>
            </button>
</div>


      <!-- view count -->
<div class="view-count section">
    <CustomText tag="b">3915 beğenme</CustomText>
</div>

      <!-- comments list -->




    <!-- date time -->



    <!-- comment form -->
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
import Avatar from '@/components/Avatar'
import IconMore from '@/icons/more.svg' 
import IconLike from '@/icons/like.svg' 
import IconComment from '@/icons/comment.svg' 
import IconDirect from '@/icons/direct.svg' 
import IconSave from '@/icons/save.svg' 
export default {
    name : "Post",
    components : {
        Avatar,
        CustomText,
        IconMore,
        IconLike,
        IconComment,
        IconDirect,
        IconSave,

    }
}
</script>

<style lang="postcss" scoped>
    .post{
        border : 1px solid rgb(var(--b6a));
        border-radius: 3px;
    }

    .section{
        padding-left: 16px;
        padding-right: 16px;
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

        .action-buttons{
        height: 45px;
        display: flex;
        align-items: center;

        button {
            margin-right: 16px;
        }

        .action-save{
            margin-left: auto;
            margin-right: 0;
        }
        }
</style>