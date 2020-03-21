<template>
    <div id="nav-wrap">
        <div id="logo-st">
            <img src="../assets/cropped-logo.png" />
        </div>
        <div id="nav-st">
            <ul>
                <li>link 1</li>
                <li>link 2</li>
                <li>link 3</li>
                <li>link 4</li>
            </ul>
        </div>
        <div class="fix"></div>
    </div>
</template>

<script>

export default {
  name: 'navi',
  /* data (){
      return
  },
  components: {
      editor: Editor
  } */
};
</script>
<style scope="css">
    #nav-wrap {
        margin-bottom: 15px;
    }
    #logo-st{
        width: 100px;
        float:left;
    }
    #logo-st img {
        width: 100%
    }
    #nav-st {
        margin-top: 30px;
    }
    #nav-st ul{
        list-style: none;
        color: #fff;
        font-size: 0.875em;
        color: #fff;
    }
    #nav-st ul li {
        display:inline-block;
        margin-right: 15px;
    }
    #nav-st ul li:last-child {
        margin-right: 0
    }
    #nav-st{
        float:right;
    }

</style>
