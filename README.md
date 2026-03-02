<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chapter 1: Ten Principles of Economics</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script defer src="https://cdn.jsdelivr.net/npm/alpinejs@3.x.x/dist/cdn.min.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap');
        body { font-family: 'Inter', sans-serif; }
        .prose h2 { color: #4f46e5; margin-top: 2rem; border-bottom: 2px solid #f3f4f6; padding-bottom: 0.5rem; }
        .principle-card { transition: transform 0.2s; }
        .principle-card:hover { transform: translateY(-4px); }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 leading-relaxed">

    <nav class="sticky top-0 bg-white/90 backdrop-blur-sm border-b border-slate-200 z-50 p-4">
        <div class="max-w-4xl mx-auto flex justify-between items-center">
            <span class="font-extrabold text-indigo-600 tracking-tight">ECONOMICS 101</span>
            <div class="hidden md:flex space-x-6 text-sm font-semibold text-slate-500">
                <a href="#decisions" class="hover:text-indigo-600">Decision Making</a>
                <a href="#interaction" class="hover:text-indigo-600">Interaction</a>
                <a href="#economy" class="hover:text-indigo-600">Economy-Wide</a>
            </div>
        </div>
    </nav>

    <main class="max-w-4xl mx-auto py-12 px-6">
        
        <header class="mb-16">
            <p class="text-indigo-600 font-bold tracking-widest uppercase text-sm mb-2">Mankiw: Ninth Edition</p>
            <h1 class="text-5xl font-extrabold text-slate-900 mb-6 tracking-tight">Chapter 1: Ten Principles of Economics</h1>
            <div class="bg-indigo-600 text-white p-6 rounded-2xl shadow-lg">
                <p class="text-lg italic opacity-90">"Economy" comes from the Greek word <strong>oikonomos</strong>: "One who manages a household."</p>
            </div>
        </header>

        <section class="prose prose-slate max-w-none mb-16">
            <p class="text-xl text-slate-600">
                Society faces many decisions regarding the allocation of <strong>scarce resources</strong>[cite: 11, 13, 17]. 
                Because resources are limited, society cannot produce everything people desire[cite: 18, 19]. 
                Economics is the study of how society manages these resources[cite: 20, 21].
            </p>
        </section>

        <h2 id="decisions" class="text-3xl font-bold mb-8 text-slate-900">I. How People Make Decisions</h2>
        <div class="grid gap-6 mb-16">
            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 1</span>
                <h3 class="text-xl font-bold mb-2">People Face Trade-offs</h3>
                <p class="text-slate-600">"There ain't no such thing as a free lunch." To get something we like, we give up something else[cite: 53, 54, 55].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 2</span>
                <h3 class="text-xl font-bold mb-2">The Cost of Something is What You Give Up to Get It</h3>
                <p class="text-slate-600">Decision-makers must consider <strong>Opportunity Cost</strong>: whatever must be given up to obtain an item[cite: 86, 90, 91].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 3</span>
                <h3 class="text-xl font-bold mb-2">Rational People Think at the Margin</h3>
                <p class="text-slate-600">Rational people make decisions by comparing <strong>marginal benefits</strong> and <strong>marginal costs</strong>[cite: 94, 103].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 4</span>
                <h3 class="text-xl font-bold mb-2">People Respond to Incentives</h3>
                <p class="text-slate-600">An incentive is something that induces a person to act, such as a change in price[cite: 117, 118, 120].</p>
            </div>
        </div>

        <h2 id="interaction" class="text-3xl font-bold mb-8 text-slate-900">II. How People Interact</h2>
        <div class="grid gap-6 mb-16">
            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 5</span>
                <h3 class="text-xl font-bold mb-2">Trade Can Make Everyone Better Off</h3>
                <p class="text-slate-600">Trade allows people to specialize in what they do best and enjoy a greater variety of goods[cite: 136, 138, 139].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 6</span>
                <h3 class="text-xl font-bold mb-2">Markets are Usually a Good Way to Organize Economic Activity</h3>
                <p class="text-slate-600">Market economies use decentralized decisions of firms and households, guided by an <strong>"invisible hand"</strong>[cite: 143, 151, 162].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 7</span>
                <h3 class="text-xl font-bold mb-2">Governments Can Sometimes Improve Market Outcomes</h3>
                <p class="text-slate-600">Government is needed to enforce property rights and address <strong>market failures</strong> like externalities or market power[cite: 195, 198, 205].</p>
            </div>
        </div>

        <h2 id="economy" class="text-3xl font-bold mb-8 text-slate-900">III. How the Economy as a Whole Works</h2>
        <div class="grid gap-6 mb-16">
            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 8</span>
                <h3 class="text-xl font-bold mb-2">Standard of Living Depends on Ability to Produce Goods</h3>
                <p class="text-slate-600">Differences in living standards are explained by <strong>productivity</strong>: the amount of goods produced per unit of labor[cite: 227, 234, 235].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 9</span>
                <h3 class="text-xl font-bold mb-2">Prices Rise When the Government Prints Too Much Money</h3>
                <p class="text-slate-600"><strong>Inflation</strong> is caused by growth in the quantity of money, which causes the value of money to fall[cite: 243, 244, 248, 249].</p>
            </div>

            <div class="principle-card bg-white p-6 rounded-xl border border-slate-200 shadow-sm">
                <span class="text-indigo-500 font-bold text-sm uppercase">Principle 10</span>
                <h3 class="text-xl font-bold mb-2">Society Faces a Short-run Trade-off Between Inflation and Unemployment</h3>
                <p class="text-slate-600">Reducing inflation often causes a temporary rise in unemployment—a key part of the <strong>business cycle</strong>[cite: 253, 260, 263].</p>
            </div>
        </div>

    </main>

    <footer class="bg-slate-900 text-slate-400 py-12 px-6 text-center">
        <p class="text-sm">Course Materials: Principles of Economics [cite: 2]</p>
        <p class="text-xs mt-2 italic">Built for interactive learning via GitHub Pages</p>
    </footer>

</body>
</html>
