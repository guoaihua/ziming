<template>
  <div class="navbar">
    <div class="zm-navbar_header">
      头部
    </div>
    <div class="zm-navbar_list">
      <ul>
        <li class="zm-list"><router-link to="/">home</router-link></li>
        <li class="zm-list"><router-link to="/">Getting</router-link></li>
        <li class="zm-list"><router-link to="/">test1</router-link></li>
        <li class="zm-list"><router-link to="/">api</router-link></li>
        <li class="zm-list"><router-link to="/">contact</router-link></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navbar',
};
</script>

<style scoped lang="scss">
    $height: 100px;
    .navbar {
      width: 100%;
      height: $height;
      display: flex;
      justify-content: left;
      background: #1e1917;
      font-family: blod;
      font-size: 16px;
      .zm-navbar_header {
        color: #ffffff;
        height: 100%;
        width: 100px;
        display: inline-block;
        line-height: $height;
      }
      .zm-navbar_list {
        display: inline-block;
        height: 100%;
        line-height: $height;
        ul {
          height: 100%;
          .zm-list {
            width: 50px;
            list-style: none;
            float: left;
            a {
              text-decoration: none;
              color: #CE8E32;
              text-align: center;
            }
            a:hover {
              color: #ffffff;
            }
          }
        }
      }
    }
</style>
