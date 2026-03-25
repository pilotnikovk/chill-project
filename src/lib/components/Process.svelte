<script>
  const steps = [
    { num: '01', title: 'Concept', text: 'Исследуем нишу, анализируем боли пользователей и создаем визуальный концепт.' },
    { num: '02', title: 'Blueprint', text: 'Проектируем интерактивный прототип, где каждая кнопка на своем месте.' },
    { num: '03', title: 'Forge', text: 'Превращаем дизайн в чистый код на SvelteKit с поддержкой всех экранов.' },
    { num: '04', title: 'Launch', text: 'Деплой в облако, SEO-оптимизация и полная поддержка после запуска.' }
  ];
</script>

<section id="process" class="py-24 max-w-7xl mx-auto px-6">
  <div class="mb-20">
    <h2 class="text-4xl md:text-6xl font-black mb-4 uppercase tracking-tighter">Наш процесс</h2>
    <div class="h-1 w-20 bg-cyan-500 rounded-full"></div>
  </div>

  <div class="grid md:grid-cols-4 gap-12">
    {#each steps as step}
      <div class="relative group">
        <span class="absolute -top-12 -left-6 text-7xl font-black text-white/5 group-hover:text-cyan-500/10 transition duration-700 select-none">
          {step.num}
        </span>
        <h4 class="text-2xl font-bold mb-4 flex items-center gap-3">
          <span class="w-1.5 h-6 bg-cyan-500 rounded-full"></span>
          {step.title}
        </h4>
        <p class="text-white/40 leading-relaxed font-medium">
          {step.text}
        </p>
      </div>
    {/each}
  </div>
</section>
