<div class="flex h-screen bg-[#0a0a0a] text-white overflow-hidden font-sans">
  <!-- SIDEBAR -->
  <aside class="w-64 bg-black/40 border-r border-white/5 flex flex-col p-6 space-y-10">
    <div class="text-2xl font-black italic tracking-tighter uppercase">Admin</div>
    
    <nav class="flex-1 space-y-2">
      <a href="#" class="flex items-center space-x-4 p-4 rounded-xl bg-white/5 text-cyan-400 font-bold">
        <span>📊</span> <span>Dashboard</span>
      </a>
      <a href="#" class="flex items-center space-x-4 p-4 rounded-xl hover:bg-white/5 text-white/60 transition">
        <span>📝</span> <span>Posts</span>
      </a>
      <a href="#" class="flex items-center space-x-4 p-4 rounded-xl hover:bg-white/5 text-white/60 transition">
        <span>👥</span> <span>Users</span>
      </a>
      <a href="#" class="flex items-center space-x-4 p-4 rounded-xl hover:bg-white/5 text-white/60 transition">
        <span>⚙️</span> <span>Settings</span>
      </a>
    </nav>
    
    <button class="p-4 bg-red-500/10 text-red-400 font-bold rounded-xl border border-red-500/20 hover:bg-red-500/20 transition">Выйти</button>
  </aside>

  <!-- CONTENT AREA -->
  <main class="flex-1 overflow-y-auto p-10 bg-[radial-gradient(circle_at_top_right,_#1a1a1a,_#0a0a0a)]">
    <header class="flex justify-between items-center mb-12">
      <h1 class="text-4xl font-bold tracking-tight">Overview</h1>
      <div class="flex space-x-4">
        <button class="px-6 py-2 bg-white/5 border border-white/10 rounded-xl hover:bg-white/10 transition">Обновить</button>
        <button class="px-6 py-2 bg-cyan-500 text-black font-bold rounded-xl hover:shadow-[0_0_30px_-5px_rgba(6,182,212,0.5)] transition">Добавить</button>
      </div>
    </header>

    <!-- METRICS GRID -->
    <div class="grid md:grid-cols-4 gap-6 mb-12">
      <div class="p-6 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-md">
        <p class="text-white/40 mb-1 text-sm font-medium uppercase tracking-wider">Total Views</p>
        <p class="text-3xl font-black italic">142.5K</p>
        <p class="text-emerald-400 text-sm mt-2 font-bold">+12% vs last month</p>
      </div>
      <div class="p-6 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-md">
        <p class="text-white/40 mb-1 text-sm font-medium uppercase tracking-wider">Avg Session</p>
        <p class="text-3xl font-black italic">04:12</p>
        <p class="text-emerald-400 text-sm mt-2 font-bold">+30s this week</p>
      </div>
      <div class="p-6 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-md">
        <p class="text-white/40 mb-1 text-sm font-medium uppercase tracking-wider">Conversion</p>
        <p class="text-3xl font-black italic">3.82%</p>
        <p class="text-rose-400 text-sm mt-2 font-bold">-0.5% today</p>
      </div>
      <div class="p-6 bg-white/5 border border-white/10 rounded-3xl backdrop-blur-md">
        <p class="text-white/40 mb-1 text-sm font-medium uppercase tracking-wider">Revenue</p>
        <p class="text-3xl font-black italic">$12,401</p>
        <p class="text-emerald-400 text-sm mt-2 font-bold">All time high</p>
      </div>
    </div>

    <!-- MAIN CHART AREA -->
    <div class="p-8 bg-white/5 border border-white/10 rounded-3xl h-[400px] flex items-center justify-center relative overflow-hidden">
      <div class="absolute inset-0 bg-gradient-to-t from-cyan-500/5 to-transparent"></div>
      <p class="text-white/20 font-black text-4xl italic tracking-tighter uppercase opacity-50 select-none">Project Analytics Flow</p>
      <!-- CHART UI MOCK -->
      <div class="absolute bottom-20 left-10 right-10 h-32 flex items-end space-x-2">
        <div class="flex-1 bg-white/10 h-10 rounded-t-lg transition hover:bg-cyan-500/50"></div>
        <div class="flex-1 bg-white/10 h-20 rounded-t-lg transition hover:bg-cyan-500/50"></div>
        <div class="flex-1 bg-white/10 h-14 rounded-t-lg transition hover:bg-cyan-500/50"></div>
        <div class="flex-1 bg-cyan-500 h-28 rounded-t-lg"></div>
        <div class="flex-1 bg-white/10 h-18 rounded-t-lg transition hover:bg-cyan-500/50"></div>
        <div class="flex-1 bg-white/10 h-24 rounded-t-lg transition hover:bg-cyan-500/50"></div>
        <div class="flex-1 bg-white/10 h-16 rounded-t-lg transition hover:bg-cyan-500/50"></div>
      </div>
    </div>
  </main>
</div>
