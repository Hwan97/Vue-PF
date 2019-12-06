<template lang="html">
  <div class="wrap">
    <div class="sideform-btn">
      <a href="#" id="side-btn" @click="showIntro" ><img src="https://vuejsexamples.com/favicon.png" alt="" width="40px" id="btn-img">
      </a>
      <span>← Click</span>
    </div>
    <div id="sideform">
      <span class="close-btn" @click="closeIntro">
          <span v-for="(x, index) in 2" :key="x" class="bm-cross" :style="{position: 'absolute', width: '3px', height: '14px',background:'#fff',transform: index === 1 ? 'rotate(45deg)' : 'rotate(-45deg)'}">
      </span>
      </span>
      <div id="sidemenu">
          <img src="https://image.flaticon.com/icons/svg/265/265755.svg" alt="" :style="{width: '100px', padding: '50px 70px'}">
        <ul>
          <li>이름 : 허지환</li>
          <li>나이 : 23살</li>
          <li>지역 : 서울</li>
          <li>취미 : 운동</li>
          <li>안녕하세요. 최근에 저는</li>
          <li>컴퓨터활용능력1급 을 취득하고</li>
          <li>정보처리기능사를 취득했습니다.</li>
          <li>학점은행제를 하고 있으며 현재</li>
          <li>컴퓨터공학과 재학중이며 4학년 정도</li>
          <li>됩니다. 내년 초 졸업예정입니다.</li>
          <li>이 포트폴리오는 학원 수료후</li>
          <li>2018년도에 제작되었습니다.</li>
          <li>항상 스스로를 계발하는 개발자가</li>
          <li>되고 싶습니다. 연락주세요!</li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    showIntro(){
      // this.$nextTick(function() {
      //      document.getElementById('sideform').style.width = this.width
      //        ? this.width + 'px'
      //        : '300px';
      //    });
   document.getElementById('sideform').style.left = '0px';
   document.getElementById('btn-img').style.transform = 'rotate(180deg)';
 },
 closeIntro(){
   document.getElementById('sideform').style.left = '-300px';
   document.getElementById('btn-img').style.transform = 'rotate(0deg)';
 }
  }
}
// showIntro(){
//    // this.$emit('showIntro');
//

//    // document.getElementById('sidemenu').style.display = 'block';
// }

</script>

<style>
  #sideform{
    height: 80%;
    width:300px;
    background: #41b883;
    position: fixed;
    top:0;
    left: -300px;
    transition: 1s;
    box-shadow: 0 24px 80px rgb(51, 77, 99);
  }
  .sideform-btn span{
    font-size:11px;
    font-weight: bold;
  }
  #sidemenu{
    transition: 5s;
  }
  #sidemenu li{
    color:white;
    font-size: 13px;
    line-height: 30px;
  }
  #sidemenu li:nth-child(4){
    padding-bottom: 25px;
  }
  #side-btn{
    margin-left: 300px;
  }
  #side-btn img{
    transition: 1s;
  }.close-btn {
    height: 24px;
    width: 24px;
    cursor: pointer;
    position: absolute;
    right: 2px;
    top: 12px;
}
</style>
