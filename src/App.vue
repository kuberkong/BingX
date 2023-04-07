<template>
    
    <div class="wrap">
        <a href="#"><img class="img1" src="data:image/png;base64,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" alt=""></a>
        <nav>
            <a href="#">語言</a>
            <a href="#">個人資料</a>
        </nav>
    </div>
    
   
    <div class="header">
        <nav>
            <h1 class="about">
             
                <a href="#"><font-awesome-icon :icon="['fass', 'house']" class="bbb"/><img src=""/>資料看板</a>
                <a href="#"><img src=""/>資料詳情</a>
                <a href="#"><img src=""/>佣金明細</a>
                <a href="#"><img src=""/>客戶管理</a>
                <a href="#"><img src=""/>合夥人管理</a>
            </h1>
        </nav>
            <div class="about-1">
                <h2>資料看板</h2>
                <h3>資料概況</h3>
                <img src="i警示" alt=""> 
                <p>最新資料更新時間：2023/04/05 11:08(UTC+8)；統計時區以UTC+8為準· 
                    當日佣金資料將在次日0點~1點（UTC+8）進行結算，結算過程可能存在延時，請在結算完成後進行檢視。當前頁面不包含今日佣金資料。
                </p> 
                <input type="">
            </div>      
    </div>

        <nav class="nose">
              <h1>用戶佣金明細</h1>
              <a href="#">全部</a>
              <a href="#">標準合約</a>
              <a href="#">永續合約</a>
              <a href="#">現貨</a>
              <a href="#">外部跟單</a>
        </nav>

</template>

<script setup>
    
</script>

<style>
*{
    margin: 0;
    padding: 0;
    list-style:none;
}
.bbb { 
    padding-right: 10px;
    width: 25px;
    height: 25px;
}
.header {
    display: flex;
    background-color: antiquewhite;
    width: 100%;
}
.about{
    display: flex;
    flex-direction: column;
    width: 180px;
    background-color:#fff;


}
.about a {
    line-height: 25px;
    padding: 20px;
    color:black;
    text-decoration: none;
    transition: .5s;
    border-radius: 10%;
    text-align: end;
    font-weight: bold;
}
.about a:hover {
    background-color:aquamarine;
}
.img1 {
    width: 400px;
    height: 100px;
}
.wrap {
    display: flex;
    justify-content: space-between;
}
.wrap nav {
    width: 200px;
    height: 20px;
}
.wrap nav a {
    padding: 20px 13px;
    justify-content: space-around;
    text-decoration: none;
    line-height: 50px;
    border-radius: 10%;
    transition: .5s;
    color:black;
    font-weight: bold;
}
.wrap nav a:hover {
    background-color: aquamarine;
}
.nose h1 {
    display:block;
    padding: 20px 20px 15px;
}
.nose a {
    padding: 10px;
    text-decoration: none;
    color: #000;
}
.nose a:hover {
    color:chocolate;
}
</style>

