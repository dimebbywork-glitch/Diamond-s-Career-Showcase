<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diamond Rachel - Career Portfolio & Pivot Showcase</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Arimo:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Space+Grotesk:wght@400;500;700&display=swap" rel="stylesheet">
    <!-- FontAwesome for Premium Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            cream: '#FAF9F6',
                            charcoal: '#2D3436',
                            rose: '#E9967A',
                            roseDark: '#D47A6A',
                            dusty: '#8E909A',
                            terracotta: '#C86A5A',
                            sage: '#8A9A86'
                        }
                    },
                    fontFamily: {
                        sans: ['Arimo', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                        mono: ['Space Grotesk', 'monospace']
                    }
                }
            }
        }
    </script>
    <style>
        .custom-scrollbar::-webkit-scrollbar {
            width: 6px;
            height: 6px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: #FAF9F6;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #E9967A;
            border-radius: 4px;
        }
        .slide-transition {
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .active-dot {
            background-color: #E9967A;
            transform: scale(1.25);
        }
        .drawer-transition {
            transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }
    </style>
</head>
<body class="bg-brand-cream text-brand-charcoal font-sans antialiased selection:bg-brand-rose/30 overflow-x-hidden">

    <!-- NAVIGATION HEADER -->
    <header class="fixed top-0 left-0 w-full bg-brand-cream/90 backdrop-blur-md border-b border-brand-charcoal/10 z-40 px-6 py-4">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 bg-brand-rose rounded-full flex items-center justify-center text-white font-serif font-bold text-lg">DR</div>
                <div>
                    <span class="font-serif font-bold text-lg tracking-wider block">DIAMOND RACHEL</span>
                    <span class="font-mono text-xs text-brand-roseDark tracking-widest uppercase">Success & Curation Specialist</span>
                </div>
            </div>
            
            <!-- Quick Contacts -->
            <div class="hidden lg:flex items-center space-x-6 text-sm font-mono">
                <a href="mailto:diamondrachel34@gmail.com" class="hover:text-brand-rose transition-colors"><i class="fa-solid fa-envelope mr-1 text-brand-rose"></i> diamondrachel34@gmail.com</a>
                <a href="tel:678-360-3681" class="hover:text-brand-rose transition-colors"><i class="fa-solid fa-phone mr-1 text-brand-rose"></i> 678-360-3681</a>
                <span class="text-brand-dusty"><i class="fa-solid fa-location-dot mr-1 text-brand-rose"></i> Atlanta Metro Area</span>
            </div>

            <!-- View Mode Switcher -->
            <div class="flex items-center bg-brand-charcoal/5 p-1 rounded-full border border-brand-charcoal/10">
                <button onclick="setViewMode('deck')" id="btn-deck" class="px-4 py-1.5 rounded-full text-xs font-mono font-bold uppercase transition-all duration-300 bg-brand-charcoal text-brand-cream shadow-sm">
                    <i class="fa-solid fa-chalkboard mr-1.5"></i> Presentation
                </button>
                <button onclick="setViewMode('scroll')" id="btn-scroll" class="px-4 py-1.5 rounded-full text-xs font-mono font-bold uppercase transition-all duration-300 text-brand-charcoal/70 hover:text-brand-charcoal">
                    <i class="fa-solid fa-file-invoice mr-1.5"></i> Portfolio View
                </button>
            </div>
        </div>
    </header>

    <!-- MAIN APP WRAPPER -->
    <main class="pt-24 min-h-screen flex flex-col justify-between">

        <!-- ==================== MODE 1: INTERACTIVE PRESENTATION DECK ==================== -->
        <div id="deck-view-container" class="w-full flex-grow flex flex-col justify-center items-center py-6 px-4">
            
            <!-- Deck Control Bar -->
            <div class="w-full max-w-6xl flex justify-between items-center mb-4 text-xs font-mono text-brand-charcoal/60">
                <span>PITCH DECK: RE-SHAPING THE CLIENT JOURNEY</span>
                <span id="slide-index-indicator">Slide 1 of 10</span>
            </div>

            <!-- Slide Box -->
            <div class="w-full max-w-6xl aspect-[16/9] min-h-[500px] md:min-h-[580px] bg-white rounded-2xl shadow-xl border border-brand-charcoal/10 overflow-hidden relative flex flex-col slide-transition">
                
                <!-- BACKGROUND FLOURISHES -->
                <div class="absolute -top-40 -right-40 w-96 h-96 rounded-full bg-brand-rose/5 blur-3xl pointer-events-none"></div>
                <div class="absolute -bottom-40 -left-40 w-96 h-96 rounded-full bg-brand-sage/5 blur-3xl pointer-events-none"></div>

                <!-- Slide 1: Welcome / Pivot Hook -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14" id="deck-slide-0">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Diamond Rachel</span>
                        <span class="font-mono text-xs text-brand-dusty">01 / INTRODUCTION</span>
                    </div>
                    
                    <div class="my-auto max-w-3xl">
                        <div class="inline-block px-3 py-1 bg-brand-rose/10 text-brand-roseDark font-mono text-xs rounded-full uppercase mb-4">The Pivot Strategy</div>
                        <h1 class="font-serif text-4xl md:text-6xl text-brand-charcoal leading-tight font-bold">
                            Elevating Client Success & Strategic Partnership
                        </h1>
                        <p class="text-lg md:text-xl text-brand-charcoal/70 mt-6 max-w-2xl font-light">
                            Transitioning target business acquisition discipline into long-term accounts management, client retention, and sustainable brand partner growth.
                        </p>
                    </div>

                    <div class="flex items-center space-x-6 border-t border-brand-charcoal/10 pt-6">
                        <div class="flex space-x-2">
                            <span class="w-2.5 h-2.5 rounded-full bg-brand-rose"></span>
                            <span class="w-2.5 h-2.5 rounded-full bg-brand-charcoal/20"></span>
                            <span class="w-2.5 h-2.5 rounded-full bg-brand-charcoal/20"></span>
                        </div>
                        <span class="text-sm font-mono text-brand-dusty font-semibold">Pioneering relationship growth with technical SEO and creative rigor.</span>
                    </div>
                </div>

                <!-- Slide 2: The Core Pivot Philosophy -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-1">
                    <div class="flex justify-between items-start">
                        <span class="font-serif italic text-brand-roseDark text-lg">"Retention is the New Acquisition"</span>
                        <span class="font-mono text-xs text-brand-dusty">02 / CORE PHILOSOPHY</span>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 my-auto">
                        <div>
                            <h2 class="font-serif text-3xl md:text-4xl text-brand-charcoal font-bold leading-snug">The Alignment Framework</h2>
                            <p class="text-base text-brand-charcoal/70 mt-4 leading-relaxed">
                                High-stress transaction models focus entirely on short-term conversions. True expansion occurs when an account delivers consistent value post-sale.
                            </p>
                            <p class="text-base text-brand-charcoal/70 mt-3 leading-relaxed">
                                With a background combining hands-on technical curation and complex account execution, I act as the perfect bridge between customer expectations and actual realization.
                            </p>
                        </div>
                        <div class="bg-brand-cream/60 p-6 rounded-xl border border-brand-charcoal/5 space-y-4 flex flex-col justify-center">
                            <div class="flex items-start space-x-4">
                                <div class="w-10 h-10 bg-brand-rose/20 text-brand-roseDark rounded-lg flex items-center justify-center flex-shrink-0"><i class="fa-solid fa-heart-circle-check"></i></div>
                                <div>
                                    <h4 class="font-bold text-sm">Customer Advocacy First</h4>
                                    <p class="text-xs text-brand-charcoal/60 mt-0.5">Reducing operational friction, boosting LTV, and turning clients into long-term strategic brand promoters.</p>
                                </div>
                            </div>
                            <div class="flex items-start space-x-4">
                                <div class="w-10 h-10 bg-brand-sage/20 text-brand-sage rounded-lg flex items-center justify-center flex-shrink-0"><i class="fa-solid fa-chart-line"></i></div>
                                <div>
                                    <h4 class="font-bold text-sm">Strategic Upsells & Renewals</h4>
                                    <p class="text-xs text-brand-charcoal/60 mt-0.5">Finding organic, low-pressure pathways to expand contract value through continuous data optimization.</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">SHIFTING MINDSETS FROM TRANSACTIONAL TO RELATION-DRIVEN GROWTH</div>
                </div>

                <!-- Slide 3: Pinterest Accomplishments -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-2">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Pinterest Experience</span>
                        <span class="font-mono text-xs text-brand-dusty">03 / PARTNER STEWARDSHIP</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-12 gap-8 my-auto">
                        <div class="md:col-span-7 space-y-4">
                            <h3 class="font-serif text-3xl font-bold text-brand-charcoal">Visual Onboarding & Optimization</h3>
                            <p class="text-base text-brand-charcoal/70">
                                Managed core publisher campaign curation and brand integration strategy on Pinterest's ecosystem. Guided high-budget advertisers from onboarding to live strategy optimization.
                            </p>
                            <ul class="space-y-2 text-sm text-brand-charcoal/80">
                                <li><i class="fa-regular fa-circle-check text-brand-rose mr-2"></i> Onboarded complex digital clients with brand-specific visual templates.</li>
                                <li><i class="fa-regular fa-circle-check text-brand-rose mr-2"></i> Tailored advertising optimization layouts, driving higher organic adoption and campaign CTRs.</li>
                                <li><i class="fa-regular fa-circle-check text-brand-rose mr-2"></i> Fostered creative partnership pathways to maximize platform loyalty and renewals.</li>
                            </ul>
                        </div>
                        <div class="md:col-span-5 bg-brand-rose/5 rounded-xl border border-brand-rose/20 p-6 flex flex-col justify-between">
                            <span class="font-mono text-xs text-brand-roseDark tracking-widest uppercase">Platform Impact</span>
                            <div class="my-4">
                                <div class="text-4xl font-serif font-bold text-brand-roseDark">Seamless Adoption</div>
                                <p class="text-xs text-brand-charcoal/70 mt-2">Drove retention by creating scalable onboarding guides, drastically reducing post-sales customer friction.</p>
                            </div>
                            <div class="h-1 w-full bg-brand-rose/20 rounded-full overflow-hidden">
                                <div class="h-full bg-brand-rose w-4/5 rounded-full"></div>
                            </div>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">HIGHLIGHT: SCALE, CURATION, & MULTI-CHANNEL BRAND ONBOARDING</div>
                </div>

                <!-- Slide 4: Pocket & Mozilla Brand Stewardship -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-3">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-sage tracking-widest text-sm uppercase">Mozilla & Pocket Experience</span>
                        <span class="font-mono text-xs text-brand-dusty">04 / STRATEGIC STEWARDSHIP</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 my-auto">
                        <div class="space-y-4">
                            <h3 class="font-serif text-3xl font-bold text-brand-charcoal">Publisher Alignment & Content Ecosystems</h3>
                            <p class="text-base text-brand-charcoal/70">
                                Curated highly engaged sponsored content streams, balancing corporate publisher monetization metrics with clean editorial curation for over 10M+ daily active web users.
                            </p>
                            <div class="p-4 bg-brand-cream border-l-4 border-brand-sage rounded-r-lg text-sm text-brand-charcoal/70 italic">
                                "Synchronized advertising partnerships with flawless organic end-user experiences."
                            </div>
                        </div>
                        <div class="space-y-4">
                            <h4 class="font-mono text-xs text-brand-sage font-bold tracking-wider uppercase">Strategic Impact Areas:</h4>
                            <div class="grid grid-cols-2 gap-4">
                                <div class="p-3 bg-white rounded-lg border border-brand-charcoal/5">
                                    <div class="text-xl font-bold text-brand-sage">10M+</div>
                                    <div class="text-xs text-brand-dusty">Audience Footprint</div>
                                </div>
                                <div class="p-3 bg-white rounded-lg border border-brand-charcoal/5">
                                    <div class="text-xl font-bold text-brand-sage">98%</div>
                                    <div class="text-xs text-brand-dusty">Quality Score Match</div>
                                </div>
                                <div class="p-3 bg-white rounded-lg border border-brand-charcoal/5">
                                    <div class="text-xl font-bold text-brand-sage">Editorial</div>
                                    <div class="text-xs text-brand-dusty">Cross-Functional Prep</div>
                                </div>
                                <div class="p-3 bg-white rounded-lg border border-brand-charcoal/5">
                                    <div class="text-xl font-bold text-brand-sage">Partner Trust</div>
                                    <div class="text-xs text-brand-dusty">Zero-Risk Escalation</div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">ALIGNING EDITORIAL EXCELLENCE WITH SPONSORED PARTNER VALUE</div>
                </div>

                <!-- Slide 5: Interactive Pivot Translator -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-4">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Value Transformation</span>
                        <span class="font-mono text-xs text-brand-dusty">05 / EXPERIENCE PIVOT TRANSLATOR</span>
                    </div>

                    <div class="my-auto">
                        <h3 class="font-serif text-2xl md:text-3xl font-bold text-brand-charcoal text-center mb-6">Interactive Translation: From Sales to Success</h3>
                        
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                            <!-- Left: Standard BDR Sales Frame -->
                            <div class="p-5 bg-red-50/50 border border-red-200/50 rounded-xl">
                                <h4 class="font-mono text-xs text-red-600 font-bold uppercase tracking-wider mb-3"><i class="fa-solid fa-triangle-exclamation mr-1.5"></i> Traditional Sales Frame (High Stress)</h4>
                                <ul class="space-y-3 text-sm text-brand-charcoal/80">
                                    <li class="p-2.5 rounded hover:bg-white transition-all cursor-pointer border border-transparent hover:border-red-100" onclick="translatePivot(0)">
                                        <div class="font-semibold text-red-800">"Cold Outbound Prospecting & Lead Gen"</div>
                                        <span class="text-xs text-brand-dusty">Focusing on high volumes and arbitrary lists.</span>
                                    </li>
                                    <li class="p-2.5 rounded hover:bg-white transition-all cursor-pointer border border-transparent hover:border-red-100" onclick="translatePivot(1)">
                                        <div class="font-semibold text-red-800">"Objection Handling & Standard Pushes"</div>
                                        <span class="text-xs text-brand-dusty">Pushing past objections transactionally.</span>
                                    </li>
                                    <li class="p-2.5 rounded hover:bg-white transition-all cursor-pointer border border-transparent hover:border-red-100" onclick="translatePivot(2)">
                                        <div class="font-semibold text-red-800">"Hitting Daily Dials & Sales Quotas"</div>
                                        <span class="text-xs text-brand-dusty">Managing numbers without focus on relationship health.</span>
                                    </li>
                                </ul>
                            </div>

                            <!-- Right: Partner & Customer Success Translation -->
                            <div class="p-5 bg-emerald-50/50 border border-emerald-200/50 rounded-xl relative overflow-hidden flex flex-col justify-between">
                                <div class="absolute top-2 right-2 text-emerald-100 text-6xl font-serif pointer-events-none font-bold">Pivot</div>
                                <div>
                                    <h4 class="font-mono text-xs text-emerald-700 font-bold uppercase tracking-wider mb-3"><i class="fa-solid fa-circle-check mr-1.5"></i> Strategic Success Frame (High Value & Retentive)</h4>
                                    <div id="pivot-translation-container" class="space-y-2 p-3 bg-white rounded-lg border border-emerald-100 shadow-sm h-36 flex flex-col justify-center transition-all duration-300">
                                        <div class="font-bold text-brand-charcoal text-base" id="pivot-translated-title">Select a Sales bullet on the left to see the high-value translation!</div>
                                        <p class="text-xs text-brand-charcoal/60" id="pivot-translated-desc">Showing how Diamond's pipeline experiences benefit Customer Retention, Account Health, and Upsells.</p>
                                    </div>
                                </div>
                                <div class="mt-4 text-[10px] font-mono text-emerald-700 uppercase tracking-widest text-center">Click left items to translate</div>
                            </div>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">PROVING SALES ASSETS TRANSLATE DIRECTLY TO STRATEGIC ADVISING</div>
                </div>

                <!-- Slide 6: Digital & Content Strategy Roots -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-5">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Technical Acumen</span>
                        <span class="font-mono text-xs text-brand-dusty">06 / SEO & CONTENT STRATEGY</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 my-auto">
                        <div class="space-y-4">
                            <h3 class="font-serif text-3xl font-bold text-brand-charcoal">SEO Architecture & Discovery Strategy</h3>
                            <p class="text-base text-brand-charcoal/70">
                                Post-sales managers should be strategic, revenue-retaining partners. My deep mastery of Search Engine Optimization (SEO) means I help clients audit their organic discovery maps to secure real digital value.
                            </p>
                            <div class="flex gap-3">
                                <span class="px-2.5 py-1 bg-brand-charcoal/5 rounded font-mono text-xs text-brand-charcoal font-semibold">Google Analytics</span>
                                <span class="px-2.5 py-1 bg-brand-charcoal/5 rounded font-mono text-xs text-brand-charcoal font-semibold">SEM Rush</span>
                                <span class="px-2.5 py-1 bg-brand-charcoal/5 rounded font-mono text-xs text-brand-charcoal font-semibold">Ahrefs</span>
                            </div>
                        </div>
                        <div class="p-6 bg-brand-cream/80 rounded-xl border border-brand-charcoal/10 space-y-4">
                            <h4 class="font-mono text-xs text-brand-roseDark font-bold uppercase tracking-wider">SEO Client Outcomes:</h4>
                            <div class="space-y-3">
                                <div class="flex justify-between items-center text-sm border-b border-brand-charcoal/5 pb-2">
                                    <span>Client Keyword Optimization</span>
                                    <span class="font-bold text-brand-roseDark">#1 Rank Boost</span>
                                </div>
                                <div class="flex justify-between items-center text-sm border-b border-brand-charcoal/5 pb-2">
                                    <span>Inbound Organic Traffic</span>
                                    <span class="font-bold text-brand-roseDark">+35% Growth</span>
                                </div>
                                <div class="flex justify-between items-center text-sm pb-2">
                                    <span>Digital Experience Auditing</span>
                                    <span class="font-bold text-brand-roseDark">Audit & Strategy</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">TECHNICAL DEPTH PROVES STRATEGIC CAPACITY</div>
                </div>

                <!-- Slide 7: Curation & Fashion Merchandising Roots -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-6">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-sage tracking-widest text-sm uppercase">Creative Roots</span>
                        <span class="font-mono text-xs text-brand-dusty">07 / DESIGN & MERCHANDISING</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-12 gap-8 my-auto">
                        <div class="md:col-span-4 bg-brand-sage/5 border border-brand-sage/10 p-6 rounded-xl flex flex-col justify-between">
                            <i class="fa-solid fa-compass-drafting text-brand-sage text-4xl"></i>
                            <div>
                                <h4 class="font-serif text-xl font-bold text-brand-charcoal">The Visual Eye</h4>
                                <p class="text-xs text-brand-charcoal/60 mt-1">My formal background in brand aesthetics & visual merchandising empowers me to guide enterprise brand configurations flawlessly.</p>
                            </div>
                        </div>
                        <div class="md:col-span-8 space-y-4">
                            <h3 class="font-serif text-3xl font-bold text-brand-charcoal">Curation as a Retention Engine</h3>
                            <p class="text-base text-brand-charcoal/70">
                                Having worked inside styling, digital curation, and lifestyle spaces, I approach client brands with immediate intuition. I understand alignment, premium layout standards, and market demographics.
                            </p>
                            <p class="text-base text-brand-charcoal/70">
                                This makes me an exceptional fit for AdTech, creative agency, or enterprise portfolios—transforming relationship management from basic support into high-level visual counsel.
                            </p>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">BRIDGING BRAND REVERENCE WITH CLIENT VALUE EXPANSION</div>
                </div>

                <!-- Slide 8: The "Health Score" Blueprint -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-7">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Execution Methodology</span>
                        <span class="font-mono text-xs text-brand-dusty">08 / CUSTOMER SUCCESS PROCESS</span>
                    </div>

                    <div class="my-auto">
                        <h3 class="font-serif text-3xl font-bold text-brand-charcoal mb-6 text-center">My Strategic Account Playbook</h3>
                        <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                            <div class="p-4 bg-white border border-brand-charcoal/10 rounded-xl relative">
                                <div class="absolute top-2 right-2 text-2xl font-serif text-brand-roseDark opacity-25">01</div>
                                <h4 class="font-bold text-sm">Value Mapping</h4>
                                <p class="text-xs text-brand-charcoal/60 mt-1.5">Deep alignment to understand client definitions of success in the first 30 days.</p>
                            </div>
                            <div class="p-4 bg-white border border-brand-charcoal/10 rounded-xl relative">
                                <div class="absolute top-2 right-2 text-2xl font-serif text-brand-roseDark opacity-25">02</div>
                                <h4 class="font-bold text-sm">Risk Intercepts</h4>
                                <p class="text-xs text-brand-charcoal/60 mt-1.5">Tracking health scores (adoption, campaign engagement) to mitigate risk before contract ends.</p>
                            </div>
                            <div class="p-4 bg-white border border-brand-charcoal/10 rounded-xl relative">
                                <div class="absolute top-2 right-2 text-2xl font-serif text-brand-roseDark opacity-25">03</div>
                                <h4 class="font-bold text-sm">Actionable QBRs</h4>
                                <p class="text-xs text-brand-charcoal/60 mt-1.5">Reframing business reviews on performance metrics rather than defensive account reporting.</p>
                            </div>
                            <div class="p-4 bg-white border border-brand-charcoal/10 rounded-xl relative">
                                <div class="absolute top-2 right-2 text-2xl font-serif text-brand-roseDark opacity-25">04</div>
                                <h4 class="font-bold text-sm">Organic Expansion</h4>
                                <p class="text-xs text-brand-charcoal/60 mt-1.5">Converting client happiness into renewal confidence and low-pressure accounts growth.</p>
                            </div>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">REPLACING RETENTION STRESS WITH SYSTEMATIC PARTNER HEALING</div>
                </div>

                <!-- Slide 9: Professional Pillars Showcase -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-8">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Skill Stack</span>
                        <span class="font-mono text-xs text-brand-dusty">09 / COMPETENCIES</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 my-auto">
                        <div class="p-5 bg-brand-cream border border-brand-charcoal/5 rounded-xl">
                            <h4 class="font-bold mb-3"><i class="fa-solid fa-sliders text-brand-rose mr-1.5"></i> Tooling Ecosystem</h4>
                            <ul class="space-y-1.5 text-xs text-brand-charcoal/70">
                                <li>CRM Mastery (Salesforce, HubSpot)</li>
                                <li>Customer Success (Gainsight, ChurnZero)</li>
                                <li>SEO Operations (Google Search Console, Ahrefs)</li>
                                <li>Team Alignment (Asana, Notion, Slack)</li>
                            </ul>
                        </div>
                        <div class="p-5 bg-brand-cream border border-brand-charcoal/5 rounded-xl">
                            <h4 class="font-bold mb-3"><i class="fa-solid fa-comments text-brand-rose mr-1.5"></i> Stakeholder Advisory</h4>
                            <ul class="space-y-1.5 text-xs text-brand-charcoal/70">
                                <li>Enterprise Handoff Workflows</li>
                                <li>Executive QBR Strategy & Delivery</li>
                                <li>Cross-Functional Ad Operations</li>
                                <li>Partner Onboarding & Program Design</li>
                            </ul>
                        </div>
                        <div class="p-5 bg-brand-cream border border-brand-charcoal/5 rounded-xl">
                            <h4 class="font-bold mb-3"><i class="fa-solid fa-umbrella text-brand-rose mr-1.5"></i> Mitigation Focus</h4>
                            <ul class="space-y-1.5 text-xs text-brand-charcoal/70">
                                <li>Client Health Score Tracking</li>
                                <li>Early Risk Interventions & Playbooks</li>
                                <li>Stable Renewal Strategy & execution</li>
                                <li>Campaign Creative Optimization</li>
                            </ul>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">COMPLETE COMPLIANCE WITH MODERN CUSTOMER OPERATIONS STANDARDS</div>
                </div>

                <!-- Slide 10: Call to Action / Pitch Close -->
                <div class="slide-content h-full flex flex-col justify-between p-8 md:p-14 hidden" id="deck-slide-9">
                    <div class="flex justify-between items-start">
                        <span class="font-mono text-brand-roseDark tracking-widest text-sm uppercase">Next Steps</span>
                        <span class="font-mono text-xs text-brand-dusty">10 / COLLABORATION</span>
                    </div>

                    <div class="text-center my-auto max-w-2xl mx-auto space-y-6">
                        <h3 class="font-serif text-4xl font-bold text-brand-charcoal">Secure Value. Mitigate Stress. Elevate Partners.</h3>
                        <p class="text-base text-brand-charcoal/70 leading-relaxed">
                            I am actively seeking strategic roles within <strong>Customer Success Management, Partner Success Management, or Enterprise Account Support</strong> in the Atlanta Metro Area or remotely. 
                        </p>
                        <p class="text-sm font-mono text-brand-roseDark uppercase tracking-widest">
                            Ready to make an immediate impact on net revenue retention.
                        </p>
                        <div class="pt-4 flex justify-center space-x-4">
                            <a href="mailto:diamondrachel34@gmail.com" class="px-6 py-2.5 bg-brand-charcoal text-brand-cream text-xs font-mono font-bold uppercase rounded-full hover:bg-brand-roseDark transition-colors">
                                <i class="fa-solid fa-envelope mr-1.5"></i> Get in Touch
                            </a>
                            <a href="https://linkedin.com/in/diamond-rachel" target="_blank" class="px-6 py-2.5 bg-brand-cream border border-brand-charcoal/10 text-brand-charcoal text-xs font-mono font-bold uppercase rounded-full hover:border-brand-charcoal transition-colors">
                                <i class="fa-brands fa-linkedin mr-1.5"></i> LinkedIn Profile
                            </a>
                        </div>
                    </div>

                    <div class="text-xs font-mono text-brand-dusty border-t border-brand-charcoal/10 pt-4">DIAMOND RACHEL • ATLANTA, GA • (678) 360-3681</div>
                </div>

                <!-- Deck Navigation Overlays & Footers -->
                <div class="absolute bottom-6 right-8 flex space-x-3 z-20">
                    <button onclick="prevSlide()" class="w-10 h-10 bg-brand-charcoal/5 hover:bg-brand-charcoal hover:text-brand-cream border border-brand-charcoal/10 rounded-full flex items-center justify-center transition-all cursor-pointer">
                        <i class="fa-solid fa-chevron-left text-xs"></i>
                    </button>
                    <button onclick="nextSlide()" class="w-10 h-10 bg-brand-charcoal/5 hover:bg-brand-charcoal hover:text-brand-cream border border-brand-charcoal/10 rounded-full flex items-center justify-center transition-all cursor-pointer">
                        <i class="fa-solid fa-chevron-right text-xs"></i>
                    </button>
                </div>

            </div>

            <!-- Dot Navigation Indicators -->
            <div class="flex space-x-2.5 mt-6 z-20" id="slide-dots-container">
                <!-- Javascript will generate slide indicator dots -->
            </div>
        </div>


        <!-- ==================== MODE 2: INTERACTIVE SCROLLING PORTFOLIO ==================== -->
        <div id="scroll-view-container" class="w-full hidden">
            
            <!-- Hero Splash -->
            <section class="max-w-7xl mx-auto px-6 py-12 md:py-24 grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-7 space-y-6">
                    <span class="font-mono text-xs text-brand-roseDark tracking-widest uppercase bg-brand-rose/10 px-3 py-1 rounded-full">Strategic Relationship Specialist</span>
                    <h1 class="font-serif text-5xl md:text-7xl font-bold leading-tight">Diamond Rachel</h1>
                    <p class="text-xl text-brand-charcoal/70 font-light leading-relaxed">
                        Transitioning outbound sales metrics focus into high-level customer experience support, campaign design, and partner-led revenue retention.
                    </p>
                    <div class="flex flex-wrap gap-4 pt-2">
                        <span class="px-3 py-1.5 bg-brand-charcoal/5 border border-brand-charcoal/10 rounded-full font-mono text-xs"><i class="fa-solid fa-circle-check text-brand-rose mr-1.5"></i> Customer Success Strategy</span>
                        <span class="px-3 py-1.5 bg-brand-charcoal/5 border border-brand-charcoal/10 rounded-full font-mono text-xs"><i class="fa-solid fa-circle-check text-brand-rose mr-1.5"></i> Brand Curation</span>
                        <span class="px-3 py-1.5 bg-brand-charcoal/5 border border-brand-charcoal/10 rounded-full font-mono text-xs"><i class="fa-solid fa-circle-check text-brand-rose mr-1.5"></i> SEO & Discovery Strategy</span>
                    </div>
                </div>
                
                <div class="lg:col-span-5 bg-white p-8 rounded-2xl border border-brand-charcoal/10 shadow-lg space-y-6">
                    <h3 class="font-serif text-2xl font-bold text-brand-charcoal">The Value Pivot</h3>
                    <p class="text-sm text-brand-charcoal/60 leading-relaxed">
                        "I am leveraging my sales-centric focus on client pain points to manage, grow, and renew complex post-sales portfolios. I build low-stress, highly systemized customer retention engines that keep client churn at zero."
                    </p>
                    <div class="border-t border-brand-charcoal/10 pt-4 space-y-3">
                        <div class="flex justify-between text-xs font-mono">
                            <span class="text-brand-dusty">TARGET TARGET ROLES</span>
                            <span class="font-bold text-brand-roseDark">CSM, Account Director, Partner Manager</span>
                        </div>
                        <div class="flex justify-between text-xs font-mono">
                            <span class="text-brand-dusty">PRIMARY LOCATION</span>
                            <span class="font-bold text-brand-roseDark">Atlanta Metro Area (Open to Remote/Hybrid)</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Experience Deep-Dive Timeline section -->
            <section class="bg-white border-t border-b border-brand-charcoal/10 py-16 px-6">
                <div class="max-w-5xl mx-auto space-y-12">
                    <div class="text-center max-w-2xl mx-auto space-y-4">
                        <span class="font-mono text-xs text-brand-roseDark tracking-widest uppercase">Career Chronology</span>
                        <h2 class="font-serif text-3xl md:text-5xl font-bold">Interactively Mapping Accomplishments</h2>
                        <p class="text-sm text-brand-charcoal/60">Explore the major accomplishments of my career pathway, detailing how creative direction, operations management, and metrics drive client stability.</p>
                    </div>

                    <!-- Interactive Experience Showcase Widget -->
                    <div class="bg-brand-cream rounded-2xl border border-brand-charcoal/10 overflow-hidden grid grid-cols-1 md:grid-cols-12">
                        <!-- Navigation Panel -->
                        <div class="md:col-span-4 border-r border-brand-charcoal/10 p-4 space-y-2">
                            <button onclick="selectHistoryTimeline('pinn')" id="hist-btn-pinn" class="w-full text-left p-4 rounded-xl transition-all font-serif font-bold text-lg border bg-white border-brand-rose/30 text-brand-charcoal shadow-sm flex items-center justify-between">
                                <span>Pinterest</span>
                                <i class="fa-solid fa-chevron-right text-xs text-brand-rose"></i>
                            </button>
                            <button onclick="selectHistoryTimeline('moz')" id="hist-btn-moz" class="w-full text-left p-4 rounded-xl transition-all font-serif font-bold text-lg border border-transparent text-brand-charcoal/60 hover:bg-white/50 hover:text-brand-charcoal flex items-center justify-between">
                                <span>Mozilla / Pocket</span>
                                <i class="fa-solid fa-chevron-right text-xs opacity-0"></i>
                            </button>
                            <button onclick="selectHistoryTimeline('sforce')" id="hist-btn-sforce" class="w-full text-left p-4 rounded-xl transition-all font-serif font-bold text-lg border border-transparent text-brand-charcoal/60 hover:bg-white/50 hover:text-brand-charcoal flex items-center justify-between">
                                <span>Salesforce</span>
                                <i class="fa-solid fa-chevron-right text-xs opacity-0"></i>
                            </button>
                            <button onclick="selectHistoryTimeline('seo')" id="hist-btn-seo" class="w-full text-left p-4 rounded-xl transition-all font-serif font-bold text-lg border border-transparent text-brand-charcoal/60 hover:bg-white/50 hover:text-brand-charcoal flex items-center justify-between">
                                <span>SEO & Digital Strategy</span>
                                <i class="fa-solid fa-chevron-right text-xs opacity-0"></i>
                            </button>
                        </div>

                        <!-- Details Panel -->
                        <div class="md:col-span-8 p-6 md:p-10 flex flex-col justify-between min-h-[380px]" id="timeline-detail-box">
                            <div class="space-y-4">
                                <div class="flex justify-between items-center">
                                    <span class="font-mono text-xs text-brand-roseDark font-bold tracking-widest uppercase">Brand Partnerships Manager</span>
                                    <span class="font-mono text-xs text-brand-dusty">CONTRACT</span>
                                </div>
                                <h3 class="font-serif text-2xl md:text-3xl font-bold" id="timeline-title-display">Strategic Partner Curation at Pinterest</h3>
                                <p class="text-sm leading-relaxed text-brand-charcoal/70" id="timeline-desc-display">
                                    Managed onboarding, asset visual layout, and strategic platform delivery for top digital accounts. Aligned cross-functional creative resources to ensure campaign success, boosting user interactions and maintaining platform retention metrics.
                                </p>
                                <div class="space-y-2 pt-2">
                                    <h4 class="font-mono text-xs text-brand-charcoal font-bold uppercase tracking-wider">Major Achievements & Responsibilities:</h4>
                                    <ul class="text-xs text-brand-charcoal/80 space-y-1.5 list-disc pl-4" id="timeline-bullets-display">
                                        <li>Optimized visuals to match strict platform requirements, maximizing engagement potential.</li>
                                        <li>Assisted in post-sale onboarding workflows, ensuring rapid deployment and client alignment.</li>
                                        <li>Conducted regular campaign health checkups, identifying risk items before campaign closures.</li>
                                    </ul>
                                </div>
                            </div>
                            <div class="border-t border-brand-charcoal/10 pt-4 mt-6 flex justify-between items-center text-xs text-brand-dusty">
                                <span>CLIENT ADVISING</span>
                                <span>PINTEREST PORTFOLIO</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Competency Grid Alignment Section -->
            <section class="max-w-7xl mx-auto px-6 py-16 space-y-12">
                <div class="text-center max-w-2xl mx-auto space-y-4">
                    <span class="font-mono text-xs text-brand-roseDark tracking-widest uppercase">The Performance Toolkit</span>
                    <h2 class="font-serif text-3xl md:text-5xl font-bold">Why Hire Me For Success?</h2>
                    <p class="text-sm text-brand-charcoal/60">I substitute typical sales hustle with analytical rigor and curation. Here is the alignment breakdown.</p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <!-- Card 1 -->
                    <div class="p-8 bg-white rounded-2xl border border-brand-charcoal/10 space-y-4 shadow-sm hover:shadow-md transition-all">
                        <div class="w-12 h-12 bg-brand-rose/10 text-brand-roseDark rounded-xl flex items-center justify-center text-xl"><i class="fa-solid fa-address-book"></i></div>
                        <h3 class="font-serif text-xl font-bold">Seamless Onboarding</h3>
                        <p class="text-sm text-brand-charcoal/70 leading-relaxed">
                            First impressions dictate partner retention. I approach onboarding with the structured empathy of a customer advocate, designing tailored launch playbooks that decrease deployment time.
                        </p>
                    </div>
                    <!-- Card 2 -->
                    <div class="p-8 bg-white rounded-2xl border border-brand-charcoal/10 space-y-4 shadow-sm hover:shadow-md transition-all">
                        <div class="w-12 h-12 bg-brand-sage/10 text-brand-sage rounded-xl flex items-center justify-center text-xl"><i class="fa-solid fa-magnifying-glass-chart"></i></div>
                        <h3 class="font-serif text-xl font-bold">Analytical Optimization</h3>
                        <p class="text-sm text-brand-charcoal/70 leading-relaxed">
                            Drawing on my deep SEO experience, I act as an advisory partner. I review performance statistics to optimize account strategies organically, ensuring expansion occurs with low pressure.
                        </p>
                    </div>
                    <!-- Card 3 -->
                    <div class="p-8 bg-white rounded-2xl border border-brand-charcoal/10 space-y-4 shadow-sm hover:shadow-md transition-all">
                        <div class="w-12 h-12 bg-brand-charcoal/10 text-brand-charcoal rounded-xl flex items-center justify-center text-xl"><i class="fa-solid fa-handshake-angle"></i></div>
                        <h3 class="font-serif text-xl font-bold">Consolidated Expansion</h3>
                        <p class="text-sm text-brand-charcoal/70 leading-relaxed">
                            Using structured QBR cycles and consistent health monitoring, I resolve stakeholder friction, guaranteeing client alignment, contract stability, and predictable multi-year renewals.
                        </p>
                    </div>
                </div>
            </section>
        </div>

    </main>

    <!-- FIXED FOOTER ACTIONS -->
    <footer class="bg-brand-charcoal text-brand-cream/80 py-8 px-6 border-t border-brand-brand-charcoal/20 z-10 relative">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-6">
            <div class="text-center md:text-left">
                <span class="font-serif text-lg font-bold text-brand-cream">Diamond Rachel</span>
                <p class="text-xs text-brand-dusty mt-1">Ready for high-impact Customer & Partner Success Roles.</p>
            </div>
            
            <div class="flex flex-wrap justify-center gap-3">
                <button onclick="openModal()" class="px-6 py-2.5 bg-brand-charcoal border border-brand-rose/40 hover:border-brand-rose text-brand-cream font-mono text-xs font-bold uppercase rounded-full shadow-lg transition-all cursor-pointer">
                    <i class="fa-solid fa-file-pdf mr-1.5 text-brand-rose"></i> View Resumé Pivot Outline
                </button>
                <button onclick="toggleAICoPilot()" class="px-6 py-2.5 bg-brand-rose hover:bg-brand-roseDark text-white font-mono text-xs font-bold uppercase rounded-full shadow-lg transition-all cursor-pointer">
                    <i class="fa-solid fa-wand-magic-sparkles mr-1.5"></i> Ask AI Co-Pilot
                </button>
            </div>
            
            <span class="text-xs text-brand-dusty">© 2026. Custom Coded Portfolio Deck.</span>
        </div>
    </footer>

    <!-- INTERACTIVE RESUMÉ OUTLINE MODAL -->
    <div id="resume-modal" class="fixed inset-0 bg-brand-charcoal/80 z-[100] backdrop-blur-sm hidden flex items-center justify-center p-4">
        <div class="bg-white w-full max-w-4xl max-h-[90vh] rounded-2xl shadow-2xl overflow-y-auto custom-scrollbar flex flex-col">
            <!-- Modal Header -->
            <div class="p-6 border-b border-brand-charcoal/10 flex justify-between items-center">
                <div>
                    <h2 class="font-serif text-2xl font-bold text-brand-charcoal">Diamond Rachel</h2>
                    <span class="font-mono text-xs text-brand-roseDark">Proposed Strategic Resume Outline</span>
                </div>
                <button onclick="closeModal()" class="text-brand-charcoal/60 hover:text-brand-charcoal text-2xl cursor-pointer">
                    <i class="fa-solid fa-circle-xmark"></i>
                </button>
            </div>

            <!-- Modal Content -->
            <div class="p-8 space-y-8 text-sm text-brand-charcoal/80">
                
                <!-- Section: Summary -->
                <div class="space-y-3">
                    <h3 class="font-serif text-lg font-bold text-brand-roseDark border-b border-brand-charcoal/15 pb-1">Professional Summary</h3>
                    <p class="leading-relaxed">
                        Results-driven relationship manager and brand steward with 8+ years of expertise spanning content curation, account management, and strategic platform optimizations at <strong>Pinterest</strong> and <strong>Mozilla</strong>. Exceptional background in aligning brand identities with platform standards, managing client expectations, and identifying optimization solutions that drive engagement. Successfully transition high-touch account execution into structured customer growth, mitigating account risk and securing consistent net renewals.
                    </p>
                </div>

                <!-- Section: Core Competencies -->
                <div class="space-y-3">
                    <h3 class="font-serif text-lg font-bold text-brand-roseDark border-b border-brand-charcoal/15 pb-1">Core Professional Competencies</h3>
                    <div class="grid grid-cols-2 md:grid-cols-3 gap-3 font-mono text-xs text-brand-charcoal">
                        <div class="p-2 bg-brand-cream border border-brand-charcoal/5 rounded"><i class="fa-solid fa-user-check text-brand-rose mr-1"></i> Customer Success Manager</div>
                        <div class="p-2 bg-brand-cream border border-brand-charcoal/5 rounded"><i class="fa-solid fa-chart-line text-brand-rose mr-1"></i> Retention & Renewal Strategy</div>
                        <div class="p-2 bg-brand-cream border border-brand-charcoal/5 rounded"><i class="fa-solid fa-hands-holding-circle text-brand-rose mr-1"></i> Strategic Partner Alignment</div>
                        <div class="p-2 bg-brand-cream border border-brand-charcoal/5 rounded"><i class="fa-solid fa-magnifying-glass text-brand-rose mr-1"></i> SEO Architecture Auditing</div>
                        <div class="p-2 bg-brand-cream border border-brand-charcoal/5 rounded"><i class="fa-solid fa-image text-brand-rose mr-1"></i> Visual Brand & Asset Curation</div>
                        <div class="p-2 bg-brand-cream border border-brand-charcoal/5 rounded"><i class="fa-solid fa-shield-halved text-brand-rose mr-1"></i> Account Health Checkups</div>
                    </div>
                </div>

                <!-- Section: Professional Experience -->
                <div class="space-y-6">
                    <h3 class="font-serif text-lg font-bold text-brand-roseDark border-b border-brand-charcoal/15 pb-1">Strategic Experience History</h3>
                    
                    <!-- Exp Block 1 -->
                    <div class="space-y-2">
                        <div class="flex justify-between font-bold text-brand-charcoal">
                            <h4>Brand Partnerships Curation Manager (Pinterest contract)</h4>
                            <span class="font-mono text-xs">2021 — 2022</span>
                        </div>
                        <p class="text-xs italic text-brand-dusty">Steered content recommendation curation and brand integration strategy on Pinterest's core publisher ecosystem.</p>
                        <ul class="list-disc pl-5 space-y-1 text-xs">
                            <li>Managed and nurtured digital accounts onboarding, optimizing platform experiences and aesthetic configurations for peak customer satisfaction.</li>
                            <li>Coordinated directly with cross-functional creative resources to translate client concepts into actionable visual campaigns.</li>
                            <li>Conducted proactive performance diagnostic checks, maintaining low account escalation scores and stable campaign compliance.</li>
                        </ul>
                    </div>

                    <!-- Exp Block 2 -->
                    <div class="space-y-2">
                        <div class="flex justify-between font-bold text-brand-charcoal">
                            <h4>Editorial Content Curation Lead (Mozilla/Pocket contract)</h4>
                            <span class="font-mono text-xs">2021</span>
                        </div>
                        <p class="text-xs italic text-brand-dusty">Maintained and refined recommendation quality parameters, satisfying major publisher growth metrics.</p>
                        <ul class="list-disc pl-5 space-y-1 text-xs">
                            <li>Curated recommendations delivered daily to millions of global web consumers, maintaining strict editorial and partner requirements.</li>
                            <li>Analyzed data metrics to align sponsored monetization strategies smoothly with high organic user retention metrics.</li>
                            <li>Delivered deep qualitative content assessments, establishing visual standards across cross-functional engineering teams.</li>
                        </ul>
                    </div>
                </div>

                <!-- Modal Actions -->
                <div class="pt-4 border-t border-brand-charcoal/10 flex justify-end space-x-3">
                    <button onclick="closeModal()" class="px-5 py-2 bg-brand-charcoal text-white font-mono text-xs font-bold uppercase rounded-full hover:bg-brand-rose transition-colors">
                        Got it!
                    </button>
                </div>
            </div>
        </div>
    </div>


    <!-- ==================== LIVE AI CO-PILOT SIDEBAR DRAWER ==================== -->
    <div id="ai-copilot-drawer" class="fixed top-0 right-0 h-full w-full max-w-md bg-white border-l border-brand-charcoal/10 shadow-2xl z-50 transform translate-x-full drawer-transition flex flex-col">
        <!-- Drawer Header -->
        <div class="p-6 border-b border-brand-charcoal/10 bg-brand-cream/40 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <span class="w-2.5 h-2.5 rounded-full bg-brand-rose animate-ping"></span>
                <h3 class="font-serif font-bold text-lg text-brand-charcoal">Diamond's AI Co-Pilot</h3>
            </div>
            <button onclick="toggleAICoPilot()" class="text-brand-charcoal/60 hover:text-brand-charcoal text-xl transition-colors">
                <i class="fa-solid fa-xmark"></i>
            </button>
        </div>

        <!-- Drawer Tabs -->
        <div class="flex border-b border-brand-charcoal/10 bg-brand-cream/10 text-xs font-mono">
            <button onclick="setAITab('qa')" id="ai-tab-qa" class="flex-1 py-3 text-center border-b-2 border-brand-rose font-bold text-brand-charcoal">
                <i class="fa-solid fa-comments mr-1.5"></i> RECRUITER Q&A
            </button>
            <button onclick="setAITab('pitch')" id="ai-tab-pitch" class="flex-1 py-3 text-center border-b-2 border-transparent text-brand-charcoal/60 hover:text-brand-charcoal transition-all">
                <i class="fa-solid fa-wand-magic-sparkles mr-1.5"></i> INSTANT PITCH
            </button>
        </div>

        <!-- Drawer Body Content -->
        <div class="flex-grow overflow-y-auto custom-scrollbar p-6 flex flex-col justify-between">
            
            <!-- SECTION A: Q&A CHATBOT -->
            <div id="ai-content-qa" class="h-full flex flex-col justify-between space-y-4">
                <!-- Chat Bubbles Area -->
                <div id="ai-chat-history" class="space-y-4 flex-grow overflow-y-auto custom-scrollbar pr-2 max-h-[380px]">
                    <div class="flex items-start space-x-2.5">
                        <div class="w-7 h-7 bg-brand-rose rounded-full flex items-center justify-center text-white text-xs font-serif font-bold">DR</div>
                        <div class="bg-brand-cream/80 border border-brand-charcoal/5 p-3 rounded-2xl rounded-tl-none text-xs text-brand-charcoal max-w-[85%]">
                            Hi there! I'm Diamond's career advisor AI. Ask me anything about her skills, her transitions, why she excels at post-sales account retention, or her specific achievements at Pinterest and Mozilla!
                        </div>
                    </div>
                </div>

                <!-- Quick Query Pills -->
                <div class="flex flex-wrap gap-2 pt-2">
                    <button onclick="submitQuickQuery('Why is Diamond a good fit for Customer Success?')" class="text-[10px] font-mono border border-brand-charcoal/10 rounded-full px-2.5 py-1 text-brand-charcoal hover:border-brand-rose hover:text-brand-rose transition-all">
                        CSM Fit?
                    </button>
                    <button onclick="submitQuickQuery('Describe her strategy at Pinterest.')" class="text-[10px] font-mono border border-brand-charcoal/10 rounded-full px-2.5 py-1 text-brand-charcoal hover:border-brand-rose hover:text-brand-rose transition-all">
                        Pinterest Role?
                    </button>
                    <button onclick="submitQuickQuery('How does she handle customer renewals?')" class="text-[10px] font-mono border border-brand-charcoal/10 rounded-full px-2.5 py-1 text-brand-charcoal hover:border-brand-rose hover:text-brand-rose transition-all">
                        Renewals approach?
                    </button>
                </div>

                <!-- Input area -->
                <div class="border-t border-brand-charcoal/10 pt-3 flex items-center space-x-2">
                    <input type="text" id="ai-chat-input" placeholder="Type a question for Diamond's AI..." class="flex-grow text-xs border border-brand-charcoal/10 rounded-lg px-3 py-2.5 focus:outline-none focus:border-brand-rose">
                    <button onclick="sendChatMessage()" class="w-10 h-10 bg-brand-charcoal text-brand-cream rounded-lg hover:bg-brand-rose transition-all flex items-center justify-center">
                        <i id="send-chat-icon" class="fa-solid fa-paper-plane text-xs"></i>
                    </button>
                </div>
            </div>

            <!-- SECTION B: OUTREACH & COVER LETTER GENERATOR -->
            <div id="ai-content-pitch" class="hidden flex flex-col justify-between h-full space-y-4">
                <div class="space-y-4">
                    <span class="text-xs text-brand-charcoal/60 leading-relaxed block">
                        Input details of a target position below to instantly generate an outreach message bridging Diamond's brand success experience with that specific role.
                    </span>
                    
                    <div class="space-y-3">
                        <div>
                            <label class="block font-mono text-[10px] text-brand-charcoal/80 uppercase tracking-wider mb-1 font-bold">Target Company</label>
                            <input type="text" id="pitch-company" placeholder="e.g. Mailchimp, Salesloft, Salesforce" class="w-full text-xs border border-brand-charcoal/10 rounded-lg px-3 py-2 focus:outline-none focus:border-brand-rose">
                        </div>
                        <div>
                            <label class="block font-mono text-[10px] text-brand-charcoal/80 uppercase tracking-wider mb-1 font-bold">Target Job Title</label>
                            <input type="text" id="pitch-title" placeholder="e.g. Customer Success Manager, Partner Manager" class="w-full text-xs border border-brand-charcoal/10 rounded-lg px-3 py-2 focus:outline-none focus:border-brand-rose">
                        </div>
                        <div>
                            <label class="block font-mono text-[10px] text-brand-charcoal/80 uppercase tracking-wider mb-1 font-bold">Focus Highlight</label>
                            <select id="pitch-focus" class="w-full text-xs border border-brand-charcoal/10 rounded-lg px-3 py-2 focus:outline-none focus:border-brand-rose bg-white">
                                <option value="onboarding">Pinterest Visual Onboarding Focus</option>
                                <option value="retention">Mozilla Partner Retention & Curation</option>
                                <option value="seo">SEO & Analytics Optimization Advisory</option>
                                <option value="all">Consolidated (Aesthetics & Data Strategy)</option>
                            </select>
                        </div>
                    </div>

                    <button onclick="generateCustomPitch()" class="w-full py-2.5 bg-brand-rose hover:bg-brand-roseDark text-white font-mono text-xs font-bold uppercase rounded-lg shadow-md transition-colors flex items-center justify-center space-x-2">
                        <i class="fa-solid fa-sparkles"></i>
                        <span>Generate Pivot Pitch</span>
                    </button>
                </div>

                <!-- Output Area -->
                <div class="flex-grow flex flex-col justify-end pt-4">
                    <label class="block font-mono text-[10px] text-brand-charcoal/80 uppercase tracking-wider mb-1 font-bold">Generated Outreach Strategy</label>
                    <div class="bg-brand-cream/80 border border-brand-charcoal/10 rounded-xl p-4 min-h-[160px] max-h-[220px] overflow-y-auto custom-scrollbar relative">
                        <p id="pitch-output-text" class="text-xs text-brand-charcoal/80 italic whitespace-pre-line leading-relaxed">
                            A custom crafted response will appear here...
                        </p>
                        <!-- Copy Trigger -->
                        <button onclick="copyGeneratedPitch()" class="absolute bottom-2 right-2 text-brand-dusty hover:text-brand-rose text-xs bg-white p-1 rounded border border-brand-charcoal/10">
                            <i class="fa-solid fa-copy"></i>
                        </button>
                    </div>
                </div>
            </div>

        </div>

        <!-- Drawer Footer -->
        <div class="p-4 border-t border-brand-charcoal/10 bg-brand-cream/20 text-[10px] font-mono text-brand-dusty text-center">
            Leveraging real-time contextual Gemini Grounding.
        </div>
    </div>

    <!-- Toast Notification Banner -->
    <div id="toast-notif" class="fixed bottom-6 left-6 bg-brand-charcoal text-brand-cream px-5 py-3 rounded-xl shadow-2xl font-mono text-xs hidden z-50 flex items-center space-x-2 border border-brand-rose/30">
        <i class="fa-solid fa-circle-check text-brand-rose"></i>
        <span id="toast-message">Message copied!</span>
    </div>


    <!-- ==================== JAVASCRIPT LOGIC ==================== -->
    <script>
        // App State
        let currentSlide = 0;
        const totalSlides = 10;
        let activeViewMode = 'deck'; // 'deck' or 'scroll'
        let aiDrawerOpen = false;
        let activeAiTab = 'qa'; // 'qa' or 'pitch'

        // Resume Metadata injected for Gemini API
        // This acts as local context knowledge for the model.
        const diamondResumeContext = `
            Candidate Name: Diamond Rachel
            Location: Atlanta, GA Area
            Phone: (678) 360-3681
            Email: diamondrachel34@gmail.com
            Target Roles: Customer Success Manager (CSM), Partner Success Specialist, Account Director, Partner Manager
            
            Work Experience Summary:
            1. Salesforce (Enterprise Account Representative - 2022-2023): Partnered in tandem with Enterprise Account Executives (AEs) to navigate multi-layered corporate structures, diagnose operational client bottlenecks, map software solution paths, and secure executive alignment.
            2. Pinterest (Brand Partnerships Manager - 2021-2022): Coordinated client visual onboarding strategies, trained high-budget advertising partners, and optimized campaign visuals (Pinterest Ads) to enhance campaign click-through and platform loyalty.
            3. Mozilla & Pocket (Editorial Content Lead / Publisher Success - 2021): Managed relationships with major publishing organizations, curated recommendation flows for over 10M+ daily active web users, and balanced publisher monetization with exceptional retention.
            4. AdRoll (Agency Account Associate - 2021): Teamed up with Senior Account Executives to present customized retargeting and display marketing strategies to advertising agencies, managing client health and renewals.
            5. Independent SEO Strategist (2018-2021): Tailored complete keyword maps and SEO audits for startup companies, achieving rank boosts and high organic audience retention.
            6. Visual Merchandising (Various Leaders - 2015-2018): Styled physical product footprints, restructured visual inventories, and curated premium loyalty relationships.
            
            Pivot Philosophy: Transitioning pipeline creation discipline and business cycle knowledge into long-term accounts management, strategic publisher alignment, and zero-churn retention outcomes. Highly creative eye with solid data/analytical strategy capacity.
        `;

        // Timeline History Data mapping
        const historyData = {
            pinn: {
                title: "Strategic Partner Curation at Pinterest",
                desc: "Managed onboarding, asset visual layout, and strategic platform delivery for top digital accounts. Aligned cross-functional creative resources to ensure campaign success, boosting user interactions and maintaining platform retention metrics.",
                bullets: [
                    "Optimized visuals to match strict platform requirements, maximizing engagement potential.",
                    "Assisted in post-sale onboarding workflows, ensuring rapid deployment and client alignment.",
                    "Conducted regular campaign health checkups, identifying risk items before campaign closures."
                ],
                role: "Brand Partnerships Manager",
                type: "CONTRACT"
            },
            moz: {
                title: "Editorial Curation Lead at Mozilla & Pocket",
                desc: "Supervised high-volume digital content streams, aligning publisher revenue agendas with editorial aesthetics. Curated recommended articles and sponsorships reaching over 10M+ daily visitors worldwide.",
                bullets: [
                    "Balanced delicate sponsor expectations with highly critical audience expectations.",
                    "Established robust quality metric criteria, decreasing user experience complaint reviews.",
                    "Aligned daily deliverables with cross-functional engineering and visual support teams."
                ],
                role: "Editorial Lead Coordinator",
                type: "CONTRACT"
            },
            sforce: {
                title: "Enterprise Solutions Mapping at Salesforce",
                desc: "Partnered in tandem with Enterprise Account Executives to map complex workflow software solutions for corporate clients, establishing clean handoff pathways.",
                bullets: [
                    "Conducted thorough account operational diagnostic audits to pinpoint workflow gaps.",
                    "Strategized with AEs to custom-tailor Sales Cloud & Service Cloud offerings for stakeholders.",
                    "Designed relationship transition paths to secure client trust during the early sales lifecycle."
                ],
                role: "Enterprise Representative",
                type: "SALES OPERATIONS"
            },
            seo: {
                title: "Organic Strategy Architect",
                desc: "Designed and engineered complex keyword systems and content maps to help brands scale. Performed complete audits of visual navigation systems to match target client acquisition requirements.",
                bullets: [
                    "Increased search visibility and ranked primary keywords to Google position #1.",
                    "Drafted tailored analytical tracking dashboards to present organic account health metrics directly to stakeholders.",
                    "Automated key customer content auditing systems, reducing strategic advising assessment times by 40%."
                ],
                role: "SEO & Digital Strategy Consultant",
                type: "INDEPENDENT"
            }
        };

        // Pivot Translation Data
        const pivotTranslations = [
            {
                title: "Strategic Client Onboarding",
                desc: "Instead of cold messaging to fill pipelines, I leverage acquisition strategy to structure zero-friction client onboarding setups, ensuring customers reach 'first-value' in record time."
            },
            {
                title: "Data-Driven Relationship Advisory",
                desc: "I replace tactical 'objection handling' with analytical review meetings. I treat objections as system optimization cues, advising customers with deep SEO and visual insight."
            },
            {
                title: "Account Health & Risk Prevention",
                desc: "Quotas focus on the short-term. I treat account expansion as an ongoing growth goal—watching metrics, managing risk early, and safeguarding consistent renewals."
            }
        ];

        // Slide Dots Init
        window.onload = function() {
            const dotsContainer = document.getElementById('slide-dots-container');
            dotsContainer.innerHTML = '';
            for(let i = 0; i < totalSlides; i++) {
                const dot = document.createElement('button');
                dot.className = `w-3 h-3 rounded-full bg-brand-charcoal/20 hover:bg-brand-rose transition-all cursor-pointer ${i === 0 ? 'active-dot' : ''}`;
                dot.id = `slide-dot-${i}`;
                dot.onclick = () => goToSlide(i);
                dotsContainer.appendChild(dot);
            }
            updateSlideView();
        }

        // View Mode Switcher
        function setViewMode(mode) {
            activeViewMode = mode;
            const deckContainer = document.getElementById('deck-view-container');
            const scrollContainer = document.getElementById('scroll-view-container');
            const btnDeck = document.getElementById('btn-deck');
            const btnScroll = document.getElementById('btn-scroll');

            if (mode === 'deck') {
                deckContainer.classList.remove('hidden');
                scrollContainer.classList.add('hidden');
                btnDeck.className = "px-4 py-1.5 rounded-full text-xs font-mono font-bold uppercase transition-all duration-300 bg-brand-charcoal text-brand-cream shadow-sm";
                btnScroll.className = "px-4 py-1.5 rounded-full text-xs font-mono font-bold uppercase transition-all duration-300 text-brand-charcoal/70 hover:text-brand-charcoal";
            } else {
                deckContainer.classList.add('hidden');
                scrollContainer.classList.remove('hidden');
                btnScroll.className = "px-4 py-1.5 rounded-full text-xs font-mono font-bold uppercase transition-all duration-300 bg-brand-charcoal text-brand-cream shadow-sm";
                btnDeck.className = "px-4 py-1.5 rounded-full text-xs font-mono font-bold uppercase transition-all duration-300 text-brand-charcoal/70 hover:text-brand-charcoal";
            }
        }

        // Slide navigation
        function goToSlide(index) {
            currentSlide = index;
            updateSlideView();
        }

        function nextSlide() {
            if (currentSlide < totalSlides - 1) {
                currentSlide++;
            } else {
                currentSlide = 0; // wrap around
            }
            updateSlideView();
        }

        function prevSlide() {
            if (currentSlide > 0) {
                currentSlide--;
            } else {
                currentSlide = totalSlides - 1; // wrap around
            }
            updateSlideView();
        }

        function updateSlideView() {
            // Update slides visibility
            for (let i = 0; i < totalSlides; i++) {
                const slide = document.getElementById(`deck-slide-${i}`);
                const dot = document.getElementById(`slide-dot-${i}`);
                if (slide) {
                    if (i === currentSlide) {
                        slide.classList.remove('hidden');
                    } else {
                        slide.classList.add('hidden');
                    }
                }
                if (dot) {
                    if (i === currentSlide) {
                        dot.classList.add('active-dot');
                    } else {
                        dot.classList.remove('active-dot');
                    }
                }
            }
            
            // Update text indicators
            document.getElementById('slide-index-indicator').innerText = `Slide ${currentSlide + 1} of ${totalSlides}`;
        }

        // Interactive Pivot Translator Panel
        function translatePivot(id) {
            const data = pivotTranslations[id];
            const titleElement = document.getElementById('pivot-translated-title');
            const descElement = document.getElementById('pivot-translated-desc');
            
            // Add a brief animation flash
            const parent = document.getElementById('pivot-translation-container');
            parent.style.opacity = '0';
            setTimeout(() => {
                titleElement.innerText = data.title;
                descElement.innerText = data.desc;
                parent.style.opacity = '1';
                parent.classList.add('border-emerald-300');
                parent.classList.remove('border-emerald-100');
            }, 200);
        }

        // Timeline History switcher
        function selectHistoryTimeline(key) {
            const data = historyData[key];
            const buttons = ['pinn', 'moz', 'sforce', 'seo'];
            
            // Toggle active classes on buttons
            buttons.forEach(btnKey => {
                const button = document.getElementById(`hist-btn-${btnKey}`);
                const icon = button.querySelector('i');
                if (btnKey === key) {
                    button.className = "w-full text-left p-4 rounded-xl transition-all font-serif font-bold text-lg border bg-white border-brand-rose/30 text-brand-charcoal shadow-sm flex items-center justify-between";
                    icon.className = "fa-solid fa-chevron-right text-xs text-brand-rose opacity-100";
                } else {
                    button.className = "w-full text-left p-4 rounded-xl transition-all font-serif font-bold text-lg border border-transparent text-brand-charcoal/60 hover:bg-white/50 hover:text-brand-charcoal flex items-center justify-between";
                    icon.className = "fa-solid fa-chevron-right text-xs opacity-0";
                }
            });

            // Populate content with brief transition
            const box = document.getElementById('timeline-detail-box');
            box.style.opacity = '0';
            setTimeout(() => {
                document.getElementById('timeline-title-display').innerText = data.title;
                document.getElementById('timeline-desc-display').innerText = data.desc;
                
                // Set role tags
                box.querySelector('span:first-child').innerText = data.role;
                box.querySelector('span:nth-child(2)').innerText = data.type;

                // Set bullet list items
                const listContainer = document.getElementById('timeline-bullets-display');
                listContainer.innerHTML = '';
                data.bullets.forEach(bulletText => {
                    const li = document.createElement('li');
                    li.innerText = bulletText;
                    listContainer.appendChild(li);
                });
                
                box.style.opacity = '1';
            }, 200);
        }

        // Modal triggers
        function openModal() {
            document.getElementById('resume-modal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('resume-modal').classList.add('hidden');
        }

        // --- AI CO-PILOT LOGIC & INTERACTION ---
        function toggleAICoPilot() {
            const drawer = document.getElementById('ai-copilot-drawer');
            aiDrawerOpen = !aiDrawerOpen;
            if (aiDrawerOpen) {
                drawer.classList.remove('translate-x-full');
            } else {
                drawer.classList.add('translate-x-full');
            }
        }

        function setAITab(tab) {
            activeAiTab = tab;
            const tabQa = document.getElementById('ai-tab-qa');
            const tabPitch = document.getElementById('ai-tab-pitch');
            const contentQa = document.getElementById('ai-content-qa');
            const contentPitch = document.getElementById('ai-content-pitch');

            if (tab === 'qa') {
                tabQa.className = "flex-1 py-3 text-center border-b-2 border-brand-rose font-bold text-brand-charcoal";
                tabPitch.className = "flex-1 py-3 text-center border-b-2 border-transparent text-brand-charcoal/60 hover:text-brand-charcoal transition-all";
                contentQa.classList.remove('hidden');
                contentPitch.classList.add('hidden');
            } else {
                tabPitch.className = "flex-1 py-3 text-center border-b-2 border-brand-rose font-bold text-brand-charcoal";
                tabQa.className = "flex-1 py-3 text-center border-b-2 border-transparent text-brand-charcoal/60 hover:text-brand-charcoal transition-all";
                contentPitch.classList.remove('hidden');
                contentQa.classList.add('hidden');
            }
        }

        // Utility: Show Toast Notification
        function showToast(message) {
            const toast = document.getElementById('toast-notif');
            document.getElementById('toast-message').innerText = message;
            toast.classList.remove('hidden');
            setTimeout(() => {
                toast.classList.add('hidden');
            }, 3000);
        }

        // --- GEMINI API CALL (With Backoff and Prompt Engineering) ---
        async function callGeminiAPI(systemPrompt, userQuery) {
            const apiKey = ""; // Canvas Injector handles API Key runtime mapping automatically.
            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-3-flash-preview:generateContent?key=${apiKey}`;

            const payload = {
                contents: [{ parts: [{ text: userQuery }] }],
                systemInstruction: {
                    parts: [{ text: systemPrompt }]
                }
            };

            // Implement exponential backoff for handling potential API throttling
            let retries = 3;
            let delay = 1000;
            while (retries > 0) {
                try {
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    
                    if (response.ok) {
                        const result = await response.json();
                        const textOutput = result?.candidates?.[0]?.content?.parts?.[0]?.text;
                        if (textOutput) return textOutput;
                    }
                } catch (err) {
                    // Fail silently during retries as required by guidelines
                }
                retries--;
                await new Promise(resolve => setTimeout(resolve, delay));
                delay *= 2; // Exponential multiplier
            }
            return "Connection timeout. Please double-check connection settings or try again shortly.";
        }

        // --- SECTION A: Q&A CHATBOT EXECUTION ---
        async function sendChatMessage() {
            const inputField = document.getElementById('ai-chat-input');
            const queryText = inputField.value.trim();
            if (!queryText) return;

            // Clear input immediately and render user bubble
            inputField.value = '';
            appendBubble('user', queryText);

            // Show loading animation bubble
            const loadingBubbleId = appendBubble('ai', 'Thinking...', true);

            // System prompt directing Gemini to acts as Diamond's advocate recruiter/advisor
            const systemPrompt = `
                You are a world-class professional career advocate and portfolio AI assistant representing Diamond Rachel, a Strategic Relationship & Campaign Success Specialist. 
                Your purpose is to explain Diamond's background to corporate recruiters looking to fill Customer Success Manager (CSM), Partner Success Manager, and digital Account Director roles.
                
                Keep your answers highly professional, positive, crisp (under 3-4 sentences), and formatted in clear paragraphs. Frame her Salesforce background as elite consultative workflow experience, and her Pinterest/Mozilla time as premium, post-sales curation and client-growth outcomes.
                
                Always be helpful and advocate for why Diamond's blend of visual brand intuition and sales metrics makes her the ultimate low-friction CSM choice in the Atlanta Area or remotely.
                
                Diamond's Career Context Details:
                ${diamondResumeContext}
            `;

            const aiResponse = await callGeminiAPI(systemPrompt, queryText);
            
            // Remove loading placeholder and update bubble with output
            removeLoadingBubble(loadingBubbleId, aiResponse);
        }

        function appendBubble(role, message, isLoading = false) {
            const container = document.getElementById('ai-chat-history');
            const bubbleId = 'bubble-' + Date.now();
            
            const messageDiv = document.createElement('div');
            messageDiv.id = bubbleId;
            messageDiv.className = `flex items-start space-x-2.5 ${role === 'user' ? 'justify-end' : ''}`;

            if (role === 'user') {
                messageDiv.innerHTML = `
                    <div class="bg-brand-rose text-white p-3 rounded-2xl rounded-tr-none text-xs max-w-[85%]">
                        ${message}
                    </div>
                    <div class="w-7 h-7 bg-brand-charcoal text-brand-cream rounded-full flex items-center justify-center text-xs font-mono font-bold">U</div>
                `;
            } else {
                messageDiv.innerHTML = `
                    <div class="w-7 h-7 bg-brand-rose rounded-full flex items-center justify-center text-white text-xs font-serif font-bold">DR</div>
                    <div class="bg-brand-cream/80 border border-brand-charcoal/5 p-3 rounded-2xl rounded-tl-none text-xs text-brand-charcoal max-w-[85%] ${isLoading ? 'animate-pulse' : ''}">
                        ${message}
                    </div>
                `;
            }

            container.appendChild(messageDiv);
            container.scrollTop = container.scrollHeight;
            return bubbleId;
        }

        function removeLoadingBubble(id, finalMessage) {
            const bubble = document.getElementById(id);
            if (bubble) {
                const textContainer = bubble.querySelector('div:nth-child(2)');
                if (textContainer) {
                    textContainer.classList.remove('animate-pulse');
                    textContainer.innerText = finalMessage;
                }
            }
            const chatHistory = document.getElementById('ai-chat-history');
            chatHistory.scrollTop = chatHistory.scrollHeight;
        }

        function submitQuickQuery(question) {
            document.getElementById('ai-chat-input').value = question;
            sendChatMessage();
        }

        // --- SECTION B: OUTREACH & COVER LETTER PITCH GENERATOR ---
        async function generateCustomPitch() {
            const companyInput = document.getElementById('pitch-company').value.trim();
            const titleInput = document.getElementById('pitch-title').value.trim();
            const focusInput = document.getElementById('pitch-focus').value;
            const outputText = document.getElementById('pitch-output-text');

            if (!companyInput || !titleInput) {
                showToast("Please enter target Company and Job Title.");
                return;
            }

            outputText.innerText = "Crafting custom narrative pivot... Please hold...";
            outputText.classList.add('animate-pulse');

            const systemPrompt = `
                You are a senior executive career coach and resume writer. Draft a brief, high-conversion LinkedIn outreach message or cover letter intro (approx 100-150 words) written from Diamond Rachel's perspective.
                
                The target company is "${companyInput}" and the target job title is "${titleInput}".
                Align the pitch around her target role pivot towards Post-Sales Relationship Retention, Account Management, or Partner Success.
                
                Use a tone that is highly polished, professional, warm, and confident. Downplay traditional cold outbound metrics and emphasize her collaborative workflow stewardship.
                
                Based on focus selection:
                - "onboarding": Highlight Pinterest creative partner launch systems.
                - "retention": Highlight Mozilla publisher relationship management.
                - "seo": Highlight her analytical SEO strategy/advisory capacity.
                - "all": Consolidate her multi-platform brand metrics with aesthetics.
                
                Reference Diamond's Background context:
                ${diamondResumeContext}
            `;

            const promptQuery = `Create a custom, high-converting outreach message targeting a role at ${companyInput} as a ${titleInput} under the focus profile: ${focusInput}.`;
            const pitchOutput = await callGeminiAPI(systemPrompt, promptQuery);

            outputText.classList.remove('animate-pulse');
            outputText.innerText = pitchOutput;
        }

        // Copy generated message to clipboard safely
        function copyGeneratedPitch() {
            const textToCopy = document.getElementById('pitch-output-text').innerText;
            if (!textToCopy || textToCopy.includes("A custom crafted")) return;

            // Use executive command helper to avoid iframe cross-origin restrictions
            const textEl = document.createElement('textarea');
            textEl.value = textToCopy;
            document.body.appendChild(textEl);
            textEl.select();
            document.execCommand('copy');
            document.body.removeChild(textEl);

            showToast("Copied outreach pitch to clipboard!");
        }
    </script>

</body>
</html>
