<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pradyot Pritam | Quantum Computing Specialist</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* slate-50 */
        }
        .quantum-accent {
            color: #4f46e5; /* indigo-600 */
        }
        .quantum-bg {
            background-color: #4f46e5; /* indigo-600 */
        }
        .quantum-border {
            border-color: #4f46e5; /* indigo-600 */
        }
        .tab-active {
            background-color: #4f46e5; /* indigo-600 */
            color: #ffffff;
        }
        .tab-inactive {
            background-color: #eef2ff; /* indigo-100 */
            color: #3730a3; /* indigo-800 */
        }
        .content-pane {
            display: none;
        }
        .content-pane.active {
            display: grid;
        }
        .algo-pill-active {
            background-color: #3730a3; /* indigo-800 */
            color: #ffffff;
            transform: scale(1.05);
        }
    </style>
    <!-- Chosen Palette: "Quantum Calm" (Base: Slate-50, Text: Slate-800, Accent: Indigo-600) -->
    <!-- Application Structure Plan: A single-page, scrolling portfolio designed to guide visitors from a high-level introduction to specific skills and a clear call to action. The structure is: 1) A Hero section for immediate impact. 2) An interactive "Expertise Explorer" with tabs for Platforms, Algorithms, and Applications, turning static lists into an engaging experience. 3) A "Collaboration" section to state goals clearly. 4) A final "Contact" footer. This structure is more user-friendly and engaging than a linear document, allowing users to explore areas of interest non-linearly. -->
    <!-- Visualization & Content Choices: The core interactive element is the "Expertise Explorer." Report Info: Lists of platforms, algorithms, and technologies. -> Goal: Organize & Inform. -> Viz/Method: A tabbed interface built with HTML/CSS/JS. Inside the "Algorithms" tab, clickable "pills" update a description area. -> Interaction: JS-driven showing/hiding of content panes and updating text content based on user clicks. -> Justification: This transforms static lists from the README into an interactive demonstration of expertise, enhancing user engagement. -> Library/Method: Vanilla JS for DOM manipulation. No charts (Chart.js/Plotly) are used as the source material is qualitative with no quantitative data to visualize. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
</head>
<body class="text-slate-800">

    <!-- Header & Hero Section -->
    <header id="home" class="w-full min-h-screen flex flex-col items-center justify-center text-center p-4 bg-slate-100">
        <div class="w-48 h-48 mb-6">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbDB6dHU1dHE1a3J2Z3g4eGd2bWIwN3ZzZ3N2c3JmMm5tZ3hpZGRzeCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/M9gbBdgwXbA2s/giphy.gif" alt="Animated atom" class="w-full h-full object-contain">
        </div>
        <h1 class="text-4xl md:text-6xl font-extrabold mb-2">Hi, I’m Pradyot! 👋</h1>
        <h2 class="text-xl md:text-3xl font-semibold quantum-accent">⚛️ Bridging the Quantum Realm with Real-World Impact ⚛️</h2>
        <p class="max-w-3xl mx-auto mt-4 text-slate-600">
            I'm deeply immersed in the fascinating world of Quantum Computing, exploring cutting-edge Quantum Algorithms, and pioneering Optimization techniques for both fundamental physics challenges and complex real-world problems.
        </p>
        <a href="#contact" class="mt-8 px-8 py-3 rounded-full quantum-bg text-white font-bold text-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
            Get in Touch
        </a>
    </header>

    <main class="max-w-7xl mx-auto p-4 md:p-8">

        <!-- Expertise Explorer Section -->
        <section id="expertise" class="my-16 scroll-mt-20">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold">Expertise Explorer</h2>
                <p class="mt-2 text-slate-600 max-w-2xl mx-auto">Explore my technical capabilities across platforms, algorithms, and key application areas. Click the tabs below to navigate.</p>
            </div>

            <!-- Tabs -->
            <div id="tabs-container" class="flex flex-wrap justify-center gap-2 md:gap-4 mb-8">
                <button data-tab="platforms" class="tab-btn px-6 py-2 font-semibold rounded-full transition-all duration-300 tab-active">Platforms & Hardware</button>
                <button data-tab="algorithms" class="tab-btn px-6 py-2 font-semibold rounded-full transition-all duration-300 tab-inactive">Algorithmic Toolkit</button>
                <button data-tab="applications" class="tab-btn px-6 py-2 font-semibold rounded-full transition-all duration-300 tab-inactive">Application Areas</button>
            </div>

            <!-- Content Panes -->
            <div id="content-container" class="mt-4">
                <!-- Platforms Pane -->
                <div id="platforms-content" class="content-pane active gap-8 md:grid-cols-3">
                    <div class="bg-white p-6 rounded-lg shadow-md border-t-4 quantum-border">
                        <h3 class="text-xl font-bold mb-2">Digital Gate-Based</h3>
                        <p class="text-slate-600">Actively developing solutions and running experiments on gate-based quantum hardware, with hands-on experience using <strong class="quantum-accent">IBM QPUs</strong>.</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md border-t-4 quantum-border">
                        <h3 class="text-xl font-bold mb-2">Analog Quantum Computing</h3>
                        <p class="text-slate-600">Leveraging analog platforms like <strong class="quantum-accent">D-Wave's quantum annealers</strong> to tackle complex optimization problems, particularly those rooted in physics.</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md border-t-4 quantum-border">
                        <h3 class="text-xl font-bold mb-2">Accelerated Computing</h3>
                        <p class="text-slate-600">Expanding into <strong class="quantum-accent">GPU computing and NVIDIA CUDA</strong> to accelerate high-performance quantum simulations and workflows, pushing the boundaries of what's possible.</p>
                    </div>
                </div>

                <!-- Algorithms Pane -->
                <div id="algorithms-content" class="content-pane gap-8 md:grid-cols-3">
                    <div class="md:col-span-1">
                        <h3 class="text-xl font-bold mb-4">Click an Algorithm</h3>
                        <div id="algo-pills" class="flex flex-wrap gap-2">
                            <!-- Pills will be generated by JS -->
                        </div>
                    </div>
                    <div class="md:col-span-2 bg-white p-6 rounded-lg shadow-md min-h-[150px]">
                         <h4 id="algo-title" class="text-lg font-bold quantum-accent">Select an Algorithm</h4>
                         <p id="algo-description" class="text-slate-600 mt-2">Click on one of the algorithm pills to see a brief description of its purpose and application here.</p>
                    </div>
                </div>

                <!-- Applications Pane -->
                <div id="applications-content" class="content-pane gap-8 md:grid-cols-2">
                     <div class="bg-white p-6 rounded-lg shadow-md border-t-4 quantum-border">
                        <h3 class="text-xl font-bold mb-2">Quantum Optimization</h3>
                        <p class="text-slate-600">Pioneering optimization techniques using quantum principles to solve complex real-world and fundamental physics challenges that are intractable for classical computers.</p>
                    </div>
                     <div class="bg-white p-6 rounded-lg shadow-md border-t-4 quantum-border">
                        <h3 class="text-xl font-bold mb-2">Quantum Machine Learning</h3>
                        <p class="text-slate-600">Actively integrating my algorithmic toolkit into cutting-edge <strong class="quantum-accent">Quantum Machine Learning (QML)</strong> techniques to explore new frontiers in artificial intelligence.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Collaboration Section -->
        <section id="collaboration" class="my-16 scroll-mt-20">
            <div class="bg-white rounded-lg shadow-lg p-8 md:p-12 text-center">
                 <h2 class="text-3xl md:text-4xl font-bold">💞️ Let's Innovate Together!</h2>
                 <p class="mt-4 text-slate-600 max-w-3xl mx-auto">I'm eagerly looking to collaborate on industry and research-related projects that push the boundaries of quantum science and optimization. If you're working on challenges in the following areas, I would love to connect!</p>
                 <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 mt-8 text-left">
                     <div class="bg-slate-50 p-4 rounded-md">🖥️ Quantum Hardware</div>
                     <div class="bg-slate-50 p-4 rounded-md">🔢 Algorithm Development</div>
                     <div class="bg-slate-50 p-4 rounded-md">🤖 Quantum Machine Learning</div>
                     <div class="bg-slate-50 p-4 rounded-md">🚀 GPU Acceleration</div>
                 </div>
            </div>
        </section>

    </main>
    
    <!-- Footer -->
    <footer id="contact" class="bg-slate-800 text-white scroll-mt-20">
        <div class="max-w-7xl mx-auto p-8 md:p-12 text-center">
            <h2 class="text-2xl md:text-3xl font-bold">Get in Touch</h2>
            <p class="mt-2 max-w-xl mx-auto text-slate-300">I'm always open to discussing new ideas and potential collaborations. Let's connect and help shape the future with Quantum AI!</p>
            <a href="mailto:pradyotpritam@gmail.com" class="inline-block mt-6 px-8 py-3 rounded-full quantum-bg text-white font-bold text-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
                pradyotpritam@gmail.com
            </a>
            <div class="mt-8 text-slate-400">
                <p>Pronouns: He/Him</p>
                <p class="mt-1">⚡ Fun fact: I'm passionate about bridging the gap between theoretical physics and practical applications through quantum advancements.</p>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const tabsContainer = document.getElementById('tabs-container');
            const contentContainer = document.getElementById('content-container');
            const tabButtons = tabsContainer.querySelectorAll('.tab-btn');
            const contentPanes = contentContainer.querySelectorAll('.content-pane');

            const algoData = {
                'VQE': { title: 'Variational Quantum Eigensolver (VQE)', description: 'A hybrid quantum-classical algorithm used to find the minimum eigenvalue of a matrix, primarily for problems in quantum chemistry and optimization.' },
                'QPE': { title: 'Quantum Phase Estimation (QPE)', description: 'A core quantum algorithm used to estimate the phase of an eigenvector of a unitary operator. It is a key subroutine in many other algorithms, like Shor\'s algorithm.' },
                'HHL': { title: 'Harrow-Hassidim-Lloyd (HHL)', description: 'A quantum algorithm for solving systems of linear equations. It can offer an exponential speedup over classical algorithms under specific conditions.' },
                'QAE': { title: 'Quantum Amplitude Estimation (QAE)', description: 'A quantum algorithm that provides a quadratic speedup for many problems that can be cast as estimating an amplitude, such as Monte Carlo methods.' },
                'QSCI': { title: 'Quantum-inspired Classical Inference (QSCI)', description: 'A technique that applies principles from quantum mechanics to enhance classical machine learning and inference models.' },
                'VQLS': { title: 'Variational Quantum Linear Solver (VQLS)', description: 'A variational hybrid algorithm for solving linear systems of equations, often more suitable for near-term, noisy quantum devices than HHL.' },
                'VarQA': { title: 'Variational Quantum Algorithm (VarQA)', description: 'A general class of algorithms that use a classical optimizer to train a parameterized quantum circuit, applicable to a wide range of problems.' },
            };
            
            const algoPillsContainer = document.getElementById('algo-pills');
            const algoTitleEl = document.getElementById('algo-title');
            const algoDescriptionEl = document.getElementById('algo-description');
            
            Object.keys(algoData).forEach(key => {
                const pill = document.createElement('button');
                pill.className = 'algo-pill px-4 py-1.5 text-sm font-semibold rounded-full transition-all duration-300 bg-slate-200 text-slate-700 hover:bg-slate-300';
                pill.textContent = key;
                pill.dataset.algo = key;
                algoPillsContainer.appendChild(pill);
            });
            const algoPills = algoPillsContainer.querySelectorAll('.algo-pill');
            
            tabsContainer.addEventListener('click', (e) => {
                const targetButton = e.target.closest('.tab-btn');
                if (!targetButton) return;

                const tabId = targetButton.dataset.tab;

                tabButtons.forEach(btn => {
                    btn.classList.remove('tab-active');
                    btn.classList.add('tab-inactive');
                });
                targetButton.classList.add('tab-active');
                targetButton.classList.remove('tab-inactive');

                contentPanes.forEach(pane => {
                    pane.classList.remove('active');
                });
                document.getElementById(`${tabId}-content`).classList.add('active');
            });
            
            algoPillsContainer.addEventListener('click', (e) => {
                 const targetPill = e.target.closest('.algo-pill');
                 if (!targetPill) return;
                 
                 const algoKey = targetPill.dataset.algo;
                 const data = algoData[algoKey];
                 
                 algoPills.forEach(pill => pill.classList.remove('algo-pill-active'));
                 targetPill.classList.add('algo-pill-active');
                 
                 algoTitleEl.textContent = data.title;
                 algoDescriptionEl.textContent = data.description;
            });
        });
    </script>

</body>
</html>
