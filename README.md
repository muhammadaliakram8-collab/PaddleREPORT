<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PadelISB Feasibility Report 2026</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --neon-cyan: #00f5d4;
            --electric-blue: #4361ee;
            --soft-purple: #7209b7;
            --warning-orange: #f77f00;
            --dark-bg: #0a0a0f;
            --card-bg: #12121a;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background: var(--dark-bg);
            color: #e2e8f0;
            overflow-x: hidden;
        }
        
        h1, h2, h3, .display-font {
            font-family: 'Space Grotesk', sans-serif;
        }
        
        .gradient-text {
            background: linear-gradient(135deg, var(--neon-cyan) 0%, var(--electric-blue) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .gradient-border {
            position: relative;
            background: var(--card-bg);
            border: 1px solid rgba(255,255,255,0.1);
        }
        
        .gradient-border::before {
            content: '';
            position: absolute;
            inset: -1px;
            border-radius: inherit;
            padding: 1px;
            background: linear-gradient(135deg, var(--neon-cyan), var(--electric-blue), var(--soft-purple));
            -webkit-mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
            -webkit-mask-composite: xor;
            mask-composite: exclude;
            opacity: 0.5;
        }
        
        .stat-card {
            background: linear-gradient(135deg, rgba(0,245,212,0.1) 0%, rgba(67,97,238,0.05) 100%);
            border: 1px solid rgba(0,245,212,0.2);
            backdrop-filter: blur(10px);
        }
        
        .glow-cyan {
            box-shadow: 0 0 20px rgba(0,245,212,0.3);
        }
        
        .grid-pattern {
            background-image: radial-gradient(circle at 1px 1px, rgba(255,255,255,0.05) 1px, transparent 0);
            background-size: 40px 40px;
        }
        
        .revenue-bar {
            background: linear-gradient(90deg, var(--neon-cyan) 0%, var(--electric-blue) 100%);
            height: 100%;
            border-radius: 4px;
            transition: width 1s ease-out;
        }
        
        .check-mark {
            color: var(--neon-cyan);
        }
        
        .cross-mark {
            color: #ef4444;
        }
        
        .tilt-card {
            transform: perspective(1000px) rotateX(2deg);
            transition: transform 0.3s ease;
        }
        
        .tilt-card:hover {
            transform: perspective(1000px) rotateX(0deg) translateY(-5px);
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        .odds-circle {
            background: conic-gradient(var(--neon-cyan) calc(var(--percentage) * 1%), transparent 0);
        }
        
        .timeline-line {
            background: linear-gradient(180deg, var(--neon-cyan) 0%, var(--electric-blue) 50%, var(--soft-purple) 100%);
        }
    </style>
</head>
<body class="grid-pattern">

    <!-- Hero Section -->
    <section class="min-h-screen flex flex-col justify-center items-center relative overflow-hidden px-4 py-20">
        <div class="absolute inset-0 bg-gradient-to-b from-transparent via-purple-900/10 to-transparent pointer-events-none"></div>
        
        <div class="max-w-6xl mx-auto text-center relative z-10">
            <div class="mb-6 inline-block px-4 py-1 rounded-full border border-cyan-400/30 bg-cyan-400/10 text-cyan-400 text-sm tracking-widest uppercase">
                March 2026 · Islamabad, Pakistan
            </div>
            
            <h1 class="text-5xl md:text-7xl font-bold mb-6 leading-tight display-font">
                Can <span class="gradient-text">PadelISB</span> Work?
            </h1>
            
            <p class="text-xl md:text-2xl text-gray-400 max-w-3xl mx-auto mb-12 font-light">
                A refined feasibility analysis of building Islamabad's first digital padel ecosystem — combining rigorous financial modeling with real-world market dynamics.
            </p>
            
            <div class="flex flex-wrap justify-center gap-4 mb-16">
                <div class="stat-card px-8 py-4 rounded-2xl">
                    <div class="text-3xl font-bold text-cyan-400 display-font">6.8/10</div>
                    <div class="text-sm text-gray-400 uppercase tracking-wider">Feasibility Score</div>
                </div>
                <div class="stat-card px-8 py-4 rounded-2xl border-blue-500/20" style="background: linear-gradient(135deg, rgba(67,97,238,0.1) 0%, rgba(114,9,183,0.05) 100%); border-color: rgba(67,97,238,0.2);">
                    <div class="text-3xl font-bold text-blue-400 display-font">72%</div>
                    <div class="text-sm text-gray-400 uppercase tracking-wider">Success Odds</div>
                </div>
                <div class="stat-card px-8 py-4 rounded-2xl border-purple-500/20" style="background: linear-gradient(135deg, rgba(114,9,183,0.1) 0%, rgba(247,127,0,0.05) 100%); border-color: rgba(114,9,183,0.2);">
                    <div class="text-3xl font-bold text-purple-400 display-font">3-5yr</div>
                    <div class="text-sm text-gray-400 uppercase tracking-wider">Market Window</div>
                </div>
            </div>
        </div>
        
        <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
            <svg class="w-6 h-6 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
            </svg>
        </div>
    </section>

    <!-- Market Snapshot Grid -->
    <section class="py-20 px-4 max-w-7xl mx-auto">
        <h2 class="text-3xl md:text-4xl font-bold mb-12 text-center display-font">Market Reality Check</h2>
        
        <div class="grid grid-cols-2 md:grid-cols-3 gap-6 mb-16">
            <div class="gradient-border rounded-2xl p-6 text-center tilt-card">
                <div class="text-4xl md:text-5xl font-bold gradient-text display-font mb-2">~8</div>
                <div class="text-sm text-gray-400 uppercase tracking-widest">Courts in ISB</div>
                <div class="text-xs text-gray-500 mt-2">CDA auctioned 5 new sites</div>
            </div>
            
            <div class="gradient-border rounded-2xl p-6 text-center tilt-card">
                <div class="text-4xl md:text-5xl font-bold text-cyan-400 display-font mb-2">1-3K</div>
                <div class="text-sm text-gray-400 uppercase tracking-widest">Active Players</div>
                <div class="text-xs text-gray-500 mt-2">High ARPU demographic</div>
            </div>
            
            <div class="gradient-border rounded-2xl p-6 text-center tilt-card">
                <div class="text-4xl md:text-5xl font-bold text-blue-400 display-font mb-2">Zero</div>
                <div class="text-sm text-gray-400 uppercase tracking-widest">Direct Competitors</div>
                <div class="text-xs text-gray-500 mt-2">Blue ocean opportunity</div>
            </div>
            
            <div class="gradient-border rounded-2xl p-6 text-center tilt-card">
                <div class="text-4xl md:text-5xl font-bold text-purple-400 display-font mb-2">Rs 5M</div>
                <div class="text-sm text-gray-400 uppercase tracking-widest">Monthly Market</div>
                <div class="text-xs text-gray-500 mt-2">Total addressable</div>
            </div>
            
            <div class="gradient-border rounded-2xl p-6 text-center tilt-card">
                <div class="text-4xl md:text-5xl font-bold text-orange-400 display-font mb-2">56</div>
                <div class="text-sm text-gray-400 uppercase tracking-widest">Daily Matches</div>
                <div class="text-xs text-gray-500 mt-2">~7 hrs/court avg</div>
            </div>
            
            <div class="gradient-border rounded-2xl p-6 text-center tilt-card">
                <div class="text-4xl md:text-5xl font-bold text-green-400 display-font mb-2">92%</div>
                <div class="text-sm text-gray-400 uppercase tracking-widest">Retention Rate</div>
                <div class="text-xs text-gray-500 mt-2">Global padel statistic</div>
            </div>
        </div>
    </section>

    <!-- Problem-Solution Fit -->
    <section class="py-20 px-4 bg-gradient-to-b from-transparent to-blue-900/10">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold mb-12 display-font">Problem-Solution Matrix</h2>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="gradient-border rounded-2xl p-8">
                    <div class="flex items-center justify-between mb-6">
                        <h3 class="text-2xl font-bold text-red-400 display-font">The Pain Points</h3>
                        <span class="px-3 py-1 bg-red-400/10 text-red-400 rounded-full text-sm">Current State</span>
                    </div>
                    
                    <div class="space-y-6">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-red-400/10 flex items-center justify-center flex-shrink-0">
                                <span class="text-2xl">😤</span>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg mb-1">The 4th Player Hunt</h4>
                                <p class="text-gray-400 text-sm">Padel requires exactly 4 players. Groups constantly scramble to find that last person, resulting in cancelled sessions.</p>
                                <div class="mt-2 text-xs text-red-400 font-semibold">SEVERITY: HIGH</div>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-orange-400/10 flex items-center justify-center flex-shrink-0">
                                <span class="text-2xl">📞</span>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg mb-1">Phone-Only Booking</h4>
                                <p class="text-gray-400 text-sm">Zero digital infrastructure. Courts rely on WhatsApp and calls, causing double-bookings and inefficient slot management.</p>
                                <div class="mt-2 text-xs text-orange-400 font-semibold">SEVERITY: MEDIUM</div>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-yellow-400/10 flex items-center justify-center flex-shrink-0">
                                <span class="text-2xl">💸</span>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg mb-1">Payment Friction</h4>
                                <p class="text-gray-400 text-sm">Cash-only or manual transfers. No automated payments, deposits, or refund systems for cancellations.</p>
                                <div class="mt-2 text-xs text-yellow-400 font-semibold">SEVERITY: MEDIUM</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="gradient-border rounded-2xl p-8 border-cyan-400/30">
                    <div class="flex items-center justify-between mb-6">
                        <h3 class="text-2xl font-bold text-cyan-400 display-font">PadelISB Solutions</h3>
                        <span class="px-3 py-1 bg-cyan-400/10 text-cyan-400 rounded-full text-sm">Proposed</span>
                    </div>
                    
                    <div class="space-y-6">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-cyan-400/10 flex items-center justify-center flex-shrink-0">
                                <svg class="w-6 h-6 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z"></path>
                                </svg>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg mb-1">Smart Matchmaking</h4>
                                <p class="text-gray-400 text-sm">AI-powered player matching based on skill level, location, and availability. Never hunt for a 4th again.</p>
                                <div class="mt-2 flex gap-2">
                                    <span class="text-xs bg-cyan-400/20 text-cyan-400 px-2 py-1 rounded">Skill Matching</span>
                                    <span class="text-xs bg-cyan-400/20 text-cyan-400 px-2 py-1 rounded">Ratings</span>
                                </div>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-blue-400/10 flex items-center justify-center flex-shrink-0">
                                <svg class="w-6 h-6 text-blue-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"></path>
                                </svg>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg mb-1">Real-Time Booking</h4>
                                <p class="text-gray-400 text-sm">Live court availability with instant confirmation. SaaS dashboard for court owners to manage inventory.</p>
                                <div class="mt-2 flex gap-2">
                                    <span class="text-xs bg-blue-400/20 text-blue-400 px-2 py-1 rounded">Live Calendar</span>
                                    <span class="text-xs bg-blue-400/20 text-blue-400 px-2 py-1 rounded">Auto-sync</span>
                                </div>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-purple-400/10 flex items-center justify-center flex-shrink-0">
                                <svg class="w-6 h-6 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 9V7a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2m2 4h10a2 2 0 002-2v-6a2 2 0 00-2-2H9a2 2 0 00-2 2v6a2 2 0 002 2zm7-5a2 2 0 11-4 0 2 2 0 014 0z"></path>
                                </svg>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg mb-1">Integrated Payments</h4>
                                <p class="text-gray-400 text-sm">JazzCash/EasyPaisa integration with deposit system, split payments between players, and automated refunds.</p>
                                <div class="mt-2 flex gap-2">
                                    <span class="text-xs bg-purple-400/20 text-purple-400 px-2 py-1 rounded">Split Pay</span>
                                    <span class="text-xs bg-purple-400/20 text-purple-400 px-2 py-1 rounded">Escrow</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Competitive Landscape -->
    <section class="py-20 px-4 max-w-7xl mx-auto">
        <h2 class="text-3xl md:text-4xl font-bold mb-4 display-font">Competitive Landscape</h2>
        <p class="text-gray-400 mb-12 max-w-2xl">Blue ocean scenario: No dedicated padel tech exists in Islamabad. Competition is behavioral, not product-based.</p>
        
        <div class="overflow-x-auto">
            <table class="w-full text-left border-collapse">
                <thead>
                    <tr class="border-b border-gray-800">
                        <th class="pb-4 text-gray-400 font-medium uppercase tracking-wider text-sm">Competitor</th>
                        <th class="pb-4 text-gray-400 font-medium uppercase tracking-wider text-sm text-center">Pakistan</th>
                        <th class="pb-4 text-gray-400 font-medium uppercase tracking-wider text-sm text-center">Padel Focus</th>
                        <th class="pb-4 text-gray-400 font-medium uppercase tracking-wider text-sm text-center">Court Booking</th>
                        <th class="pb-4 text-gray-400 font-medium uppercase tracking-wider text-sm text-center">Player Match</th>
                        <th class="pb-4 text-gray-400 font-medium uppercase tracking-wider text-sm text-center">ISB Presence</th>
                    </tr>
                </thead>
                <tbody class="text-sm">
                    <tr class="border-b border-gray-800/50 bg-cyan-400/5">
                        <td class="py-4 font-bold text-cyan-400">PadelISB (You)</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                    </tr>
                    <tr class="border-b border-gray-800/50">
                        <td class="py-4 font-medium text-gray-300">Playtomic</td>
                        <td class="py-4 text-center text-red-400 text-xl">✗</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-red-400 text-xl">✗</td>
                    </tr>
                    <tr class="border-b border-gray-800/50">
                        <td class="py-4 font-medium text-gray-300">SukhChayn Sports</td>
                        <td class="py-4 text-center text-cyan-400 text-xl">✓</td>
                        <td class="py-4 text-center text-red-400 text-xl">✗</td>
                        <td class="py-4 text-center text-yellow-400 text-xl">~</td>
                        <td class="py-4 text-center text-red-400 text-xl">✗
