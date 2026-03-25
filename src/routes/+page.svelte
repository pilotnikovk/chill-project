<script>
  import SEO from '$lib/components/SEO.svelte';
  import Process from '$lib/components/Process.svelte';
  let isMenuOpen = false;
  const toggleMenu = () => isMenuOpen = !isMenuOpen;
</script>

<SEO />

<header class="fixed top-0 w-full z-50 bg-white/10 backdrop-blur-md border-b border-white/20">
  <nav class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
    <div class="text-3xl font-black text-white tracking-tighter uppercase italic">Chill</div>
    
    <div class="hidden md:flex space-x-8 text-white/80 font-medium">
      <a href="#hero" class="hover:text-cyan-400 transition">Главная</a>
      <a href="#services" class="hover:text-cyan-400 transition">Сервисы</a>
      <a href="#process" class="hover:text-cyan-400 transition">Процесс</a>
      <a href="#about" class="hover:text-cyan-400 transition">О нас</a>
      <a href="#contact" class="px-6 py-2 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-full text-white hover:shadow-lg hover:scale-105 transition active:scale-95">Заказать</a>
    </div>

    <button on:click={toggleMenu} class="md:hidden text-white">
      <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m4 6h16"></path></svg>
    </button>
  </nav>
</header>

<main class="min-h-screen bg-[#050505] text-white">
  <!-- HERO SECTION -->
  <section id="hero" class="relative pt-32 pb-20 px-6 flex flex-col items-center text-center overflow-hidden">
    <!-- Глоу эффект на фоне -->
    <div class="absolute -top-40 -left-40 w-96 h-96 bg-cyan-500/20 blur-[120px] rounded-full"></div>
    <div class="absolute top-1/2 -right-40 w-80 h-80 bg-purple-500/20 blur-[120px] rounded-full"></div>

    <h1 class="text-6xl md:text-8xl font-black mb-6 tracking-tighter bg-clip-text text-transparent bg-gradient-to-b from-white to-white/40 leading-tight">
      ПРОСТОТА <br/> В КАЖДОМ ПИКСЕЛЕ
    </h1>
    <p class="max-w-2xl text-xl text-white/60 mb-10 leading-relaxed">
      Создаем интерфейсы, которые дышат. Профессиональная разработка с акцентом на UX, скорость и чистоту кода.
    </p>
    
    <div class="flex flex-col md:flex-row gap-4">
      <button class="px-10 py-5 bg-white text-black font-bold rounded-2xl hover:bg-cyan-400 transition shadow-[0_0_50px_-10px_rgba(255,255,255,0.3)]">Смотреть проекты</button>
      <button class="px-10 py-5 border border-white/20 rounded-2xl font-bold hover:bg-white/5 transition backdrop-blur-sm italic">Наш манифест</button>
    </div>
  </section>

  <!-- SERVICES / FEATURES -->
  <section id="services" class="py-24 max-w-7xl mx-auto px-6 grid md:grid-cols-3 gap-8">
    <div class="p-8 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-sm group hover:border-cyan-500/50 transition">
      <div class="w-12 h-12 bg-cyan-500/20 rounded-xl mb-6 flex items-center justify-center text-cyan-400">⚡</div>
      <h3 class="text-2xl font-bold mb-4">Fastest Core</h3>
      <p class="text-white/40 leading-relaxed">SvelteKit и оптимизированные ассеты обеспечивают загрузку сайта менее чем за 1 секунду.</p>
    </div>
    <div class="p-8 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-sm group hover:border-purple-500/50 transition">
      <div class="w-12 h-12 bg-purple-500/20 rounded-xl mb-6 flex items-center justify-center text-purple-400">📱</div>
      <h3 class="text-2xl font-bold mb-4">Adaptive Flow</h3>
      <p class="text-white/40 leading-relaxed">Дизайн, который идеально ложится на экран любого устройства от часов до 4К монитора.</p>
    </div>
    <div class="p-8 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-sm group hover:border-orange-500/50 transition">
      <div class="w-12 h-12 bg-orange-500/20 rounded-xl mb-6 flex items-center justify-center text-orange-400">📈</div>
      <h3 class="text-2xl font-bold mb-4">SEO Master</h3>
      <p class="text-white/40 leading-relaxed">Чистая семантика HTML5 и правильные мета-данные выведут вас в топ выдачи.</p>
    </div>
  </section>

  <!-- PROCESS SECTION -->
  <Process />
</main>

<style>
  :global(html) {
    scroll-behavior: smooth;
  }
</style>
