<script setup></script>

<template>
  <div>
    <img
      src="https://image.api.playstation.com/vulcan/img/cfn/11307NUlRPcxCgzizu6gpFZiR_WIqYHV9W0G8obBn0J1qCXY-SjbkzKihVNA3WzUQHbD08zWVaN-a7U5--t57lc-gckkQ0f-.png"
    />
    <h1>ыыы</h1>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Molestiae
      doloremque beatae cumque numquam eaque id! Accusamus modi praesentium,
      molestiae exercitationem deleniti, totam tempore sit, ab laudantium quae
      consequatur aliquid! Eveniet!
    </p>
    <nav>
      <i class="fas fa-history"></i>
      <span>2450</span>
    </nav>
    <nav>
      <i class="fas fa-tv"></i>
      <span>24670</span>
    </nav>
    <button>Подробнее</button>
  </div>
</template>

<style scoped>
div{
    width: 500px;
    background-color: #FEDAC2;
    padding: 20px;
    border-radius: 40px;
    color: #C02A1B;
    display: flex;
    flex-direction: column;

}
img{
    width: 100%;
    object-fit: cover;
    aspect-ratio: 16/9;
    border-radius: 30px;
}
h1{
    font-size: 30px;
    margin: 10px 0;
}
p{
    font-size: 15px;
    margin-bottom: 10px;
    display: block;
}
nav{
    display: flex;
    font-size: 17px;
    margin-bottom: 10px;
    
}
i{
    margin-right: 10px;
}
button{
    background-color: #B0D8DC;
    border-radius: 30px;
    font-size: 20px;
    padding: 10px 10px;
    margin-left: auto;
    transition: all 0.5s;
}
button:hover{
    background-color:aqua;
    transform: scale(1.1);
}
</style>
