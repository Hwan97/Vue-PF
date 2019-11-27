<template>
  <div class="Main-wrap">
    <div class="Main-Title">
      <h1>Front-end Developer <br/>Heo Ji Hwan</h1>
    </div>
    <div class="Main-Content">
      <div class="Main-Content-logo">
        <a href="http://allinfom.tistory.com/" title="블로그 바로가기"><img src="https://image.flaticon.com/icons/png/128/8/8708.png" alt="me" width="40px"></a>
        <a href="https://hwan97.github.io/2018-PF/" title="포트폴리오 바로가기"><img src="https://image.flaticon.com/icons/png/128/236/236817.png" alt="me" width="40px"></a>
        <a href="https://github.com/Hwan97" title="GitHub 바로가기"><img src="https://image.flaticon.com/icons/png/128/733/733609.png" alt="me" width="40px"></a>
      </div>
    </div>
    <div class="main_link">
      <div class="main_link_content shadow">
        <a href="http://allinfom.tistory.com/">Blog</a>
        <a href="https://hwan97.github.io/Jh-PortFolio">PortFolio</a>
        <a href="https://github.com/Hwan97">GitHub</a>
      </div>
    </div>
    <p class="caption">
      방문해주셔서 감사합니다.
      <small>© Copyright Ji Hwan all right reserved.</small>
    </p>
  </div>
</template>
<script>
export default {
}
</script>

<style scoped>
.Main-Title{
  width: 100%;
  text-align: center;
  margin-top:10%;
  padding-bottom: 2.5%
}
.Main-Title h1{
  font-weight:100 ;
  color:#343a40;
  font-size:40px;
}
.Main-Content{
  text-align: center;
}
.Main-Content-logo a{
  padding: 20px;
}
.main_link{
  width: 100%;
  text-align: center;
  line-height: 150px;
}
.main_link_content a{
      background: #343a40;
      color:white;
      padding: .375rem .75rem;
      display: inline-block;
      white-space: nowrap;
      vertical-align: middle;
      -webkit-user-select: none;
      -moz-user-select: none;
      -ms-user-select: none;
      user-select: none;
      border: 1px solid transparent;
      font-size: 1rem;
      line-height: 1.5;
      border-radius: .25rem;
      transition: background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;
}
.main_link_content a:hover{
   background: white;
  color:black;
  border:1px solid #343a40;
  border-radius: 10px;
}
.caption{
  text-align: center;
  font-size: 13px;
  margin-top:10rem;
}
.caption small{
  display: block;
}
</style>
