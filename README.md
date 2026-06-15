
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ARC Governance | Enterprise Records, Accountability & Compliance Consulting</title>
    <!-- Google Fonts: Playfair Display for premium luxury serif, Inter for crisp body copy -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        navy: {
                            50: '#f4f6fa',
                            100: '#e9edf5',
                            800: '#0f1e36',
                            900: '#0a1424',
                            950: '#050a12',
                        },
                        beacon: {
                            DEFAULT: '#0066cc',
                            light: '#38bdf8',
                            dark: '#0369a1',
                        },
                        gold: {
                            DEFAULT: '#dca51a',
                            hover: '#c59b27',
                            light: '#f9f5e8',
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    }
                }
            }
        }
    </script>
    <!-- Lucide Icons CDN -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        .gold-gradient-bg {
            background: linear-gradient(135deg, #dca51a 0%, #f3e5ab 50%, #b8860b 100%);
        }
        .hero-glow {
            background: radial-gradient(circle at 50% 30%, rgba(56, 189, 248, 0.05) 0%, rgba(10, 20, 36, 0) 70%);
        }
    </style>
</head>
<body class="bg-navy-950 text-gray-100 font-sans selection:bg-gold selection:text-navy-950">

    <!-- Top micro-banner for urgent advisory vibe -->
    <div class="bg-navy-900 border-b border-navy-800 text-xs text-center py-2 px-4 text-gray-300">
        <span class="inline-flex items-center gap-2">
            <span class="w-2 h-2 rounded-full bg-gold animate-pulse"></span>
            <strong>Active Counsel:</strong> Connecting policy, accountability, and execution across enterprise records architectures.
        </span>
    </div>

    <!-- Navigation Header -->
    <header class="sticky top-0 z-50 bg-navy-950/90 backdrop-blur-md border-b border-navy-800/60 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- ARC Governance Brand Logo -->
                <a href="#" class="flex items-center gap-4 group">
                    <div class="relative w-14 h-14 flex-shrink-0 bg-navy-900 rounded-lg p-1.5 border border-navy-800">
                        <!-- Precise recreate of the new ARC Governance logo mark -->
                        <svg viewBox="0 0 120 120" class="w-full h-full" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <!-- Left diagonal & Overlapping top apex cap -->
                            <path d="M 60 14 L 20 96 L 36 96 L 60 47 L 58 47 L 58 42 L 74 42 Z" fill="#e5e7eb" />
                            <!-- Right diagonal (Gold/Amber) -->
                            <path d="M 58 42 L 74 42 L 100 96 L 84 96 Z" fill="#dca51a" />
                            <!-- Sweeping crescent curve arch (Perfect alignment) -->
                            <path d="M 10 78 C 37 55, 83 55, 110 78 C 83 64, 37 64, 10 78 Z" fill="#ffffff" />
                        </svg>
                    </div>
                    <div class="flex flex-col">
                        <span class="text-xl sm:text-2xl font-serif font-bold tracking-tight text-white leading-none">
                            ARC <span class="text-gold font-bold">Governance</span>
                        </span>
                        <!-- Horizontal separator line mirroring the official corporate logo -->
                        <div class="w-full h-[1px] bg-gray-800 my-1"></div>
                        <span class="text-[8.5px] sm:text-[9.5px] text-gray-300 font-serif italic tracking-wide leading-tight">
                            Accountability • Records • Compliance
                        </span>
                    </div>
                </a>

                <!-- Desktop Nav -->
                <nav class="hidden md:flex items-center gap-8">
                    <a href="#problem" class="text-sm font-medium text-gray-300 hover:text-white transition-colors">The Problem</a>
                    <a href="#services" class="text-sm font-medium text-gray-300 hover:text-white transition-colors">Services</a>
                    <a href="#case-studies" class="text-sm font-medium text-gray-300 hover:text-white transition-colors">Client Cases</a>
                    <a href="#about" class="text-sm font-medium text-gray-300 hover:text-white transition-colors">About Georgina</a>
                    <a href="#pricing" class="text-sm font-medium text-gray-300 hover:text-white transition-colors">Pricing</a>
                </nav>

                <!-- Header Actions -->
                <div class="hidden lg:flex items-center gap-4">
                    <a href="tel:239-237-7242" class="text-sm text-gray-300 hover:text-white flex items-center gap-1.5 font-medium transition-colors">
                        <i data-lucide="phone" class="w-4 h-4 text-gold"></i> 239-237-7242
                    </a>
                    <button onclick="openModal('discovery')" class="bg-gradient-to-r from-gold to-yellow-600 text-navy-950 font-semibold px-5 py-2.5 rounded text-sm hover:brightness-110 active:scale-[0.98] transition-all shadow-lg shadow-gold/10">
                        Schedule Call
                    </button>
                </div>

                <!-- Mobile Menu Button -->
                <button onclick="toggleMobileMenu()" class="md:hidden text-gray-300 hover:text-white p-2" aria-label="Toggle menu">
                    <i data-lucide="menu" id="menu-icon" class="w-6 h-6"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Nav Menu -->
        <div id="mobile-menu" class="hidden md:hidden border-t border-navy-800 bg-navy-950 px-4 py-6 space-y-4">
            <a href="#problem" onclick="toggleMobileMenu()" class="block text-base font-medium text-gray-300 hover:text-white">The Problem</a>
            <a href="#services" onclick="toggleMobileMenu()" class="block text-base font-medium text-gray-300 hover:text-white">Services</a>
            <a href="#case-studies" onclick="toggleMobileMenu()" class="block text-base font-medium text-gray-300 hover:text-white">Client Cases</a>
            <a href="#about" onclick="toggleMobileMenu()" class="block text-base font-medium text-gray-300 hover:text-white">About Georgina</a>
            <a href="#pricing" onclick="toggleMobileMenu()" class="block text-base font-medium text-gray-300 hover:text-white">Pricing</a>
            <div class="pt-4 border-t border-navy-900 space-y-3">
                <a href="tel:239-237-7242" class="flex items-center gap-2 text-gold">
                    <i data-lucide="phone" class="w-5 h-5 text-gold"></i> 239-237-7242
                </a>
                <button onclick="toggleMobileMenu(); openModal('discovery')" class="w-full text-center bg-gradient-to-r from-gold to-yellow-600 text-navy-950 font-semibold py-3 rounded">
                    Schedule Discovery Call
                </button>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative min-h-[90vh] flex items-center py-20 overflow-hidden hero-glow">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-8 items-center">
            <!-- Text Content -->
            <div class="lg:col-span-7 space-y-8">
                <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-gold/10 border border-gold/30 text-gold text-xs font-semibold uppercase tracking-wider">
                    <span class="w-1.5 h-1.5 rounded-full bg-gold animate-ping"></span>
                    Now Advising for 2026 Enterprise Mandates
                </div>

                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-serif font-semibold tracking-tight leading-[1.1] text-white">
                    You Can't Govern <br class="hidden sm:inline" />
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-white via-gray-200 to-gold">What You Can't Find.</span>
                </h1>

                <p class="text-lg sm:text-xl text-gray-300 font-light leading-relaxed">
                    Most organizations sit on years of unmanaged records, unknown retention obligations, and escalating storage costs. ARC Governance provides elite consulting to reduce risk, eliminate waste, and connect strategy to results.
                </p>

                <!-- Mini Bios / Trust builder in Hero -->
                <div class="p-4 rounded bg-navy-900/60 border border-navy-800/80 flex items-start gap-4 max-w-2xl">
                    <div class="w-12 h-12 rounded-full bg-gold/10 flex items-center justify-center flex-shrink-0 border border-gold/30">
                        <i data-lucide="shield-check" class="w-6 h-6 text-gold"></i>
                    </div>
                    <div>
                        <p class="text-sm text-gray-300 leading-relaxed">
                            Led by <strong class="text-white">Georgina Alexis</strong>, former Iron Mountain Client Success professional with <span class="text-gold font-semibold">15+ years</span> of boots-on-the-ground mastery managing high-stakes enterprise compliance portfolios.
                        </p>
                    </div>
                </div>

                <!-- Action Blocks -->
                <div class="flex flex-col sm:flex-row items-stretch sm:items-center gap-4 pt-2">
                    <button onclick="openModal('discovery')" class="bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 active:scale-[0.99] transition-all text-navy-950 font-bold px-8 py-4 rounded text-base text-center shadow-xl shadow-gold/15 flex items-center justify-center gap-2">
                        <span>Schedule a Discovery Call</span>
                        <i data-lucide="arrow-right" class="w-5 h-5"></i>
                    </button>
                    <a href="#calculator" class="bg-navy-900 border border-navy-700 hover:bg-navy-800 text-white font-medium px-8 py-4 rounded text-base text-center transition-all flex items-center justify-center gap-2">
                        <span>Calculate Potential Savings</span>
                        <i data-lucide="calculator" class="w-5 h-5 text-gray-400"></i>
                    </a>
                </div>
            </div>

            <!-- Graphic / Brand Showcase (ARC Governance Core Four Pillars) -->
            <div class="lg:col-span-5 relative">
                <div class="relative mx-auto max-w-[420px] lg:max-w-none">
                    <div class="absolute -inset-2 bg-gradient-to-r from-gold to-yellow-800 rounded-2xl blur-xl opacity-10 animate-pulse"></div>
                    
                    <div class="relative bg-navy-900/95 border border-navy-800 rounded-xl p-6 sm:p-8 shadow-2xl space-y-6">
                        <div class="border-b border-navy-800 pb-3">
                            <h3 class="text-lg font-serif font-bold text-white">ARC Core Framework</h3>
                            <p class="text-xs text-gray-400 mt-1">Connecting policy, accountability, and execution.</p>
                        </div>

                        <!-- 4 Core Pillars matching image_8f8bdf.jpg exactly -->
                        <div class="space-y-4">
                            <!-- Policy -->
                            <div class="flex items-start gap-4 p-2 rounded hover:bg-navy-950/50 transition-colors">
                                <div class="w-10 h-10 rounded-full border border-gold/40 flex items-center justify-center flex-shrink-0 bg-gold/5">
                                    <i data-lucide="shield-alert" class="w-5 h-5 text-gold"></i>
                                </div>
                                <div>
                                    <h4 class="text-sm font-semibold text-white uppercase tracking-wider">Policy</h4>
                                    <p class="text-xs text-gray-400 mt-0.5">Guided by standards and best practices</p>
                                </div>
                            </div>
                            <!-- Accountability -->
                            <div class="flex items-start gap-4 p-2 rounded hover:bg-navy-950/50 transition-colors">
                                <div class="w-10 h-10 rounded-full border border-white/20 flex items-center justify-center flex-shrink-0 bg-white/5">
                                    <i data-lucide="users" class="w-5 h-5 text-white"></i>
                                </div>
                                <div>
                                    <h4 class="text-sm font-semibold text-white uppercase tracking-wider">Accountability</h4>
                                    <p class="text-xs text-gray-400 mt-0.5">Clear ownership and responsibility</p>
                                </div>
                            </div>
                            <!-- Records -->
                            <div class="flex items-start gap-4 p-2 rounded hover:bg-navy-950/50 transition-colors">
                                <div class="w-10 h-10 rounded-full border border-gold/40 flex items-center justify-center flex-shrink-0 bg-gold/5">
                                    <i data-lucide="folder-open" class="w-5 h-5 text-gold"></i>
                                </div>
                                <div>
                                    <h4 class="text-sm font-semibold text-white uppercase tracking-wider">Records</h4>
                                    <p class="text-xs text-gray-400 mt-0.5">Organized. Accessible. Defensible.</p>
                                </div>
                            </div>
                            <!-- Execution -->
                            <div class="flex items-start gap-4 p-2 rounded hover:bg-navy-950/50 transition-colors">
                                <div class="w-10 h-10 rounded-full border border-white/20 flex items-center justify-center flex-shrink-0 bg-white/5">
                                    <i data-lucide="trending-up" class="w-5 h-5 text-white"></i>
                                </div>
                                <div>
                                    <h4 class="text-sm font-semibold text-white uppercase tracking-wider">Execution</h4>
                                    <p class="text-xs text-gray-400 mt-0.5">Turning policy into performance</p>
                                </div>
                            </div>
                        </div>

                        <!-- Elegant visual divider -->
                        <div class="pt-4 border-t border-navy-800 text-center">
                            <p class="text-xs italic text-gray-400">"Governance that connects strategy to results."</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- TRUST & KEY STATS BAR -->
    <section class="border-y border-navy-800 bg-navy-900/40 relative z-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
            <p class="text-center text-xs uppercase tracking-widest text-gray-400 mb-6 font-semibold">Distinguished Experience & Core Competency</p>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center items-center">
                <div class="space-y-1">
                    <p class="text-3xl sm:text-4xl font-serif font-bold text-white">15+</p>
                    <p class="text-xs text-gray-400 uppercase tracking-wider">Years Industry Mastery</p>
                </div>
                <div class="space-y-1">
                    <p class="text-3xl sm:text-4xl font-serif font-bold text-white">70+</p>
                    <p class="text-xs text-gray-400 uppercase tracking-wider">Enterprise Accounts Managed</p>
                </div>
                <div class="space-y-1">
                    <p class="text-3xl sm:text-4xl font-serif font-bold text-gold">Iron Mtn.</p>
                    <p class="text-xs text-gray-400 uppercase tracking-wider">Former Client Success Mgr</p>
                </div>
                <div class="space-y-1">
                    <p class="text-3xl sm:text-4xl font-serif font-bold text-white">Elite</p>
                    <p class="text-xs text-gray-400 uppercase tracking-wider">Healthcare & Finance Advisory</p>
                </div>
            </div>
            
            <div class="mt-8 flex flex-wrap justify-center gap-y-2 gap-x-6 text-xs text-gray-400 border-t border-navy-800/50 pt-6 text-center">
                <span class="flex items-center gap-1"><i data-lucide="check" class="w-3.5 h-3.5 text-gold"></i> Information Governance</span>
                <span class="flex items-center gap-1"><i data-lucide="check" class="w-3.5 h-3.5 text-gold"></i> Records Management</span>
                <span class="flex items-center gap-1"><i data-lucide="check" class="w-3.5 h-3.5 text-gold"></i> Retention Schedule Design</span>
                <span class="flex items-center gap-1"><i data-lucide="check" class="w-3.5 h-3.5 text-gold"></i> Defensible Disposition</span>
            </div>
        </div>
    </section>

    <!-- PROBLEM SECTION -->
    <section id="problem" class="py-24 relative bg-navy-950">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:text-center max-w-3xl mx-auto space-y-4 mb-16">
                <span class="text-sm font-bold text-gold uppercase tracking-widest">The Invisible Exposure</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-white tracking-tight">
                    Most Organizations Have a Records Problem They Don't Know Exists
                </h2>
                <div class="w-12 h-1 bg-gold lg:mx-auto rounded"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Pain Points list -->
                <div class="lg:col-span-7 space-y-6">
                    <p class="text-lg text-gray-300 font-light leading-relaxed">
                        Organizations rarely struggle because they lack storage space. They struggle because they have zero internal visibility. 
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-4">
                        <div class="p-5 rounded bg-navy-900/60 border border-navy-800/80 space-y-3">
                            <div class="w-8 h-8 rounded bg-rose-500/10 flex items-center justify-center"><i data-lucide="clock-alert" class="w-4 h-4 text-rose-400"></i></div>
                            <h4 class="font-semibold text-white">Indefinite Storing</h4>
                            <p class="text-xs text-gray-400">Records are kept years past legal schedules, exponentially stacking monthly liabilities.</p>
                        </div>
                        <div class="p-5 rounded bg-navy-900/60 border border-navy-800/80 space-y-3">
                            <div class="w-8 h-8 rounded bg-rose-500/10 flex items-center justify-center"><i data-lucide="calendar-off" class="w-4 h-4 text-rose-400"></i></div>
                            <h4 class="font-semibold text-white">Outdated Retention</h4>
                            <p class="text-xs text-gray-400">Retention programs remain old or completely unaligned with active legislation.</p>
                        </div>
                        <div class="p-5 rounded bg-navy-900/60 border border-navy-800/80 space-y-3">
                            <div class="w-8 h-8 rounded bg-rose-500/10 flex items-center justify-center"><i data-lucide="map-pin-off" class="w-4 h-4 text-rose-400"></i></div>
                            <h4 class="font-semibold text-white">Zero Accountability</h4>
                            <p class="text-xs text-gray-400">Nobody knows what is in the physical boxes, or which digital folders belong to whom.</p>
                        </div>
                        <div class="p-5 rounded bg-navy-900/60 border border-navy-800/80 space-y-3">
                            <div class="w-8 h-8 rounded bg-rose-500/10 flex items-center justify-center"><i data-lucide="trending-up" class="w-4 h-4 text-rose-400"></i></div>
                            <h4 class="font-semibold text-white">Unending Cost Bloat</h4>
                            <p class="text-xs text-gray-400">Storage bills climb constantly. Valuable operational capital is siphoned into digital dustbins.</p>
                        </div>
                    </div>

                    <p class="text-base text-gray-400 leading-relaxed pt-2">
                        The core issue is rarely your storage vendor. Vendors exist to house your property and charge you rent. <strong class="text-white">The problem is organizational blindness.</strong>
                    </p>
                </div>

                <!-- Contrast Card / Visual Highlight -->
                <div class="lg:col-span-5">
                    <div class="bg-navy-900 rounded-xl p-8 border border-navy-800/80 relative overflow-hidden">
                        <div class="absolute -right-16 -bottom-16 w-48 h-48 bg-rose-500/5 rounded-full blur-xl"></div>
                        
                        <h3 class="text-xl font-serif font-bold text-white mb-4">The Dangerous Reality</h3>
                        <p class="text-sm text-gray-300 leading-relaxed mb-6">
                            When an audit, investigation, or litigation occurs, "I don't know where it is" translates directly to massive non-compliance fines, catastrophic delays, and critical data breaches.
                        </p>

                        <div class="space-y-4 border-t border-navy-800 pt-6">
                            <div class="flex items-center justify-between text-xs text-gray-400">
                                <span>Typical Box Storage Costs / Year</span>
                                <span class="font-semibold text-rose-400">Escalating +15%</span>
                            </div>
                            <div class="flex items-center justify-between text-xs text-gray-400">
                                <span>Employee Time Spent Finding One Document</span>
                                <span class="font-semibold text-rose-400">Avg 2.5 Hours</span>
                            </div>
                            <div class="flex items-center justify-between text-xs text-gray-400">
                                <span>Risk of Keeping Outdated Records</span>
                                <span class="font-semibold text-rose-400">High Legal Exposure</span>
                            </div>
                        </div>

                        <div class="mt-8">
                            <button onclick="openModal('discovery')" class="w-full py-3 text-center bg-rose-950/40 hover:bg-rose-950/60 border border-rose-800/50 text-rose-300 text-sm font-semibold rounded transition-colors">
                                Schedule Free Risk Consultation
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CASE STUDY / STORY #1: THE HEALTHCARE CRISIS -->
    <section id="case-studies" class="py-20 bg-gradient-to-b from-navy-950 to-navy-900/40 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Case study details -->
                <div class="lg:col-span-7 space-y-6">
                    <span class="text-xs font-bold text-gold uppercase tracking-wider">Critical Case Narrative</span>
                    <h3 class="text-3xl font-serif font-bold text-white leading-tight">
                        The Healthcare Client Requesting 100+ Physical Boxes Every Single Day
                    </h3>
                    <div class="w-12 h-0.5 bg-gold"></div>
                    
                    <div class="text-gray-300 space-y-4 leading-relaxed font-light">
                        <p>
                            One major healthcare institution was spending astronomical sums pulling and returning over one hundred physical file boxes from offsite storage, daily. 
                        </p>
                        <p>
                            The root cause was simple yet terrifying: <strong class="text-white">the sole employee who held the mental inventory index had abruptly resigned.</strong> With them went the complete map of their record storage ecosystem.
                        </p>
                        <p>
                            Because they lacked an active metadata index, doctors, legal teams, and administrators were flying completely blind. They had to request entire, massive box sequences just to find a single patient file.
                        </p>
                        <p>
                            We entered the engagement to map exact data flows, restructure box descriptions into clean digital databases, and eliminate the panic pulls.
                        </p>
                    </div>

                    <!-- Signature Pull Quote -->
                    <div class="border-l-4 border-gold bg-navy-950/50 p-6 rounded-r">
                        <p class="text-lg italic text-gray-200 font-serif leading-relaxed">
                            "If your inventory lives inside one employee's head, you don't actually have an inventory. You have a single point of failure."
                        </p>
                        <p class="text-xs text-gold uppercase tracking-wider font-bold mt-3">— Georgina Alexis, Founder</p>
                    </div>
                </div>

                <!-- Graphic Representing Box Pulls -->
                <div class="lg:col-span-5">
                    <div class="bg-navy-950 rounded-lg p-6 border border-navy-800 space-y-6">
                        <div class="flex items-center justify-between border-b border-navy-800 pb-3">
                            <span class="text-xs font-bold uppercase tracking-wider text-beacon-light">Daily Box Retrieval Impact</span>
                            <span class="text-xs text-rose-400 font-semibold">Pre-Intervention</span>
                        </div>
                        
                        <div class="space-y-4">
                            <div>
                                <div class="flex justify-between text-xs text-gray-400 mb-1">
                                    <span>Retrieval Volume</span>
                                    <span>100+ Boxes/Day</span>
                                </div>
                                <div class="w-full bg-navy-900 rounded-full h-2 overflow-hidden">
                                    <div class="bg-rose-500 h-2 rounded-full" style="width: 100%"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between text-xs text-gray-400 mb-1">
                                    <span>Retrieval Overhead Costs</span>
                                    <span>$12,000+ / Month</span>
                                </div>
                                <div class="w-full bg-navy-900 rounded-full h-2 overflow-hidden">
                                    <div class="bg-rose-500 h-2 rounded-full" style="width: 85%"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between text-xs text-gray-400 mb-1">
                                    <span>Administrative Search Latency</span>
                                    <span>Up to 72 Hours</span>
                                </div>
                                <div class="w-full bg-navy-900 rounded-full h-2 overflow-hidden">
                                    <div class="bg-rose-500 h-2 rounded-full" style="width: 90%"></div>
                                </div>
                            </div>
                        </div>

                        <div class="p-4 rounded bg-emerald-500/10 border border-emerald-500/20 space-y-2">
                            <h4 class="text-xs font-bold text-emerald-400 uppercase tracking-widest">Post-Intervention Result</h4>
                            <p class="text-sm text-gray-300">
                                Transformed chaos into searchable digital indices. Physical box pulls dropped by <strong class="text-white">92%</strong> in under 60 days.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- PREMIUM STORAGE COST ESTIMATOR (INTERACTIVE VALUE-ADD) -->
    <section id="calculator" class="py-20 bg-navy-900/30 border-t border-b border-navy-800">
        <div class="max-w-4xl mx-auto px-4 sm:px-6">
            <div class="text-center space-y-4 mb-12">
                <span class="text-xs font-bold text-gold uppercase tracking-widest">Complimentary Strategic Tool</span>
                <h2 class="text-3xl font-serif font-bold text-white">ARC Storage Bleed & Cost Calculator</h2>
                <p class="text-gray-400 text-sm max-w-lg mx-auto">
                    Determine approximately what percentage of your storage budget is spent on "dark data" that could potentially be defensibly destroyed.
                </p>
            </div>

            <!-- Calculator Widget Grid -->
            <div class="bg-navy-950 rounded-xl border border-navy-800 p-6 sm:p-10 shadow-2xl grid grid-cols-1 md:grid-cols-2 gap-8 items-start">
                
                <!-- Input side -->
                <div class="space-y-6">
                    <h3 class="text-lg font-serif font-semibold text-white">Your Storage Environment</h3>
                    
                    <div>
                        <label class="block text-xs font-medium uppercase tracking-wider text-gray-300 mb-2">Estimated Box Count / Digital Folders</label>
                        <div class="relative">
                            <input type="number" id="calc-boxes" value="8500" class="w-full bg-navy-900 border border-navy-850 rounded p-3 text-white focus:outline-none focus:border-gold text-lg font-mono" oninput="calculateSavings()">
                            <span class="absolute right-3 top-3.5 text-xs text-gray-400">Boxes</span>
                        </div>
                    </div>

                    <div>
                        <label class="block text-xs font-medium uppercase tracking-wider text-gray-300 mb-2">Monthly Storage Invoice (USD)</label>
                        <div class="relative">
                            <span class="absolute left-3 top-3 text-lg text-gray-400 font-serif">$</span>
                            <input type="number" id="calc-invoice" value="4800" class="w-full bg-navy-900 border border-navy-850 rounded p-3 pl-8 text-white focus:outline-none focus:border-gold text-lg font-mono" oninput="calculateSavings()">
                            <span class="absolute right-3 top-3.5 text-xs text-gray-400">/mo</span>
                        </div>
                    </div>

                    <div>
                        <label class="block text-xs font-medium uppercase tracking-wider text-gray-300 mb-2">Approx. Years Since Last Major Audit</label>
                        <select id="calc-years" class="w-full bg-navy-900 border border-navy-850 rounded p-3 text-white focus:outline-none focus:border-gold text-base" onchange="calculateSavings()">
                            <option value="1">Less than 2 Years</option>
                            <option value="3" selected>3 to 5 Years (Standard Bloat)</option>
                            <option value="7">6 to 10 Years (Severe accumulation)</option>
                            <option value="12">10+ Years / Never Audited</option>
                        </select>
                    </div>
                </div>

                <!-- Result Side -->
                <div class="bg-navy-900/80 rounded-lg p-6 border border-navy-800 space-y-6 flex flex-col justify-between h-full">
                    <div>
                        <h4 class="text-xs uppercase tracking-wider text-gold font-bold mb-4">Savings Projection Analysis</h4>
                        
                        <div class="space-y-4">
                            <div>
                                <p class="text-xs text-gray-400">Estimated Unmanaged/Expired Records</p>
                                <p class="text-2xl font-serif font-bold text-white" id="outdated-pct">35%</p>
                            </div>
                            <div>
                                <p class="text-xs text-gray-400">Projected Annual Capital Saved</p>
                                <p class="text-3xl font-serif font-bold text-gold" id="annual-savings">$20,160</p>
                            </div>
                            <div>
                                <p class="text-xs text-gray-400">Risk Profile Index</p>
                                <div class="flex items-center gap-2 mt-1">
                                    <span class="px-2.5 py-1 text-xs font-bold rounded" id="risk-badge">Medium Risk</span>
                                    <span class="text-xs text-gray-400" id="risk-desc">Outdated retention framework likely.</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="pt-6 border-t border-navy-800">
                        <button onclick="requestCustomAssessment()" class="w-full bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 text-navy-950 font-bold py-3 px-4 rounded text-sm text-center transition-all flex items-center justify-center gap-2">
                            <span>Request This Assessment Report</span>
                            <i data-lucide="file-text" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CORE SERVICES -->
    <section id="services" class="py-24 relative bg-navy-950">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:text-center max-w-3xl mx-auto space-y-4 mb-20">
                <span class="text-sm font-bold text-gold uppercase tracking-widest">Advisory Programs</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-white tracking-tight">
                    Professional Information Governance Solutions
                </h2>
                <p class="text-lg text-gray-300 font-light">
                    Every service is designed with one singular target: converting chaotic informational debris into a highly compliant, cost-optimized asset.
                </p>
                <div class="w-12 h-1 bg-gold lg:mx-auto rounded"></div>
            </div>

            <!-- Services Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Service 1 -->
                <div class="bg-navy-900 border border-navy-850 hover:border-gold/40 transition-all rounded-xl p-8 space-y-6 group flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="w-12 h-12 rounded bg-gold/10 flex items-center justify-center group-hover:bg-gold/20 transition-all">
                            <i data-lucide="bar-chart-3" class="w-6 h-6 text-gold"></i>
                        </div>
                        <h3 class="text-xl font-serif font-bold text-white">Storage Cost & Inventory Assessment</h3>
                        <p class="text-sm text-gray-300 font-light leading-relaxed">
                            A diagnostic analysis mapping exactly what is being stored, where physical files live, and detailing precise steps to shrink your storage bill.
                        </p>
                        <div class="border-t border-navy-800 pt-4 mt-2">
                            <span class="text-xs font-semibold text-gold uppercase tracking-wider block mb-2">Key Deliverables</span>
                            <ul class="text-xs text-gray-400 space-y-1.5 list-inside list-disc">
                                <li>Comprehensive Offsite Inventory Review</li>
                                <li>Waste Cost & Vendor Contract Optimization</li>
                                <li>Immediate "Quick-Win" Elimination Blueprint</li>
                                <li>Executive Findings Report</li>
                            </ul>
                        </div>
                    </div>
                    <div class="pt-6">
                        <button onclick="openModal('assessment')" class="text-sm font-semibold text-gold hover:text-white flex items-center gap-2 group-hover:translate-x-1 transition-all">
                            Request This Assessment <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>

                <!-- Service 2 -->
                <div class="bg-navy-900 border border-navy-850 hover:border-gold/40 transition-all rounded-xl p-8 space-y-6 group flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="w-12 h-12 rounded bg-gold/10 flex items-center justify-center group-hover:bg-gold/20 transition-all">
                            <i data-lucide="scale" class="w-6 h-6 text-gold"></i>
                        </div>
                        <h3 class="text-xl font-serif font-bold text-white">Retention & Disposition Strategy</h3>
                        <p class="text-sm text-gray-300 font-light leading-relaxed">
                            Create solid operational boundaries matching retention cycles with active industry regulation, legal, and company operational mandates.
                        </p>
                        <div class="border-t border-navy-800 pt-4 mt-2">
                            <span class="text-xs font-semibold text-gold uppercase tracking-wider block mb-2">Key Deliverables</span>
                            <ul class="text-xs text-gray-400 space-y-1.5 list-inside list-disc">
                                <li>Defensible Disposition Framework</li>
                                <li>Regulatory Compliant Retention Schedule</li>
                                <li>Legal Hold Safe Harbor Protocols</li>
                                <li>Multi-System Governance Blueprint</li>
                            </ul>
                        </div>
                    </div>
                    <div class="pt-6">
                        <button onclick="openModal('discovery')" class="text-sm font-semibold text-gold hover:text-white flex items-center gap-2 group-hover:translate-x-1 transition-all">
                            Inquire for Frameworks <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>

                <!-- Service 3 -->
                <div class="bg-navy-900 border border-navy-850 hover:border-gold/40 transition-all rounded-xl p-8 space-y-6 group flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="w-12 h-12 rounded bg-gold/10 flex items-center justify-center group-hover:bg-gold/20 transition-all">
                            <i data-lucide="git-branch" class="w-6 h-6 text-gold"></i>
                        </div>
                        <h3 class="text-xl font-serif font-bold text-white">Records Management Program Design</h3>
                        <p class="text-sm text-gray-300 font-light leading-relaxed">
                            Establish active protocols and records classifications so you stop stacking unnecessary future documents.
                        </p>
                        <div class="border-t border-navy-800 pt-4 mt-2">
                            <span class="text-xs font-semibold text-gold uppercase tracking-wider block mb-2">Key Deliverables</span>
                            <ul class="text-xs text-gray-400 space-y-1.5 list-inside list-disc">
                                <li>Document Lifecycle & Classification Trees</li>
                                <li>Sustainable Accountability Matrix</li>
                                <li>Step-by-Step Employee Training Outlines</li>
                                <li>Policy & Standard Operating Guidelines</li>
                            </ul>
                        </div>
                    </div>
                    <div class="pt-6">
                        <button onclick="openModal('discovery')" class="text-sm font-semibold text-gold hover:text-white flex items-center gap-2 group-hover:translate-x-1 transition-all">
                            View Program Architectures <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>

                <!-- Service 4 -->
                <div class="bg-navy-900 border border-navy-850 hover:border-gold/40 transition-all rounded-xl p-8 space-y-6 group flex flex-col justify-between">
                    <div class="space-y-4">
                        <div class="w-12 h-12 rounded bg-gold/10 flex items-center justify-center group-hover:bg-gold/20 transition-all">
                            <i data-lucide="award" class="w-6 h-6 text-gold"></i>
                        </div>
                        <h3 class="text-xl font-serif font-bold text-white">Information Governance Advisory</h3>
                        <p class="text-sm text-gray-300 font-light leading-relaxed">
                            Ongoing retainer advisory providing high-level executive strategic counsel to keep internal initiatives operating flawlessly.
                        </p>
                        <div class="border-t border-navy-800 pt-4 mt-2">
                            <span class="text-xs font-semibold text-gold uppercase tracking-wider block mb-2">Key Deliverables</span>
                            <ul class="text-xs text-gray-400 space-y-1.5 list-inside list-disc">
                                <li>Monthly Strategy & Direction Reviews</li>
                                <li>Vendor Negotiation Representation</li>
                                <li>Ad-hoc Litigation & Audit Support</li>
                                <li>C-Suite Compliance & Performance Reports</li>
                            </ul>
                        </div>
                    </div>
                    <div class="pt-6">
                        <button onclick="openModal('discovery')" class="text-sm font-semibold text-gold hover:text-white flex items-center gap-2 group-hover:translate-x-1 transition-all">
                            Explore Advisory Retainers <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- STORY SECTION #2: THE 200,000 BOX CRISIS -->
    <section class="py-24 bg-navy-900/20 border-t border-navy-800 overflow-hidden relative">
        <div class="absolute right-0 top-1/2 w-96 h-96 bg-gold/5 rounded-full blur-3xl pointer-events-none transform -translate-y-1/2"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-5 order-last lg:order-first">
                    <div class="relative">
                        <div class="absolute -inset-1 bg-gradient-to-r from-yellow-700 to-gold rounded-xl blur-md opacity-35"></div>
                        <div class="relative bg-navy-950 p-6 sm:p-8 rounded-xl border border-navy-800">
                            <div class="text-center space-y-4">
                                <span class="text-4xl">📦</span>
                                <h4 class="text-2xl font-serif font-bold text-white">200,000 Boxes</h4>
                                <p class="text-xs text-gold font-semibold uppercase tracking-widest">Unsorted Since 1990</p>
                                
                                <div class="bg-navy-900 p-4 rounded text-left space-y-2 border border-navy-800">
                                    <p class="text-xs text-gray-400">"Do you know what you have stored in these boxes?"</p>
                                    <p class="text-xs text-rose-400 font-bold">Answer: "No."</p>
                                </div>
                                <p class="text-xs text-gray-400 italic">"No retention schedules. No framework. Pure historical accumulation."</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-7 space-y-6">
                    <span class="text-xs font-bold text-gold uppercase tracking-widest">Enterprise Case Narrative</span>
                    <h3 class="text-3xl font-serif font-bold text-white leading-tight">
                        Legacy Audit and Phased Disposition Plan
                    </h3>
                    <div class="w-12 h-0.5 bg-gold"></div>

                    <div class="text-gray-300 space-y-4 font-light leading-relaxed">
                        <p>
                            An enterprise corporation had quietly built a mountain of more than <strong class="text-white">200,000 stored boxes</strong> dating back to 1990. They were paying hundreds of thousands annually in ongoing rent with zero visibility.
                        </p>
                        <p>
                            Our team worked directly alongside their general counsel to craft legal retention minimums. We systematically parsed out expired records, saving them from catastrophic litigation exposures.
                        </p>
                        <p>
                            By executing a highly controlled, defensive, phased disposition blueprint, we successfully saved them millions of dollars in immediate retention-termination vendor charges, while protecting executive leadership from auditing liabilities.
                        </p>
                    </div>

                    <div class="flex items-center gap-4 pt-2">
                        <div class="p-3 bg-gold/10 rounded-full border border-gold/20 flex-shrink-0">
                            <i data-lucide="info" class="w-6 h-6 text-gold"></i>
                        </div>
                        <div>
                            <h4 class="text-sm font-semibold text-white">Strategic Outcome</h4>
                            <p class="text-xs text-gray-400">Proper retention programs block data accumulation and instantly clean up existing financial drains.</p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- MEET GEORGINA ALEXIS (ABOUT ME) -->
    <section id="about" class="py-24 bg-navy-950">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- Profile bio details -->
                <div class="lg:col-span-7 space-y-6">
                    <span class="text-xs font-bold text-gold uppercase tracking-widest">Mastery & Background</span>
                    <h2 class="text-3xl sm:text-4xl font-serif font-bold text-white tracking-tight">
                        Meet Georgina Alexis
                    </h2>
                    <p class="text-lg text-gold font-light leading-relaxed">
                        Founder & Principal Governance Advisor
                    </p>
                    <div class="w-12 h-1 bg-gold rounded"></div>

                    <div class="text-gray-300 space-y-4 font-light leading-relaxed">
                        <p>
                            Georgina Alexis has spent more than 15 years on the frontlines of information management, guiding complex companies through storage consolidation, corporate transitions, and intense compliance mandates.
                        </p>
                        <p>
                            Before establishing ARC Governance, she acquired deep operational experience directly working within <strong class="text-white">Iron Mountain Records Management</strong> as:
                        </p>

                        <ul class="space-y-2 pl-4 text-sm text-gray-300">
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold"></i>
                                <span><strong>Client Success Manager</strong> – Iron Mountain Records Management</span>
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold"></i>
                                <span><strong>Preferred Client Services Representative</strong> – Iron Mountain</span>
                            </li>
                            <li class="flex items-center gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold"></i>
                                <span><strong>Issue Resolution Specialist</strong> – Healthcare Vertical</span>
                            </li>
                        </ul>

                        <p>
                            Having overseen over <strong class="text-white">70+ high-tier national enterprise portfolios</strong> across the healthcare, financial, and highly audited compliance space, she knows exactly how storage vendors operate, how they structure contracts, and where the unseen costs lie.
                        </p>
                    </div>

                    <div class="p-5 rounded bg-navy-900 border border-navy-800 space-y-2 max-w-2xl">
                        <h4 class="text-xs font-bold uppercase tracking-wider text-gold">Domain Strengths</h4>
                        <div class="flex flex-wrap gap-2 text-xs">
                            <span class="bg-navy-950 px-2.5 py-1 rounded text-gray-300 border border-navy-850">Offsite Storage Cleanups</span>
                            <span class="bg-navy-950 px-2.5 py-1 rounded text-gray-300 border border-navy-850">Audit Response Mapping</span>
                            <span class="bg-navy-950 px-2.5 py-1 rounded text-gray-300 border border-navy-850">Metadata Rebuilding</span>
                            <span class="bg-navy-950 px-2.5 py-1 rounded text-gray-300 border border-navy-850">Vendor Negotiations</span>
                            <span class="bg-navy-950 px-2.5 py-1 rounded text-gray-300 border border-navy-850">Legal Hold Compliance</span>
                        </div>
                    </div>
                </div>

                <!-- Bio Callout Box / Creative Representation -->
                <div class="lg:col-span-5">
                    <div class="relative">
                        <!-- Background glow effect -->
                        <div class="absolute -inset-1 bg-gradient-to-r from-gold to-yellow-600 rounded-2xl blur opacity-15"></div>
                        <div class="relative bg-navy-900 rounded-xl p-8 border border-navy-850/80 space-y-6">
                            
                            <!-- Avatar / Initials Representation -->
                            <div class="flex items-center gap-4">
                                <div class="w-16 h-16 rounded-full bg-gradient-to-tr from-navy-800 to-navy-700 flex items-center justify-center border-2 border-gold font-serif text-2xl font-bold text-gold">
                                    GA
                                </div>
                                <div>
                                    <h3 class="text-lg font-serif font-bold text-white">Georgina Alexis</h3>
                                    <p class="text-xs text-gray-400">Former Iron Mountain Specialist</p>
                                </div>
                            </div>

                            <p class="text-xs text-gray-400 leading-relaxed italic border-l-2 border-gold pl-4">
                                "In my years auditing records, I've realized the difference between disaster and absolute control is simply a solid, defensible metadata standard."
                            </p>

                            <!-- Credentials Badge list -->
                            <div class="space-y-3 pt-4 border-t border-navy-800">
                                <div class="flex items-center justify-between text-xs">
                                    <span class="text-gray-400">Enterprise Audits Led</span>
                                    <span class="font-bold text-white">70+ Accounts</span>
                                </div>
                                <div class="flex items-center justify-between text-xs">
                                    <span class="text-gray-400">Regulatory Focus Areas</span>
                                    <span class="font-bold text-white">HIPAA, SEC, FINRA, SOX</span>
                                </div>
                                <div class="flex items-center justify-between text-xs">
                                    <span class="text-gray-400">Average Savings Delivered</span>
                                    <span class="font-bold text-emerald-400">30% - 45%</span>
                                </div>
                            </div>

                            <div class="pt-4">
                                <a href="mailto:georginaalexis51@gmail.com" class="block w-full text-center py-3 bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 text-navy-950 text-xs font-bold uppercase tracking-wider rounded transition-all">
                                    Connect with Georgina Alexis
                                </a>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SIMPLE CONSULTING ENGAGEMENTS (PRICING) -->
    <section id="pricing" class="py-24 bg-gradient-to-b from-navy-950 to-navy-900 border-t border-navy-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:text-center max-w-3xl mx-auto space-y-4 mb-20">
                <span class="text-sm font-bold text-gold uppercase tracking-widest">Straightforward Engagements</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-white tracking-tight">
                    Structured Strategy Programs
                </h2>
                <p class="text-lg text-gray-300 font-light">
                    No hidden line-items. Just highly experienced, actionable consulting that pays for itself in immediate storage savings.
                </p>
                <div class="w-12 h-1 bg-gold lg:mx-auto rounded"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 items-stretch mb-12">
                <!-- Tier 1 -->
                <div class="bg-navy-950 rounded-xl p-8 border border-navy-800 hover:border-navy-700 transition-all flex flex-col justify-between">
                    <div class="space-y-6">
                        <div>
                            <span class="text-xs font-bold text-gold uppercase tracking-wider">Level 01</span>
                            <h3 class="text-2xl font-serif font-bold text-white mt-1">ARC Assessment</h3>
                            <p class="text-sm text-gray-400 mt-2 font-light">Best for organizations requiring immediate storage cost clarity.</p>
                        </div>

                        <div class="py-4 border-y border-navy-850">
                            <span class="text-3xl font-serif font-bold text-white">$1,500</span>
                            <span class="text-xs text-gray-400 block mt-1">One-time flat fee</span>
                        </div>

                        <ul class="space-y-3 text-xs text-gray-300">
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>90-Minute Strategic Consultation</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>High-Level Offsite Inventory Audit</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Offsite Storage Cost & Contract Review</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Tailored Opportunities Findings Report</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Savings Implementation Plan</span>
                            </li>
                        </ul>
                    </div>

                    <div class="pt-8">
                        <button onclick="openModal('tier-1')" class="w-full py-3 text-center bg-navy-900 hover:bg-navy-850 border border-navy-800 text-white text-xs font-bold uppercase tracking-wider rounded transition-all">
                            Choose ARC Assessment
                        </button>
                    </div>
                </div>

                <!-- Tier 2 -->
                <div class="bg-navy-950 rounded-xl p-8 border-2 border-gold/75 relative shadow-2xl flex flex-col justify-between transform lg:-translate-y-3">
                    <span class="absolute top-0 right-1/2 translate-x-1/2 -translate-y-1/2 bg-gradient-to-r from-gold to-yellow-600 text-navy-950 text-[10px] font-bold uppercase tracking-widest px-4 py-1.5 rounded-full shadow-lg">
                        Most Highly Requested
                    </span>

                    <div class="space-y-6">
                        <div>
                            <span class="text-xs font-bold text-gold uppercase tracking-wider">Level 02</span>
                            <h3 class="text-2xl font-serif font-bold text-white mt-1">Governance Blueprint</h3>
                            <p class="text-sm text-gray-400 mt-2 font-light">For entities requiring deep structure, regulatory retention paths, and strategic plans.</p>
                        </div>

                        <div class="py-4 border-y border-navy-850">
                            <span class="text-3xl font-serif font-bold text-white">$3,500</span>
                            <span class="text-xs text-gray-400 block mt-1">One-time flat fee</span>
                        </div>

                        <ul class="space-y-3 text-xs text-gray-300">
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span class="font-semibold text-white">Includes Everything in ARC Assessment</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Complete Corporate Retention Audit</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Defensible Disposition Strategy Map</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Comprehensive Governance Roadmaps</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>General Counsel / Executive Briefing Deck</span>
                            </li>
                        </ul>
                    </div>

                    <div class="pt-8">
                        <button onclick="openModal('tier-2')" class="w-full py-3 text-center bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 text-navy-950 text-xs font-bold uppercase tracking-wider rounded transition-all">
                            Choose Governance Blueprint
                        </button>
                    </div>
                </div>

                <!-- Tier 3 -->
                <div class="bg-navy-950 rounded-xl p-8 border border-navy-800 hover:border-navy-700 transition-all flex flex-col justify-between">
                    <div class="space-y-6">
                        <div>
                            <span class="text-xs font-bold text-gold uppercase tracking-wider">Level 03</span>
                            <h3 class="text-2xl font-serif font-bold text-white mt-1">Enterprise Transformation</h3>
                            <p class="text-sm text-gray-400 mt-2 font-light">Custom programmatic overhauls for massive, multi-department networks.</p>
                        </div>

                        <div class="py-4 border-y border-navy-850">
                            <span class="text-3xl font-serif font-bold text-white">Custom</span>
                            <span class="text-xs text-gray-400 block mt-1">Starts at $7,500</span>
                        </div>

                        <ul class="space-y-3 text-xs text-gray-300">
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Comprehensive Multi-Facility Assessments</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Multi-Department Workgroups & Auditing</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Employee Compliance Policy Drafting</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Full Governance Lifecycle Deployment</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <i data-lucide="check" class="w-4 h-4 text-gold flex-shrink-0 mt-0.5"></i>
                                <span>Direct Board Advisory Counsel</span>
                            </li>
                        </ul>
                    </div>

                    <div class="pt-8">
                        <button onclick="openModal('tier-3')" class="w-full py-3 text-center bg-navy-900 hover:bg-navy-850 border border-navy-800 text-white text-xs font-bold uppercase tracking-wider rounded transition-all">
                            Inquire for Enterprise
                        </button>
                    </div>
                </div>
            </div>

            <!-- Ongoing Advisory Retainer Option -->
            <div class="max-w-3xl mx-auto bg-navy-900/60 border border-navy-800 rounded-xl p-6 sm:p-8 flex flex-col sm:flex-row items-center justify-between gap-6">
                <div class="space-y-2">
                    <span class="text-[10px] font-bold text-gold uppercase tracking-widest px-2.5 py-1 bg-gold/10 rounded-full">Strategic Retainer Option</span>
                    <h4 class="text-lg font-serif font-bold text-white">Ongoing Strategic Advisory Counsel</h4>
                    <p class="text-xs text-gray-400 max-w-lg">
                        Steady monthly support, compliance schedule updates, vendor strategy consulting, and C-Suite counsel. Includes two advisory sessions monthly.
                    </p>
                </div>
                <div class="text-right flex-shrink-0 w-full sm:w-auto">
                    <p class="text-2xl font-serif font-bold text-white">$1,250 <span class="text-xs text-gray-400">/ Month</span></p>
                    <button onclick="openModal('advisory')" class="mt-3 w-full sm:w-auto bg-navy-950 hover:bg-navy-800 border border-navy-800 text-gold text-xs font-bold uppercase tracking-wider px-6 py-2.5 rounded transition-all">
                        Retain Advisory
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- WHY ARC GOVERNANCE (VALUES) -->
    <section class="py-24 bg-navy-950 relative overflow-hidden">
        <div class="absolute -left-20 top-1/4 w-80 h-80 bg-gold/5 rounded-full blur-3xl pointer-events-none"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-6 space-y-6">
                    <span class="text-xs font-bold text-gold uppercase tracking-widest">Guiding Tenets</span>
                    <h2 class="text-3xl sm:text-4xl font-serif font-bold text-white tracking-tight">
                        Accountability. Records. Compliance. Continuity.
                    </h2>
                    <div class="w-12 h-1 bg-gold rounded"></div>
                    
                    <p class="text-base text-gray-300 font-light leading-relaxed">
                        Data loss is expensive. Storing useless data is also expensive. We balance both variables by bringing experienced insight directly to your operations and connecting strategy to performance results.
                    </p>

                    <div class="space-y-3">
                        <div class="flex items-center gap-3 text-sm text-gray-300">
                            <i data-lucide="check" class="w-5 h-5 text-emerald-400"></i>
                            <span>Direct vendor pricing consolidation</span>
                        </div>
                        <div class="flex items-center gap-3 text-sm text-gray-300">
                            <i data-lucide="check" class="w-5 h-5 text-emerald-400"></i>
                            <span>Comprehensive mitigation of non-compliance fines</span>
                        </div>
                        <div class="flex items-center gap-3 text-sm text-gray-300">
                            <i data-lucide="check" class="w-5 h-5 text-emerald-400"></i>
                            <span>Instantaneous, audit-ready data tracking indexes</span>
                        </div>
                        <div class="flex items-center gap-3 text-sm text-gray-300">
                            <i data-lucide="check" class="w-5 h-5 text-emerald-400"></i>
                            <span>Absolute protection of institutional metadata knowledge</span>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-6">
                    <!-- Dynamic Graphic showing the realistic Brand Logo inside its complete vector glory -->
                    <div class="bg-navy-900 border border-navy-850 p-8 rounded-xl shadow-2xl relative overflow-hidden h-[380px] flex flex-col justify-between">
                        <!-- Simulated Grid elements representing structured files -->
                        <div class="grid grid-cols-4 gap-2 opacity-15">
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                            <div class="h-10 bg-gold rounded"></div>
                        </div>

                        <!-- Centered ARC logo graphic mark -->
                        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
                            <svg viewBox="0 0 120 120" class="w-72 h-72 text-white drop-shadow-2xl" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <!-- Left diagonal & Overlapping top apex cap -->
                                <path d="M 60 14 L 20 96 L 36 96 L 60 47 L 58 47 L 58 42 L 74 42 Z" fill="#ffffff" opacity="0.95" />
                                <!-- Right diagonal (Gold/Amber) -->
                                <path d="M 58 42 L 74 42 L 100 96 L 84 96 Z" fill="#dca51a" />
                                <!-- Sweeping crescent curve arch crossing legs (Symmetric Arc alignment) -->
                                <path d="M 10 78 C 37 55, 83 55, 110 78 C 83 64, 37 64, 10 78 Z" fill="#ffffff" />
                            </svg>
                        </div>

                        <div class="relative z-10 text-center">
                            <h4 class="text-lg font-serif font-bold text-white mb-2">Eliminate Information Chaos</h4>
                            <p class="text-xs text-gray-400 max-w-xs mx-auto">
                                Transform legacy, unsorted records from ongoing legal hazards into structured, cost-optimized assets.
                            </p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- FINAL CALL TO ACTION / SCHEDULER BLOCK -->
    <section class="py-24 bg-gradient-to-t from-navy-950 to-navy-900 border-t border-navy-800 relative">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 relative z-10 text-center space-y-8">
            <span class="text-xs font-bold text-gold uppercase tracking-widest block">Consultation Booking Portal</span>
            <h2 class="text-3xl sm:text-5xl font-serif font-bold text-white tracking-tight leading-tight">
                Ready to Understand <br class="hidden sm:inline" />What You Have?
            </h2>
            <div class="w-16 h-1 bg-gold mx-auto rounded"></div>
            
            <p class="text-lg text-gray-300 max-w-2xl mx-auto font-light leading-relaxed">
                Every offsite box, server folder, and record holds a story. The question is whether your executive team knows exactly what that story is costing. Let's optimize it.
            </p>

            <div class="bg-navy-950 p-8 rounded-xl border border-navy-800 text-left max-w-2xl mx-auto space-y-6">
                <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 border-b border-navy-900 pb-4">
                    <div>
                        <h4 class="text-sm font-semibold text-white">Direct Advisory Contact</h4>
                        <p class="text-xs text-gray-400">Consult with Georgina Alexis</p>
                    </div>
                    <div class="space-y-1 text-xs text-gray-300">
                        <a href="tel:239-237-7242" class="flex items-center gap-1.5 hover:text-white transition-colors">
                            <i data-lucide="phone" class="w-3.5 h-3.5 text-gold"></i> 239-237-7242
                        </a>
                        <a href="mailto:georginaalexis51@gmail.com" class="flex items-center gap-1.5 hover:text-white transition-colors">
                            <i data-lucide="mail" class="w-3.5 h-3.5 text-gold"></i> georginaalexis51@gmail.com
                        </a>
                    </div>
                </div>

                <!-- Simulation Request Form & Success State Container -->
                <div id="cta-form-container">
                    <form id="discovery-form" onsubmit="handleDiscoverySubmit(event)" class="space-y-4">
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Your Name</label>
                                <input type="text" id="form-name" required placeholder="Georgina Alexis" class="w-full bg-navy-900 border border-navy-850 rounded p-2.5 text-xs text-white focus:outline-none focus:border-gold">
                            </div>
                            <div>
                                <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Corporate Email Address</label>
                                <input type="email" id="form-email" required placeholder="name@company.com" class="w-full bg-navy-900 border border-navy-850 rounded p-2.5 text-xs text-white focus:outline-none focus:border-gold">
                            </div>
                        </div>
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Approximate Records / Box Count</label>
                                <select id="form-size" class="w-full bg-navy-900 border border-navy-850 rounded p-2.5 text-xs text-gray-300 focus:outline-none focus:border-gold">
                                    <option value="unknown">Undetermined / Not sure</option>
                                    <option value="small">Under 1,000 Boxes</option>
                                    <option value="medium">1,000 to 10,000 Boxes</option>
                                    <option value="large">10,000 to 50,000 Boxes</option>
                                    <option value="enterprise">50,000+ Boxes (Highly Complex)</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Primary Objective</label>
                                <select id="form-goal" class="w-full bg-navy-900 border border-navy-850 rounded p-2.5 text-xs text-gray-300 focus:outline-none focus:border-gold">
                                    <option value="costs">Reduce Storage Costs</option>
                                    <option value="compliance">Modernize Retention Schedule</option>
                                    <option value="audit">Prepare for impending Audit/Investigation</option>
                                    <option value="custom">Other Records advisory</option>
                                </select>
                            </div>
                        </div>
                        
                        <button type="submit" class="w-full bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 text-navy-950 font-bold py-3 rounded text-sm text-center tracking-wide transition-all shadow-xl shadow-gold/10 flex items-center justify-center gap-2">
                            <span>Schedule Discovery Call</span>
                            <i data-lucide="arrow-right" class="w-4.5 h-4.5"></i>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-navy-950 border-t border-navy-900 py-16 text-gray-400">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-12 gap-12 items-start mb-12">
            
            <!-- Left Brand Footer segment -->
            <div class="md:col-span-5 space-y-4">
                <a href="#" class="flex items-center gap-3">
                    <div class="w-10 h-10 flex-shrink-0 bg-navy-900 rounded p-1.5 border border-navy-800">
                        <!-- Precise footer SVG matching brand logo image_8f8bdf.jpg -->
                        <svg viewBox="0 0 120 120" class="w-full h-full text-white animate-pulse" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <!-- Left diagonal & Overlapping top apex cap -->
                            <path d="M 60 14 L 20 96 L 36 96 L 60 47 L 58 47 L 58 42 L 74 42 Z" fill="#ffffff" />
                            <!-- Right diagonal (Gold/Amber) -->
                            <path d="M 58 42 L 74 42 L 100 96 L 84 96 Z" fill="#dca51a" />
                            <!-- Sweeping crescent curve arch crossing legs (Symmetric Arc alignment) -->
                            <path d="M 10 78 C 37 55, 83 55, 110 78 C 83 64, 37 64, 10 78 Z" fill="#ffffff" />
                        </svg>
                    </div>
                    <div class="flex flex-col">
                        <span class="text-lg font-serif font-bold text-white tracking-tight leading-none">
                            ARC <span class="text-gold font-bold">Governance</span>
                        </span>
                        <div class="w-24 h-[1px] bg-gray-800 my-1"></div>
                        <span class="text-[9px] text-gray-400 font-serif italic tracking-wide leading-tight">
                            Guiding Organizations. Strategy. Compliance. Continuity.
                        </span>
                    </div>
                </a>
                <p class="text-xs text-gray-400 leading-relaxed max-w-sm pt-2">
                    Helping organizations transform historical records and data landscapes from costly liability burdens into highly organized, defensible strategic assets.
                </p>
                <p class="text-[10px] text-gray-500 font-mono">
                    Led by former Iron Mountain Client Success Professional.
                </p>
            </div>

            <!-- Middle quick links -->
            <div class="md:col-span-3 space-y-4">
                <h4 class="text-xs uppercase tracking-widest text-white font-bold">Services Portal</h4>
                <ul class="space-y-2 text-xs">
                    <li><a href="#services" class="hover:text-white transition-colors">Storage Cost Assessment</a></li>
                    <li><a href="#services" class="hover:text-white transition-colors">Retention & Disposition Strategy</a></li>
                    <li><a href="#services" class="hover:text-white transition-colors">Records Program Development</a></li>
                    <li><a href="#services" class="hover:text-white transition-colors">Information Governance Advisory</a></li>
                </ul>
            </div>

            <!-- Right contact quick segment -->
            <div class="md:col-span-4 space-y-4">
                <h4 class="text-xs uppercase tracking-widest text-white font-bold">Inquiries & Direct Dial</h4>
                <ul class="space-y-2 text-xs">
                    <li class="flex items-center gap-2">
                        <i data-lucide="phone" class="w-4 h-4 text-gold"></i>
                        <a href="tel:239-237-7242" class="hover:text-white transition-colors">239-237-7242</a>
                    </li>
                    <li class="flex items-center gap-2">
                        <i data-lucide="mail" class="w-4 h-4 text-gold"></i>
                        <a href="mailto:georginaalexis51@gmail.com" class="hover:text-white transition-colors">georginaalexis51@gmail.com</a>
                    </li>
                    <li class="text-gray-500 text-[10px] leading-relaxed pt-2">
                        Principal Advisor: Georgina Alexis<br />
                        Availability: Mon – Fri (08:00 – 18:00 EST)
                    </li>
                </ul>
            </div>

        </div>

        <!-- Lower copyright and disclaimer -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-navy-900 pt-8 flex flex-col sm:flex-row justify-between items-center gap-4 text-[11px] text-gray-500">
            <p>© 2026 ARC Governance. All rights reserved.</p>
            <p class="text-center sm:text-right">
                Designed to meet elite SEC, FINRA, HIPAA, SOX, and general corporate record compliance mandates.
            </p>
        </div>
    </footer>

    <!-- INTERACTIVE MODAL COMPONENT -->
    <div id="interactive-modal" class="fixed inset-0 z-50 flex items-center justify-center p-4 bg-navy-950/80 backdrop-blur-sm hidden">
        <div class="bg-navy-900 border border-navy-800 rounded-xl max-w-lg w-full p-6 sm:p-8 relative shadow-2xl space-y-6">
            <button onclick="closeModal()" class="absolute top-4 right-4 text-gray-400 hover:text-white p-1">
                <i data-lucide="x" class="w-5 h-5"></i>
            </button>
            
            <div class="space-y-2">
                <span class="text-[10px] font-bold text-gold uppercase tracking-widest" id="modal-tag">Consulting Request</span>
                <h3 class="text-2xl font-serif font-bold text-white" id="modal-title">Schedule Discovery</h3>
                <p class="text-xs text-gray-400" id="modal-subtitle">Begin mapping out details with Georgina Alexis.</p>
            </div>

            <!-- Modal Content & Form Wrapper -->
            <div id="modal-content-area">
                <form id="modal-form" onsubmit="handleModalSubmit(event)" class="space-y-4">
                    <input type="hidden" id="modal-type" value="default">
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Full Name</label>
                        <input type="text" id="modal-name" required class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold">
                    </div>
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Corporate Email</label>
                        <input type="email" id="modal-email" required class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold">
                    </div>
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Company / Organization Name</label>
                        <input type="text" id="modal-company" placeholder="Enterprise Group" class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold">
                    </div>
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Message or Challenge Details</label>
                        <textarea id="modal-message" rows="3" class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold" placeholder="e.g. We have offsite boxes with outdated tracking indices..."></textarea>
                    </div>

                    <button type="submit" class="w-full bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 text-navy-950 font-bold py-3 rounded text-sm tracking-wide transition-all shadow-lg shadow-gold/10 flex items-center justify-center gap-2">
                        <span>Submit Request</span>
                        <i data-lucide="arrow-right" class="w-4.5 h-4.5"></i>
                    </button>
                </form>
            </div>
        </div>
    </div>

    <!-- NOTIFICATION BOX -->
    <div id="toast-notif" class="fixed bottom-6 right-6 z-50 bg-navy-900 border border-gold/30 p-5 rounded-lg shadow-2xl flex items-start gap-3 max-w-md transform translate-y-20 opacity-0 transition-all duration-300">
        <div class="p-1 rounded bg-gold/10 text-gold"><i data-lucide="mail-check" class="w-5 h-5"></i></div>
        <div class="space-y-1">
            <h4 class="text-sm font-semibold text-white" id="toast-title">Request Transmitted</h4>
            <p class="text-xs text-gray-400" id="toast-message">Your consultation request has been safely dispatched to Georgina Alexis.</p>
        </div>
        <button onclick="hideToast()" class="text-gray-500 hover:text-white ml-2"><i data-lucide="x" class="w-4 h-4"></i></button>
    </div>

    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Responsive Mobile Menu controller
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            const icon = document.getElementById('menu-icon');
            const isHidden = menu.classList.contains('hidden');
            
            if(isHidden) {
                menu.classList.remove('hidden');
                icon.setAttribute('data-lucide', 'x');
            } else {
                menu.classList.add('hidden');
                icon.setAttribute('data-lucide', 'menu');
            }
            lucide.createIcons();
        }

        // INTERACTIVE STORAGE SAVINGS CALCULATOR ALGORITHM
        function calculateSavings() {
            const boxes = parseFloat(document.getElementById('calc-boxes').value) || 0;
            const invoice = parseFloat(document.getElementById('calc-invoice').value) || 0;
            const yearsValue = parseFloat(document.getElementById('calc-years').value) || 1;

            // Algorithm computing standard dark retention waste based on years un-audited
            let outdatedPct = 15; // default base percentage waste
            if(yearsValue === 3) outdatedPct = 35;
            else if(yearsValue === 7) outdatedPct = 55;
            else if(yearsValue === 12) outdatedPct = 75;

            // Compute standard potential annual storage space invoice savings
            const monthlySavings = (invoice * (outdatedPct / 100));
            const annualSavings = Math.round(monthlySavings * 12);

            // Risk tier boundaries
            let riskTier = "Low Risk";
            let riskClass = "bg-emerald-500/10 text-emerald-400 border border-emerald-500/20";
            let riskDesc = "Storage accumulation patterns are under control.";

            if(outdatedPct >= 35 && outdatedPct < 55) {
                riskTier = "Medium Risk";
                riskClass = "bg-amber-500/10 text-amber-400 border border-amber-500/20";
                riskDesc = "Outdated retention framework likely causing budget bleeds.";
            } else if (outdatedPct >= 55) {
                riskTier = "Severe Operational Liability";
                riskClass = "bg-rose-500/10 text-rose-400 border border-rose-500/20";
                riskDesc = "Urgent legal & storage retention overhaul recommended.";
            }

            // Render updates safely
            document.getElementById('outdated-pct').innerText = `${outdatedPct}%`;
            document.getElementById('annual-savings').innerText = `$${annualSavings.toLocaleString()}`;
            
            const badge = document.getElementById('risk-badge');
            badge.innerText = riskTier;
            badge.className = `px-2.5 py-1 text-xs font-bold rounded ${riskClass}`;
            document.getElementById('risk-desc').innerText = riskDesc;
        }

        // Active triggering on request click from calculation
        function requestCustomAssessment() {
            const boxes = document.getElementById('calc-boxes').value;
            const invoice = document.getElementById('calc-invoice').value;
            const years = document.getElementById('calc-years').options[document.getElementById('calc-years').selectedIndex].text;

            openModal('assessment', `Storage Assessment: ${boxes} Boxes / $${invoice}/mo / Last Audit: ${years}`);
        }

        // MODAL MANAGEMENT PORTAL
        function openModal(type, prefilledChallenge = '') {
            const modal = document.getElementById('interactive-modal');
            const modalTag = document.getElementById('modal-tag');
            const modalTitle = document.getElementById('modal-title');
            const modalSubtitle = document.getElementById('modal-subtitle');
            const contentArea = document.getElementById('modal-content-area');

            // Reset modal content area to default form state
            contentArea.innerHTML = `
                <form id="modal-form" onsubmit="handleModalSubmit(event)" class="space-y-4">
                    <input type="hidden" id="modal-type" value="${type}">
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Full Name</label>
                        <input type="text" id="modal-name" required class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold">
                    </div>
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Corporate Email</label>
                        <input type="email" id="modal-email" required class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold">
                    </div>
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Company / Organization Name</label>
                        <input type="text" id="modal-company" placeholder="Enterprise Group" class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold">
                    </div>
                    <div>
                        <label class="block text-[10px] font-bold uppercase tracking-wider text-gray-400 mb-1">Message or Challenge Details</label>
                        <textarea id="modal-message" rows="3" class="w-full bg-navy-950 border border-navy-800 rounded p-2.5 text-sm text-white focus:outline-none focus:border-gold" placeholder="e.g. We have offsite boxes with outdated tracking indices..."></textarea>
                    </div>

                    <button type="submit" class="w-full bg-gradient-to-r from-gold to-yellow-600 hover:brightness-110 text-navy-950 font-bold py-3 rounded text-sm tracking-wide transition-all shadow-lg shadow-gold/10 flex items-center justify-center gap-2">
                        <span>Submit Request</span>
                        <i data-lucide="arrow-right" class="w-4.5 h-4.5"></i>
                    </button>
                </form>
            `;

            if(prefilledChallenge) {
                setTimeout(() => {
                    const msgInput = document.getElementById('modal-message');
                    if (msgInput) msgInput.value = prefilledChallenge;
                }, 50);
            }

            if(type === 'assessment') {
                modalTag.innerText = "Financial Optimization Analysis";
                modalTitle.innerText = "Request Storage Assessment Report";
                modalSubtitle.innerText = "Obtain an exhaustive review of your current physical box billing rates.";
            } else if(type === 'tier-1') {
                modalTag.innerText = "Level 01 Strategy Program";
                modalTitle.innerText = "Inquire: ARC Assessment";
                modalSubtitle.innerText = "Flat fee diagnostic optimization analysis ($1,500).";
            } else if(type === 'tier-2') {
                modalTag.innerText = "Level 02 Strategy Program";
                modalTitle.innerText = "Inquire: Governance Blueprint";
                modalSubtitle.innerText = "All-inclusive retention framework & GC-briefing deck ($3,500).";
            } else if(type === 'tier-3') {
                modalTag.innerText = "Level 03 Strategy Program";
                modalTitle.innerText = "Inquire: Enterprise Transformation";
                modalSubtitle.innerText = "Multi-department programmatic overhauls (Starts at $7,500).";
            } else if(type === 'advisory') {
                modalTag.innerText = "Strategic Advisory Retainer";
                modalTitle.innerText = "Inquire: Governance Advisory";
                modalSubtitle.innerText = "Ongoing operational support retainer ($1,250/mo).";
            } else {
                modalTag.innerText = "Consultation Booking Portal";
                modalTitle.innerText = "Schedule Discovery";
                modalSubtitle.innerText = "Establish solid paths directly with Georgina Alexis.";
            }

            modal.classList.remove('hidden');
            lucide.createIcons();
        }

        // Close modal
        function closeModal() {
            document.getElementById('interactive-modal').classList.add('hidden');
        }

        // NOTIFICATION CONTROLLER (Elegant system alert)
        function triggerToast(title, message) {
            const toast = document.getElementById('toast-notif');
            document.getElementById('toast-title').innerText = title;
            document.getElementById('toast-message').innerText = message;

            toast.classList.remove('translate-y-20', 'opacity-0');
            toast.classList.add('translate-y-0', 'opacity-100');

            setTimeout(() => {
                hideToast();
            }, 6500);
        }

        // Hide toast
        function hideToast() {
            const toast = document.getElementById('toast-notif');
            toast.classList.add('translate-y-20', 'opacity-0');
            toast.classList.remove('translate-y-0', 'opacity-100');
        }

        // SUBMIT HANDLERS (Intercept submission and display real feedback mechanics)
        function handleDiscoverySubmit(e) {
            e.preventDefault();
            const name = document.getElementById('form-name').value;
            const container = document.getElementById('cta-form-container');

            // Swap form content dynamically to show success
            container.innerHTML = `
                <div class="text-center py-8 px-4 space-y-4 bg-navy-900/50 rounded-lg border border-gold/30">
                    <div class="w-16 h-16 bg-gold/10 rounded-full border border-gold/30 flex items-center justify-center mx-auto text-gold animate-bounce">
                        <i data-lucide="award" class="w-8 h-8"></i>
                    </div>
                    <div class="space-y-2">
                        <h4 class="text-xl font-serif font-bold text-white">Discovery requested, ${name}!</h4>
                        <p class="text-xs text-gray-300 max-w-md mx-auto">
                            Georgina Alexis has been notified of your inquiry. We will contact you shortly to schedule your call.
                        </p>
                    </div>
                </div>
            `;
            
            triggerToast(
                "Booking Complete", 
                `Hello ${name}, your discovery session request has been registered successfully!`
            );
            lucide.createIcons();
        }

        function handleModalSubmit(e) {
            e.preventDefault();
            const name = document.getElementById('modal-name').value;
            const contentArea = document.getElementById('modal-content-area');

            // Swap modal content dynamically to present success
            contentArea.innerHTML = `
                <div class="text-center py-8 space-y-4 bg-navy-950 rounded-lg p-6 border border-gold/20">
                    <div class="w-14 h-14 bg-gold/10 rounded-full border border-gold/30 flex items-center justify-center mx-auto text-gold">
                        <i data-lucide="check-circle" class="w-8 h-8"></i>
                    </div>
                    <div class="space-y-2">
                        <h4 class="text-lg font-serif font-bold text-white">Your Request Has Been Filed</h4>
                        <p class="text-xs text-gray-400">
                            Thank you ${name}. Georgina Alexis will connect with your team shortly.
                        </p>
                    </div>
                    <button onclick="closeModal()" class="mt-4 px-6 py-2 bg-navy-900 border border-navy-800 text-xs font-semibold text-white rounded hover:bg-navy-850">Close</button>
                </div>
            `;

            triggerToast(
                "Program Ingested Successfully", 
                `Thank you ${name}. Georgina Alexis will connect with your team shortly.`
            );
            lucide.createIcons();
        }

        // On window startup, trigger base calculation
        window.onload = function() {
            calculateSavings();
        };
    </script>
</body>
</html>
