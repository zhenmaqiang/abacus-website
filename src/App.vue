<template>
  <div class="app">

    <router-view />
  
  </div>
</template>

<script>
export default {
  name: 'App',
  mounted() {
    // 平滑滚动
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          target.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
          });
        }
      });
    });

    // 导航栏滚动效果
    window.addEventListener('scroll', () => {
      const navbar = document.querySelector('.navbar');
      if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
      } else {
        navbar.classList.remove('scrolled');
      }
    });

    // FAQ 项目展开/折叠
    document.querySelectorAll('.faq-question').forEach(question => {
      question.addEventListener('click', function() {
        const answer = this.nextElementSibling;
        const isOpen = answer.style.display === 'block';
        
        // 关闭所有答案
        document.querySelectorAll('.faq-answer').forEach(a => {
          a.style.display = 'none';
        });
        
        // 打开当前答案
        if (!isOpen) {
          answer.style.display = 'block';
        }
      });
    });
  }
}
</script>
