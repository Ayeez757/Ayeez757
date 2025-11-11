## Hi there 👋

<!--
**Ayeez757/Ayeez757** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<script>
  

@keyframes slide {
    0% {
        transform: translateX(-50%);
    }
    100% {
        transform: translateX(0);
    }
}
@keyframes slide2 {
            0% {
                transform: translateX(0);
            }
            100% {
                transform: translateX(-50%);
            }
        }
.tech-icon {
    width: 6.9vw; /* 原 50px */
    height: 6.9vw; /* 原 50px */
    border-radius: 1.4vw; /* 原 10px */
    background: rgba(255, 255, 255, 0.7);
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 0.28vw 0.7vw rgba(0, 0, 0, 0.1); /* 相对单位 */
    transition: transform 0.3s ease;
    flex-shrink: 0;
}
.tech-icon:hover {
    transform: scale(1.1);
}
.tech-icon img {
    width: 4.2vw; /* 原 30px */
    height: 4.2vw; /* 原 30px */
    margin: 0px;
    object-fit: contain;
}

@media (max-width: 768px) { 
    .tech-icon {
        margin: 0.5vw;
        height: 11vw;
        width: 11vw;
    }
    .tech-icon img {
        width: 7vw;
        height: 7vw;
    }
}

#about-avatar {
    position: relative;
    margin-left: 0;
    margin-right: auto;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    border: 3px solid white;
    margin-bottom: 1.5rem;
    animation:
        rollAcrossScreen 2s ease,
        rotate 2s ease;
}

@keyframes rollAcrossScreen {
    from {
        right: -700%;
    }
    to {
        right: 0;
    }
}

/* 自身旋转动画 */
@keyframes rotate {
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(-720deg);
    }
}

.about-section {
    display: flex;
    align-items: center;
    gap: 20px;
}

.tags-container {
    display: flex;
    flex-direction: row; /* 改为行布局 */
    flex-wrap: wrap; /* 允许换行 */
    gap: 10px;
    max-width: 500px; /* 限制最大宽度防止溢出 */
}
.about-tag {
    background: linear-gradient(45deg, rgba(109,208,242,0.75), rgba(245,154,190,0.75));
    color: white;
    padding: 6px 12px;
    border-radius: 20px;
    font-weight: bold;
    opacity: 0;
    transform: translateX(-20px);
    text-shadow: 0 1px 2px rgba(0,0,0,0.3); /* 添加文字阴影增强可读性 */
    box-shadow: 0 2px 4px rgba(0,0,0,0.1); /* 添加轻微阴影 */
}


/* 为每个标签设置不同的延迟 */
.about-tag:nth-child(1) {
    animation: fadeInRight 0.6s 2s forwards;
}

.about-tag:nth-child(2) {
    animation: fadeInRight 0.6s 2.3s forwards;
}

.about-tag:nth-child(3) {
    animation: fadeInRight 0.6s 2.6s forwards;
}

.about-tag:nth-child(4) {
    animation: fadeInRight 0.6s 2.9s forwards;
}

.about-tag:nth-child(5) {
    animation: fadeInRight 0.6s 3.2s forwards;
}
.about-tag:nth-child(6) {
    animation: fadeInRight 0.6s 3.5s forwards;
}
.about-tag:nth-child(7) {
    animation: fadeInRight 0.6s 3.8s forwards;
}
.about-tag:nth-child(8) {
    animation: fadeInRight 0.6s 4.1s forwards;
}

@keyframes fadeInRight {
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

/* 移动端适配 */
@media screen and (max-width: 768px) {
    .about-section {
        flex-direction: column;
        align-items: center;
        gap: 15px;
    }
    
    .tags-container {
        justify-content: center;
        flex-wrap: wrap;
    }
    
    /* 移动端标签动画调整 */
    .about-tag {
        transform: translateY(20px);
    }
    
    .about-tag:nth-child(1) {
        animation: fadeInUp 0.6s 2s forwards;
    }
    
    .about-tag:nth-child(2) {
        animation: fadeInUp 0.6s 2.3s forwards;
    }
    
    .about-tag:nth-child(3) {
        animation: fadeInUp 0.6s 2.6s forwards;
    }
    .about-tag:nth-child(4) {
        animation: fadeInUp 0.6s 2.9s forwards;
    }
    .about-tag:nth-child(5) {
        animation: fadeInUp 0.6s 3.2s forwards;
    }
    .about-tag:nth-child(6) {
        animation: fadeInUp 0.6s 3.5s forwards;
    }
    .about-tag:nth-child(7) {
        animation: fadeInUp 0.6s 3.8s forwards;
    }
    .about-tag:nth-child(8) {
        animation: fadeInUp 0.6s 4.1s forwards;
    }
    
    @keyframes fadeInUp {
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }
}

/* 手写风格标题 - 逐字出现动画 */
.name-section {
    text-align: start;
    margin: 30px 0;
    padding: 20px;
}

.handwriting-title {
    font-family: 'Segoe Script', 'Lucida Handwriting', 'Comic Sans MS', cursive, sans-serif;
    font-size: 3rem;
    font-weight: normal;
    color: #000;
    margin: 0;
    line-height: 0;
    min-height: 0;
}



/* 逐字动画容器 */
.char-container {
    display: inline-block;
    opacity: 0;
    transform: translateY(20px);
}

/* 为每个字符设置不同的动画延迟 */
.char-container:nth-child(1) { animation: charFadeIn 0.5s forwards; animation-delay: 0.2s; }
.char-container:nth-child(2) { animation: charFadeIn 0.5s forwards; animation-delay: 0.4s; }
.char-container:nth-child(3) { animation: charFadeIn 0.5s forwards; animation-delay: 0.6s; }
.char-container:nth-child(4) { animation: charFadeIn 0.5s forwards; animation-delay: 0.8s; }
.char-container:nth-child(5) { animation: charFadeIn 0.5s forwards; animation-delay: 1.0s; }
.char-container:nth-child(6) { animation: charFadeIn 0.5s forwards; animation-delay: 1.2s; }
.char-container:nth-child(7) { animation: charFadeIn 0.5s forwards; animation-delay: 1.4s; }
.char-container:nth-child(8) { animation: charFadeIn 0.5s forwards; animation-delay: 1.6s; }
.char-container:nth-child(9) { animation: charFadeIn 0.5s forwards; animation-delay: 1.8s; }
.char-container:nth-child(10) { animation: charFadeIn 0.5s forwards; animation-delay: 2.0s; }
.char-container:nth-child(11) { animation: charFadeIn 0.5s forwards; animation-delay: 2.2s; }
.char-container:nth-child(12) { animation: charFadeIn 0.5s forwards; animation-delay: 2.4s; }
.char-container:nth-child(13) { animation: charFadeIn 0.5s forwards; animation-delay: 2.6s; }
.char-container:nth-child(14) { animation: charFadeIn 0.5s forwards; animation-delay: 2.8s; }
.char-container:nth-child(15) { animation: charFadeIn 0.5s forwards; animation-delay: 3.0s; }
.char-container:nth-child(16) { animation: charFadeIn 0.5s forwards; animation-delay: 3.2s; }
.char-container:nth-child(17) { animation: charFadeIn 0.5s forwards; animation-delay: 3.4s; }
.char-container:nth-child(18) { animation: charFadeIn 0.5s forwards; animation-delay: 3.6s; }
.char-container:nth-child(19) { animation: charFadeIn 0.5s forwards; animation-delay: 3.8s; }



@keyframes charFadeIn {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* 移动端适配 */
@media screen and (max-width: 768px) {
    .handwriting-title {
        font-size: 2.8rem;
        padding: 15px;
    }
}

@media screen and (max-width: 480px) {
    .handwriting-title {
        font-size: 2.3rem;
        padding: 10px;
    }
    
    .char-container:nth-child(1) { animation-delay: 0.1s; }
    .char-container:nth-child(2) { animation-delay: 0.2s; }
    .char-container:nth-child(3) { animation-delay: 0.3s; }
    .char-container:nth-child(4) { animation-delay: 0.4s; }
    .char-container:nth-child(5) { animation-delay: 0.5s; }
    .char-container:nth-child(6) { animation-delay: 0.6s; }
    .char-container:nth-child(7) { animation-delay: 0.7s; }
    .char-container:nth-child(8) { animation-delay: 0.8s; }
    .char-container:nth-child(9) { animation-delay: 0.9s; }
}

/* 副标题样式 */
.subtitle {
    font-family: 'Segoe Script', 'Lucida Handwriting', 'Comic Sans MS', cursive, sans-serif;
    font-size: 2rem;
    font-weight: normal;
    color: #333;
    margin: 25px 0 0 0;
    line-height: 1.2;
    min-height: 50px;
}

/* 副标题字符样式 */
.subtitle-char {
    font-size: 1.5rem;
    color: #333;
}

/* 副标题字符动画延迟 */
.subtitle .subtitle-char:nth-child(1) { animation-delay: 1.0s; }
.subtitle .subtitle-char:nth-child(2) { animation-delay: 1.2s; }
.subtitle .subtitle-char:nth-child(3) { animation-delay: 1.4s; }
.subtitle .subtitle-char:nth-child(4) { animation-delay: 1.6s; }
.subtitle .subtitle-char:nth-child(5) { animation-delay: 1.8s; }
.subtitle .subtitle-char:nth-child(6) { animation-delay: 2.0s; }
.subtitle .subtitle-char:nth-child(7) { animation-delay: 2.2s; }
.subtitle .subtitle-char:nth-child(8) { animation-delay: 2.4s; }
.subtitle .subtitle-char:nth-child(9) { animation-delay: 2.6s; }
.subtitle .subtitle-char:nth-child(10) { animation-delay: 2.8s; }
.subtitle .subtitle-char:nth-child(11) { animation-delay: 3.0s; }
.subtitle .subtitle-char:nth-child(12) { animation-delay: 3.2s; }
.subtitle .subtitle-char:nth-child(13) { animation-delay: 3.4s; }
.subtitle .subtitle-char:nth-child(14) { animation-delay: 3.6s; }
.subtitle .subtitle-char:nth-child(15) { animation-delay: 3.8s; }
.subtitle .subtitle-char:nth-child(16) { animation-delay: 4.0s; }
.subtitle .subtitle-char:nth-child(17) { animation-delay: 4.2s; }
.subtitle .subtitle-char:nth-child(18) { animation-delay: 4.4s; }
.subtitle .subtitle-char:nth-child(19) { animation-delay: 4.6s; }    


/* 移动端适配 */
@media screen and (max-width: 768px) {
    .handwriting-title {
        font-size: 2.8rem;
        padding: 15px;
    }
    
    .subtitle {
        font-size: 1.5rem;
    }
    
    .subtitle-char {
        font-size: 1.5rem;
    }
    
    .subtitle .subtitle-char:nth-child(1) { animation-delay: 0.9s; }
    .subtitle .subtitle-char:nth-child(2) { animation-delay: 1.0s; }
    .subtitle .subtitle-char:nth-child(3) { animation-delay: 1.1s; }
    .subtitle .subtitle-char:nth-child(4) { animation-delay: 1.2s; }
    .subtitle .subtitle-char:nth-child(5) { animation-delay: 1.3s; }
    .subtitle .subtitle-char:nth-child(6) { animation-delay: 1.4s; }
    .subtitle .subtitle-char:nth-child(7) { animation-delay: 1.5s; }
    .subtitle .subtitle-char:nth-child(8) { animation-delay: 1.6s; }
    .subtitle .subtitle-char:nth-child(9) { animation-delay: 1.7s; }
    .subtitle .subtitle-char:nth-child(10) { animation-delay: 1.8s; }
    .subtitle .subtitle-char:nth-child(11) { animation-delay: 1.9s; }
    .subtitle .subtitle-char:nth-child(12) { animation-delay: 2.0s; }
    .subtitle .subtitle-char:nth-child(13) { animation-delay: 2.1s; }
    .subtitle .subtitle-char:nth-child(14) { animation-delay: 2.2s; }
    .subtitle .subtitle-char:nth-child(15) { animation-delay: 2.3s; }
    .subtitle .subtitle-char:nth-child(16) { animation-delay: 2.4s; }
    .subtitle .subtitle-char:nth-child(17) { animation-delay: 2.5s; }
    .subtitle .subtitle-char:nth-child(18) { animation-delay: 2.6s; }
    .subtitle .subtitle-char:nth-child(19) { animation-delay: 2.7s; }

}

@media screen and (max-width: 480px) {
    .handwriting-title {
        font-size: 2.3rem;
        padding: 10px;
    }
    
    .subtitle {
        font-size: 1.3rem;
    }
    
    .subtitle-char {
        font-size: 1.3rem;
    }
    
    .subtitle .subtitle-char:nth-child(1) { animation-delay: 0.8s; }
    .subtitle .subtitle-char:nth-child(2) { animation-delay: 0.9s; }
    .subtitle .subtitle-char:nth-child(3) { animation-delay: 1.0s; }
    .subtitle .subtitle-char:nth-child(4) { animation-delay: 1.1s; }
    .subtitle .subtitle-char:nth-child(5) { animation-delay: 1.2s; }
    .subtitle .subtitle-char:nth-child(6) { animation-delay: 1.3s; }
    .subtitle .subtitle-char:nth-child(7) { animation-delay: 1.4s; }
    .subtitle .subtitle-char:nth-child(8) { animation-delay: 1.5s; }
    .subtitle .subtitle-char:nth-child(9) { animation-delay: 1.6s; }
    .subtitle .subtitle-char:nth-child(10) { animation-delay: 1.7s; }
    .subtitle .subtitle-char:nth-child(11) { animation-delay: 1.8s; }
    .subtitle .subtitle-char:nth-child(12) { animation-delay: 1.9s; }
    .subtitle .subtitle-char:nth-child(13) { animation-delay: 2.0s; }
    .subtitle .subtitle-char:nth-child(14) { animation-delay: 2.1s; }
    .subtitle .subtitle-char:nth-child(15) { animation-delay: 2.2s; }
    .subtitle .subtitle-char:nth-child(16) { animation-delay: 2.3s; }
    .subtitle .subtitle-char:nth-child(17) { animation-delay: 2.4s; }
    .subtitle .subtitle-char:nth-child(18) { animation-delay: 2.5s; }
    .subtitle .subtitle-char:nth-child(19) { animation-delay: 2.6s; }

}

.box-father{
    margin-top: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 50vh;
    background-color: #efefef6c;
    border-radius: 10px;
    overflow: hidden;
}

.box{
    position: relative;
    display: flex;
}
.box .box-item{
    position: absolute;
    top:calc(50% - 150px);
    left:calc(50% - 100px);
    background-color: transparent;
    width:200px;
    height: fit-content;
    transition: 0.25s;
    box-shadow: 0 0 50px rgba(0, 0, 0, 0.5);
    user-select: none;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 5em;
    font-family: consolas;
    font-weight: 800;
    opacity: 0;
}
/* 为图片添加样式以消除白边 */
.box .box-item img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* 保持图片比例并填充容器 */
    display: block; /* 消除图片下方的空白 */
    border-radius: inherit;
}

.box .box-item:nth-child(1){
    transform: translate3d(-250px,0,0)  scale(0.8);
    opacity: 1;
    z-index: 1;
    background-color: #d8d8d800;
}
.box .box-item:nth-child(2){
    transform: translate3d(-250px,0,0)  scale(0.8);
    opacity: 1;
    z-index: 2;
    background-color: #d8d8d800;
}
.box .box-item:nth-child(3){
    transform: translate3d(-150px,0,0)  scale(0.9);
    opacity: 1;
    z-index: 3;
    background-color: #d8d8d800;
    font-size: 6em;
}
.box .box-item:nth-child(4){
    transform: translate3d(0px,0,0)  scale(1);
    opacity: 1;
    z-index: 4;
    background-color: #d8d8d800;
    font-size: 8em;
}
.box .box-item:nth-child(5){
    transform: translate3d(150px,0,0)  scale(0.9);
    opacity: 1;
    z-index: 3;
    background-color:   #d8d8d800;
    font-size: 6em;
}
.box .box-item:nth-child(6){
    transform: translate3d(250px,0,0)  scale(0.8);
    opacity: 1;
    z-index: 2;
    background-color:   #d8d8d800;
}
.box .box-item:nth-child(7){
    transform: translate3d(250px,0,0)  scale(0.8);
    opacity: 1;
    z-index: 1;
    background-color: #d8d8d800;
}


</script>

<div class="custom-html">
    <div class="about-section">
        <img src="https://blog.ayeez.cn/imgs/photo.jpg" alt="头像" id="about-avatar">
        <div class="tags-container">
            <span class="about-tag">#大一软件工程学生</span>
            <span class="about-tag">#热衷于全栈开发</span>
            <span class="about-tag">#高级cv工程师</span>
            <span class="about-tag">#喜欢瞎折腾的傻子</span>
            <span class="about-tag">#喜欢体验各种事物</span>
            <span class="about-tag">#励志成为全栈大佬</span>
            <span class="about-tag">#画画、钢琴、运动、技术控</span>
            <span class="about-tag">#Minecraft</span>
        </div>
    </div>
</div>

<!-- 逐字出现的标题 -->
<div class="name-section">
    <h1 class="handwriting-title" id="animatedTitle"></h1>
    <h2 class="subtitle" id="animatedSubtitle"></h2>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
    // 随机颜色生成函数
    function getRandomColor() {
        const colors = [
            // 柔和的红色系
            'linear-gradient(135deg, #B05F6D, #D18A94)',      // 柔和玫瑰红
            'linear-gradient(135deg, #B86D6D, #D19A9A)',      // 柔和砖红
            'linear-gradient(135deg, #A66363, #C48C8C)',      // 柔和红棕
            
            // 柔和的紫色系
            'linear-gradient(135deg, #8A6E9C, #A88EB8)',      // 柔和紫罗兰
            'linear-gradient(135deg, #947AA3, #B29AC4)',      // 柔和薰衣草
            'linear-gradient(135deg, #7D7094, #9B8EBA)',      // 柔和灰紫
            
            // 柔和的蓝色系
            'linear-gradient(135deg, #6B8CAD, #8AA9C9)',      // 柔和天蓝
            'linear-gradient(135deg, #7193A6, #91B3C9)',      // 柔和海蓝
            'linear-gradient(135deg, #69859C, #87A3BD)',      // 柔和钢蓝
            
            // 柔和的绿色系
            'linear-gradient(135deg, #7DA48C, #9DC2AA)',      // 柔和薄荷绿
            'linear-gradient(135deg, #86A486, #A4C2A4)',      // 柔和灰绿
            'linear-gradient(135deg, #8FA68A, #ADC4A7)',      // 柔和橄榄绿
            
            // 柔和的橙黄色系
            'linear-gradient(135deg, #C49B71, #D9B995)',      // 柔和桃色
            'linear-gradient(135deg, #B8A27D, #D1C09D)',      // 柔和米黄
            'linear-gradient(135deg, #BFA07A, #D9C2A0)',      // 柔和卡其
            
            // 柔和的粉色系
            'linear-gradient(135deg, #B48A9D, #D1A8BA)',      // 柔和樱花粉
            'linear-gradient(135deg, #A88C9C, #C6AAB9)',      // 柔和灰粉
            'linear-gradient(135deg, #B095A8, #CDB3C5)',      // 柔和丁香紫
            
            // 柔和的青色系
            'linear-gradient(135deg, #7DA7A7, #9DC2C2)',      // 柔和水蓝
            'linear-gradient(135deg, #859D9D, #A3BDBD)',      // 柔和灰蓝
            'linear-gradient(135deg, #7D9C9C, #9BB9B9)',      // 柔和石蓝
            
            // 柔和的中性色系
            'linear-gradient(135deg, #8A9494, #A8B2B2)',      // 柔和灰蓝
            'linear-gradient(135deg, #9C948A, #BAB2A8)',      // 柔和灰棕
            'linear-gradient(135deg, #8A9C94, #A8BAAE)',      // 柔和灰绿
            'linear-gradient(135deg, #948A9C, #B2A8BA)',      // 柔和灰紫
            'linear-gradient(135deg, #9C9C8A, #BABAA8)'       // 柔和灰黄
        ];
        return colors[Math.floor(Math.random() * colors.length)];
    }
    
    // 为每个标签设置随机背景色
    const tags = document.querySelectorAll('.about-tag');
    tags.forEach(tag => {
        tag.style.background = getRandomColor();
        // 确保文字颜色对比度足够
        tag.style.color = '#FFFFFF';
        tag.style.textShadow = '0 1px 2px rgba(0,0,0,0.3)';
    });

 // 逐字显示标题
    const titleText = "我叫阿叶Ayeez";
    const titleElement = document.getElementById('animatedTitle');
    

    
    // 为每个字符创建容器
    for (let i = 0; i < titleText.length; i++) {
        const charContainer = document.createElement('span');
        charContainer.className = 'char-container';
        charContainer.textContent = titleText[i];
        titleElement.appendChild(charContainer);
    }

    // 逐字显示副标题
    const subtitleText = "很高兴认识你Hi~ o(*￣▽￣*)ブ";
    const subtitleElement = document.getElementById('animatedSubtitle');
    
    // 为每个字符创建容器（副标题）
    for (let i = 0; i < subtitleText.length; i++) {
        const charContainer = document.createElement('span');
        charContainer.className = 'char-container subtitle-char';
        charContainer.textContent = subtitleText[i];
        subtitleElement.appendChild(charContainer);
    }
});
</script>



> - 25级软件工程在读大学生(大一)
> - 热爱计算机(喜欢全栈)，记录自己的学习历程
> - 喜欢瞎折腾的小趴菜，有众多自己的业余爱好
> - 例如：画画，弹钢琴，做饭，乒乓球，中长跑，排球，我的世界（游戏），中式建筑，生电（我的世界），魔方，骑行，桌球，国际象棋，摄影，手工木作，股市赌狗，发射器玩具，喝茶，写博客等
> - 一些奇怪的技能：双手都能写字......
> - 技术栈: Java、html、css、javascript、vue、git
> - 涉及：c、c++、python
> - IP:广东

# 我的技术栈

<!-- 我的技术栈 -->
   <!-- 技术栈区域 -->
<div class="custom-html">
    <div class="tech-stack">
        <div class="tech-icons-container">
            <div class="tech-icons">
                <!-- 编程语言 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="Java">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++">
                </div>
                <!-- 开发工具 -->
                 <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="Vue">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" alt="IntelliJ IDEA">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="VS Code">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pycharm/pycharm-original.svg" alt="PyCharm">
                </div>
                <!-- 设计工具 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/photoshop/photoshop-plain.svg" alt="Photoshop">
                </div>
                <!-- 复制一份图标用于无缝循环 -->
                <!-- 编程语言 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="Java">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++">
                </div>
                <!-- 开发工具 -->
                 <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="Vue">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" alt="IntelliJ IDEA">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="VS Code">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pycharm/pycharm-original.svg" alt="PyCharm">
                </div>
                <!-- 设计工具 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/photoshop/photoshop-plain.svg" alt="Photoshop">
                </div>
            </div>
<div class="tech-icons2">
                <!-- 编程语言 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="Java">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++">
                </div>
                <!-- 开发工具 -->
                 <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="Vue">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" alt="IntelliJ IDEA">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="VS Code">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pycharm/pycharm-original.svg" alt="PyCharm">
                </div>
                <!-- 设计工具 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/photoshop/photoshop-plain.svg" alt="Photoshop">
                </div>
                <!-- 复制一份图标用于无缝循环 -->
                <!-- 编程语言 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" alt="Java">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++">
                </div>
                <!-- 开发工具 -->
                 <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="Vue">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" alt="IntelliJ IDEA">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="VS Code">
                </div>
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pycharm/pycharm-original.svg" alt="PyCharm">
                </div>
                <!-- 设计工具 -->
                <div class="tech-icon">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/photoshop/photoshop-plain.svg" alt="Photoshop">
                </div>
            </div>
        </div>
    </div>
</div>

# 追番列表

<!-- 轮播堆叠图片 -->
<div class="box-father">
    <div class="box"></div>
    <script>
        const boxFather = document.querySelector('.box-father');
        boxFather.addEventListener('wheel', function(event){
            event.preventDefault();
        },{ passive: false });
        let box = document.querySelector('.box');
        const images = [
            '../../imgs/anime/p3.png',
            '../../imgs/anime/p4.jpeg',
            '../../imgs/anime/p5.jpg',
            '../../imgs/anime/p6.jpg',
            '../../imgs/anime/p7.jpg',
            '../../imgs/anime/p8.jpg',
            '../../imgs/anime/p9.png',
            '../../imgs/anime/p10.jpg',
            '../../imgs/anime/p17.jpg',
            '../../imgs/anime/p18.jpg',
            '../../imgs/anime/p19.jpg',
            '../../imgs/anime/p1.jpg',
            '../../imgs/anime/p2.jpg',
            '../../imgs/anime/p11.jpeg',
            '../../imgs/anime/p12.jpg',
            '../../imgs/anime/p13.jpg',
            '../../imgs/anime/p14.jpg',
            '../../imgs/anime/p15.jpg',
            '../../imgs/anime/p16.jpg',
            '../../imgs/anime/p17.jpg',
            '../../imgs/anime/p18.jpg',
            '../../imgs/anime/p19.jpg',
            '../../imgs/anime/p20.jpg',
            '../../imgs/anime/p21.jpg',
            '../../imgs/anime/p22.jpg',
            '../../imgs/anime/p23.jpg',
            '../../imgs/anime/p24.jpg',
            '../../imgs/anime/p25.jpg',
            '../../imgs/anime/p26.jpg',
            '../../imgs/anime/p27.jpg',
            '../../imgs/anime/p28.jpg',
            '../../imgs/anime/p29.jpg',
            '../../imgs/anime/p30.jpg',
            '../../imgs/anime/p31.jpg',
            '../../imgs/anime/p32.jpg',
            '../../imgs/anime/p33.jpg',
        ];
        for (let i = 0; i < images.length; i++){
            let div = document.createElement('div');
            div.className = 'box-item';
            let img = document.createElement('img');
            img.src = images[i];
            img.alt = `图片 ${i+1}`;
            img.style.width = '100%';
            img.style.height = '100%';
            img.style.objectFit = 'cover';
            img.style.borderRadius = 'inherit';
            div.appendChild(img);
            box.appendChild(div);
        }   
        function moveNext(){
            let items = document.querySelectorAll('.box-item');
            box.appendChild(items[0]);
        }
        function movePrev(){ 
            let items = document.querySelectorAll('.box-item');
            box.prepend(items[items.length - 1]);
        }
        // PC端滚轮事件
        window.addEventListener('wheel', function(event){
            if(event.deltaY > 0){
                    moveNext();
                }else{
                    movePrev();
                }
            // 检查事件是否在轮播图区域内
            if (boxFather.contains(event.target)) {
                event.preventDefault();
            }
        }, { passive: false });
        // 移动端触摸滑动支持
        let touchStartX = 0;
        let touchStartY = 0;
        let isTouching = false;
        // 触摸开始
        boxFather.addEventListener('touchstart', function(event) {
            touchStartX = event.touches[0].clientX;
            touchStartY = event.touches[0].clientY;
            isTouching = true;
        }, { passive: true });
        // 触摸移动
        boxFather.addEventListener('touchmove', function(event) {
            if (!isTouching) return;
            const touchEndX = event.touches[0].clientX;
            const touchEndY = event.touches[0].clientY;
            const diffX = touchStartX - touchEndX;
            const diffY = touchStartY - touchEndY;
            // 如果主要是水平滑动，阻止默认行为（页面滚动）
            if (Math.abs(diffX) > Math.abs(diffY)) {
                event.preventDefault();
            }
        }, { passive: false });
        // 触摸结束
        boxFather.addEventListener('touchend', function(event) {
            if (!isTouching) return;
            const touchEndX = event.changedTouches[0].clientX;
            const touchEndY = event.changedTouches[0].clientY;
            const diffX = touchStartX - touchEndX;
            const diffY = touchStartY - touchEndY;
            // 判断是水平滑动还是垂直滑动
            if (Math.abs(diffX) > Math.abs(diffY) && Math.abs(diffX) > 50) {
                // 水平滑动距离足够才触发
                if (diffX > 0) {
                    // 向左滑动 - 下一张
                    moveNext();
                } else {
                    // 向右滑动 - 上一张
                    movePrev();
                }
            }
            // 重置状态
            isTouching = false;
        });
    </script>
</div>


# 我的装备
<div class="gallery-group-main">
{% galleryGroup thinkbook14+ 我的电脑 https://tk.lenovo.com.cn/product/1043468.html?key=ThinkBook&source=fromwww&isInstallment=true ../../imgs/equipment/thinkbook14+.png %}
{% galleryGroup 迈从Z75 我的键盘（已下架）  a ../../imgs/equipment/z75s.jpg %}
{% galleryGroup 红米K80ultra 我的手机（32G+1TB） https://www.mi.com/shop/buy/detail?product_id=21432&cfrom=search ../../imgs/equipment/redminK80Ultra.png %}
{% galleryGroup ipad 我的平板 https://www.apple.com.cn/shop/buy-ipad ../../imgs/equipment/ipadm411ench.png %}
{% galleryGroup ktch24t7 我的显示器 https://www.ktcplay.com/goods/detail/1960897853373149185 ../../imgs/equipment/ktcH24T7.png %}
{% galleryGroup 漫步者W820NB 我的耳机（战损版） https://www.edifier.com/cn/product/product-832.html ../../imgs/equipment/edifierW820NB.png %}

</div>









<!-- 硬币样式打赏按钮 -->
<div class="coin-reward">
  <div class="coin-wrapper" onclick="toggleCoinReward()">
    <div class="coin" id="reward-coin">
      <div class="coin-front">
        <i class="fas fa-yen-sign"></i>
      </div>
      <div class="coin-back">
        <i class="fas fa-qrcode"></i>
      </div>
    </div>
    <div class="coin-shadow"></div>
    <div class="coin-text">点击上方硬币请我喝杯咖啡？！来劲！码字！！！</div>
  </div>
  <div class="reward-main coin-reward-main" id="coin-reward-main" style="display:none;">
    <ul class="reward-all">
      <li class="reward-item">
        <a href="https://blog.ayeez.cn/imgs/infoOfMe/wechatReward.jpg" target="_blank">
          <img class="post-qr-code-img" src="https://blog.ayeez.cn/imgs/infoOfMe/wechatReward.jpg" alt="微信">
        </a>
        <div class="post-qr-code-desc">微信</div>
      </li>
      <li class="reward-item">
        <a href="https://blog.ayeez.cn/imgs/infoOfMe/alipayReward.jpg" target="_blank">
          <img class="post-qr-code-img" src="https://blog.ayeez.cn/imgs/infoOfMe/alipayReward.jpg" alt="支付宝">
        </a>
        <div class="post-qr-code-desc">支付宝</div>
      </li>
    </ul>
    <div class="reward-note">
      <i class="fas fa-info-circle"></i> 留下你的昵称或联系方式，我会在感谢名单里特别致谢哦！( •̀ ω •́ )✧<br>（如果你也有博客，可以留下你的域名，我将会在友链以及感谢名单里添加你的链接）
    </div>
  </div>
</div>

<style>
.coin-reward {
  margin: 50px 0;
  text-align: center;
}

.coin-wrapper {
  position: relative;
  display: inline-block;
  cursor: pointer;
  perspective: 1000px;
}

.coin {
  position: relative;
  width: 80px;
  height: 80px;
  margin: 0 auto 10px;
  transform-style: preserve-3d;
  transition: transform 0.5s ease-out;
}

.coin.flipped {
  animation: flip 1.2s ease-out;
}

@keyframes flip {
  0% {
    transform: rotateY(0) scale(1);
  }
  25% {
    transform: rotateY(180deg) scale(1.1);
  }
  50% {
    transform: rotateY(360deg) scale(1.2);
  }
  75% {
    transform: rotateY(540deg) scale(1.1);
  }
  100% {
    transform: rotateY(720deg) scale(1);
  }
}

.coin-front,
.coin-back {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  backface-visibility: hidden;
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.coin-front {
  background: radial-gradient(circle at 30% 30%, #FFD700, #D4AF37);
  border: 3px solid #B8860B;
  color: #8B4513;
  font-size: 28px;
}

.coin-back {
  background: radial-gradient(circle at 30% 30%, #4A90E2, #007AFF);
  border: 3px solid #1E3A8A;
  color: white;
  font-size: 24px;
  transform: rotateY(180deg);
}

.coin-shadow {
  width: 60px;
  height: 15px;
  background: rgba(0,0,0,0.1);
  border-radius: 50%;
  margin: 10px auto 0;
  filter: blur(3px);
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0%, 100% {
    transform: scale(1);
    opacity: 0.7;
  }
  50% {
    transform: scale(0.9);
    opacity: 0.4;
  }
}

.coin-text {
  color: #666;
  font-size: 16px;
  font-weight: 500;
  margin-top: 10px;
  transition: color 0.3s;
}

.coin-wrapper:hover .coin-text {
  color: #333;
}

.coin-wrapper:hover .coin {
  transform: translateY(-5px);
}

.coin-reward-main {
  margin-top: 30px;
  padding: 20px;
  background: rgba(255, 255, 255, 0.9);
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.reward-all {
  padding: 0;
  margin: 0;
  list-style: none;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.reward-item {
  margin: 15px;
  text-align: center;
}

.post-qr-code-img {
  width: 180px;
  height: 180px;
  max-width: 100%;
  border-radius: 10px;
  border: 3px solid #f0f0f0;
  transition: transform 0.3s ease;
}

.post-qr-code-img:hover {
  transform: scale(1.05);
}

.post-qr-code-desc {
  margin-top: 10px;
  font-size: 14px;
  color: #666;
  font-weight: 500;
}

.reward-note {
  margin-top: 20px;
  padding: 12px 20px;
  background: linear-gradient(135deg, #e3f2fd 0%, #bbdefb 100%);
  border-radius: 8px;
  color: #1976d2;
  font-size: 14px;
  font-weight: 500;
  display: inline-block;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
}

.reward-note i {
  margin-right: 8px;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .coin {
    width: 70px;
    height: 70px;
  }
  
  .coin-front,
  .coin-back {
    font-size: 22px;
  }
  
  .post-qr-code-img {
    width: 150px;
    height: 150px;
  }
}

@media (max-width: 480px) {
  .coin {
    width: 60px;
    height: 60px;
  }
  
  .coin-front,
  .coin-back {
    font-size: 18px;
  }
  
  .reward-all {
    flex-direction: column;
    align-items: center;
  }
  
  .post-qr-code-img {
    width: 130px;
    height: 130px;
  }
  
  .reward-note {
    font-size: 13px;
    padding: 10px 15px;
  }
}
</style>

<script>
function toggleCoinReward() {
  const coin = document.getElementById('reward-coin');
  const rewardMain = document.getElementById('coin-reward-main');
  // 添加翻转动画类
  coin.classList.add('flipped');
  // 切换二维码显示
  if (rewardMain) {
    // 等待动画结束后切换显示状态
    setTimeout(() => {
      if (rewardMain.style.display === 'block') {
        rewardMain.style.display = 'none';
      } else {
        rewardMain.style.display = 'block';
      }
    }, 600);
  }
  // 动画结束后移除类，以便下次可以再次播放
  setTimeout(() => {
    coin.classList.remove('flipped');
  }, 1200);
}
</script>

<!-- 打赏感谢名单 -->
<div class="reward-thanks-section">
  <h3 class="thanks-title">
    <i class="fas fa-heart"></i> 衷心感谢以下小伙伴的支持！
  </h3>
  <div class="thanks-container" id="thanksContainer">
    <div class="thanks-list" id="thanksList">
      <!-- 感谢名单将通过JavaScript动态生成 -->
    </div>
    <div class="thanks-stats">
      <div class="stat-item">
        <span class="stat-number" id="totalSupporters">0</span>
        <span class="stat-label">支持者</span>
      </div>
      <div class="stat-item">
        <span class="stat-number" id="totalAmount">0</span>
        <span class="stat-label">总金额</span>
      </div>
    </div>
  </div>
</div>

<style>
.reward-thanks-section {
  margin: 60px 0 40px;
  padding: 30px;
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  border-radius: 15px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
}

.thanks-title {
  text-align: center;
  color: #495057;
  margin-bottom: 25px;
  font-size: 22px;
  font-weight: 600;
}

.thanks-title i {
  color: #e74c3c;
  margin-right: 10px;
}

.thanks-container {
  display: flex;
  flex-direction: column;
  gap: 25px;
  background-image: url('https://blog.ayeez.cn/imgs/bg/p4.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  padding: 30px;
  border-radius: 10px;
  position: relative;
}

.thanks-container::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(255, 255, 255, 0.85);
  border-radius: 10px;
  z-index: 1;
}

.thanks-container > * {
  position: relative;
  z-index: 2;
}

.thanks-list {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  justify-content: center;
}

.thanks-item {
  display: flex;
  align-items: center;
  padding: 12px 20px;
  border-radius: 50px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
  transition: all 0.3s ease;
  border: 1px solid #e9ecef;
  background-color: rgba(255, 255, 255, 0.95);
}

.thanks-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

.supporter-name {
  font-weight: 500;
  color: #495057;
  margin-right: 8px;
  text-decoration: none;
  transition: color 0.3s ease;
  cursor: pointer;
}

.supporter-name:hover {
  color: #e74c3c;
  text-decoration: underline;
}

.supporter-name.no-link {
  cursor: default;
  color: #6c757d;
}

.supporter-name.no-link:hover {
  color: #6c757d;
  text-decoration: none;
}

.supporter-amount {
  font-weight: 600;
  color: #e74c3c;
  background: rgba(231, 76, 60, 0.1);
  padding: 2px 8px;
  border-radius: 10px;
  font-size: 13px;
}

.thanks-stats {
  display: flex;
  justify-content: center;
  gap: 40px;
  margin-top: 10px;
}

.stat-item {
  text-align: center;
}

.stat-number {
  display: block;
  font-size: 28px;
  font-weight: 700;
  color: #e74c3c;
  line-height: 1;
}

.stat-label {
  font-size: 14px;
  color: #6c757d;
  margin-top: 5px;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .reward-thanks-section {
    padding: 20px;
  }
  
  .thanks-title {
    font-size: 20px;
  }
  
  .thanks-container {
    padding: 20px;
  }
  
  .thanks-stats {
    gap: 20px;
  }
  
  .stat-number {
    font-size: 24px;
  }
}

@media (max-width: 480px) {
  .thanks-item {
    padding: 10px 15px;
  }
  
  .thanks-stats {
    flex-direction: column;
    gap: 15px;
  }
}
</style>

<script>
// 打赏感谢名单数据
const supportersData = [
  { name: "小虾", amount: 9.99, noLink: true },
  { name: "祥仔", amount: 8.88, noLink: true },
  { name: "匿名支持者", amount: 0.01, noLink: true },
];

// 统计数据
const totalSupporters = supportersData.length;
const totalAmount = supportersData.reduce((sum, supporter) => sum + supporter.amount, 0);

// 渲染感谢名单
function renderSupporters() {
  const thanksList = document.getElementById('thanksList');
  const totalSupportersEl = document.getElementById('totalSupporters');
  const totalAmountEl = document.getElementById('totalAmount');
  
  // 渲染支持者列表
  thanksList.innerHTML = supportersData.map(supporter => {
    // 检查是否设置为无链接
    if (supporter.noLink) {
      return `
        <div class="thanks-item">
          <span class="supporter-name no-link">${supporter.name}</span>
          <span class="supporter-amount">¥${supporter.amount}</span>
        </div>
      `;
    } else {
      // 正常链接处理
      return `
        <div class="thanks-item">
          <a href="${supporter.link || '#'}" class="supporter-name" target="_blank">${supporter.name}</a>
          <span class="supporter-amount">¥${supporter.amount}</span>
        </div>
      `;
    }
  }).join('');
  
  // 更新统计数据
  totalSupportersEl.textContent = totalSupporters;
  totalAmountEl.textContent = totalAmount.toFixed(2);
}

// 页面加载完成后渲染
document.addEventListener('DOMContentLoaded', function() {
  renderSupporters();
});
</script>
