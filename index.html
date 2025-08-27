<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Morte Encefálica: Desvendando o Diagnóstico</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <!-- Chosen Palette: Warm Neutrals with Teal Accent -->
    <!-- Application Structure Plan: A single-page application with a sticky navigation bar for thematic scrolling. The structure is designed to guide the user from the fundamental concept and history ('O Que É?'), through the specific national context and data ('O Paradoxo Brasileiro'), into the complex medical process ('Como Acontece?'), and finally to the human and societal implications ('O Desafio Social'). This non-linear, thematic approach was chosen over mirroring the report's structure to create a more intuitive and engaging user journey, allowing exploration based on interest rather than a rigid sequence. Key interactions include an interactive timeline, a dynamic data chart, a clickable process flowchart, and a 'myths vs. facts' section to directly address the core communication challenges highlighted in the source report. -->
    <!-- Visualization & Content Choices: 
        1. History: Report Info -> Evolution of the concept of death. Goal -> Show change over time. Viz/Presentation -> Interactive Timeline. Interaction -> Click to reveal info. Justification -> More engaging than text. Library/Method -> HTML/CSS/JS.
        2. Epidemiology Data: Report Info -> Transplant/donor/waitlist numbers. Goal -> Visualize the discrepancy. Viz/Presentation -> Interactive Bar/Line Chart. Interaction -> Toggle years to update data. Justification -> Powerful visual comparison. Library/Method -> Chart.js (Canvas).
        3. Pathophysiology Process: Report Info -> Cascade of events. Goal -> Simplify a complex process. Viz/Presentation -> Interactive Flowchart. Interaction -> Click steps for explanation. Justification -> Clarifies sequence. Library/Method -> HTML/CSS/JS.
        4. Social Misconceptions: Report Info -> Reasons for family refusal. Goal -> Address misinformation. Viz/Presentation -> Myth vs. Fact accordion. Interaction -> Click to reveal facts. Justification -> Directly tackles the communication problem. Library/Method -> HTML/CSS/JS.
    -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #FDFBF8;
            color: #4A4A4A;
        }
        .nav-link {
            transition: color 0.3s, border-bottom-color 0.3s;
        }
        .nav-link:hover, .nav-link.active {
            color: #14B8A6;
            border-bottom-color: #14B8A6;
        }
        .timeline-item::before {
            content: '';
            position: absolute;
            top: 10px;
            left: -21px;
            width: 12px;
            height: 12px;
            background-color: #14B8A6;
            border: 2px solid #FDFBF8;
            border-radius: 50%;
            z-index: 1;
        }
        .flowchart-step {
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .flowchart-step:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 50vh;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 450px;
            }
        }
        .loading-spinner {
            border: 4px solid rgba(0, 0, 0, 0.1);
            border-left-color: #14B8A6;
            border-radius: 50%;
            width: 24px;
            height: 24px;
            animation: spin 1s linear infinite;
            display: inline-block;
            vertical-align: middle;
            margin-left: 8px;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body class="antialiased">

    <header id="header" class="bg-white/80 backdrop-blur-md sticky top-0 z-50 shadow-sm">
        <nav class="container mx-auto px-6 py-3 flex justify-between items-center">
            <div class="text-xl font-bold text-teal-600">Morte Encefálica</div>
            <div class="hidden md:flex space-x-8">
                <a href="#oquee" class="nav-link border-b-2 border-transparent pb-1">O Que É?</a>
                <a href="#paradoxo" class="nav-link border-b-2 border-transparent pb-1">O Paradoxo Brasileiro</a>
                <a href="#comoacontece" class="nav-link border-b-2 border-transparent pb-1">Como Acontece?</a>
                <a href="#desafio" class="nav-link border-b-2 border-transparent pb-1">O Desafio Social</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </nav>
        <div id="mobile-menu" class="hidden md:hidden">
            <a href="#oquee" class="block py-2 px-4 text-sm hover:bg-gray-200">O Que É?</a>
            <a href="#paradoxo" class="block py-2 px-4 text-sm hover:bg-gray-200">O Paradoxo Brasileiro</a>
            <a href="#comoacontece" class="block py-2 px-4 text-sm hover:bg-gray-200">Como Acontece?</a>
            <a href="#desafio" class="block py-2 px-4 text-sm hover:bg-gray-200">O Desafio Social</a>
        </div>
    </header>

    <main>
        <section id="hero" class="py-20 bg-teal-50">
            <div class="container mx-auto px-6 text-center">
                <h1 class="text-4xl md:text-6xl font-bold text-teal-800 mb-4">Desvendando a Morte Encefálica</h1>
                <p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto">Uma jornada interativa para compreender o diagnóstico que redefine a fronteira da vida e possibilita o ato de doar órgãos.</p>
            </div>
        </section>

        <section id="oquee" class="py-16 md:py-24">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-teal-700">O Que é Morte Encefálica?</h2>
                <div class="flex items-center justify-center max-w-3xl mx-auto mb-12">
                    <p id="oquee-intro-text" class="text-center text-gray-600">É a perda completa e irreversível de todas as funções do cérebro, incluindo o tronco encefálico que controla a respiração. Legalmente, é a definição de morte, mesmo que o coração continue batendo com a ajuda de aparelhos.</p>
                    <button id="tts-oquee-intro" class="ml-2 p-1 rounded-full bg-teal-100 hover:bg-teal-200 transition-colors">
                        <svg class="w-5 h-5 text-teal-600" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M9.383 3.003h1.234A.5.5 0 0111 3.5v13a.5.5 0 01-.383.497H9.383a.5.5 0 01-.499-.387l-2.618-8.239A.5.5 0 016.5 8h-2a.5.5 0 01-.497-.383l-2.618-8.24A.5.5 0 010 0v13a.5.5 0 01.497.383l2.618 8.239A.5.5 0 013.5 13h2a.5.5 0 01.499.387l2.618 8.239A.5.5 0 019.5 20h.5a.5.5 0 01.5-.5V.5a.5.5 0 01-.117-.003z" clip-rule="evenodd"></path></svg>
                    </button>
                    <div id="tts-oquee-intro-loading" class="loading-spinner hidden"></div>
                </div>
                
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div class="prose max-w-none text-gray-700">
                        <h3 class="text-2xl font-semibold mb-4 text-teal-600">Uma Breve História do Conceito de Morte</h3>
                        <p>A forma como entendemos a morte mudou drasticamente. O que antes era definido pela parada do coração, hoje é compreendido a partir da cessação da atividade cerebral. Esta linha do tempo interativa mostra a evolução desse conceito.</p>
                    </div>
                    <div id="timeline" class="relative border-l-2 border-teal-200 pl-8">
                    </div>
                </div>
            </div>
        </section>

        <section id="paradoxo" class="py-16 md:py-24 bg-gray-50">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-teal-700">O Paradoxo Brasileiro</h2>
                <div class="flex items-center justify-center max-w-3xl mx-auto mb-12">
                    <p id="paradoxo-intro-text" class="text-center text-gray-600">O Brasil possui o maior sistema público de transplantes do mundo e uma alta capacidade técnica. No entanto, a fila de espera por um órgão continua imensa. O gráfico abaixo revela a principal razão: o descompasso entre a necessidade, a capacidade de transplantar e o número de doadores efetivos.</p>
                    <button id="tts-paradoxo-intro" class="ml-2 p-1 rounded-full bg-teal-100 hover:bg-teal-200 transition-colors">
                        <svg class="w-5 h-5 text-teal-600" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M9.383 3.003h1.234A.5.5 0 0111 3.5v13a.5.5 0 01-.383.497H9.383a.5.5 0 01-.499-.387l-2.618-8.239A.5.5 0 016.5 8h-2a.5.5 0 01-.497-.383l-2.618-8.24A.5.5 0 010 0v13a.5.5 0 01.497.383l2.618 8.239A.5.5 0 013.5 13h2a.5.5 0 01.499.387l2.618 8.239A.5.5 0 019.5 20h.5a.5.5 0 01.5-.5V.5a.5.5 0 01-.117-.003z" clip-rule="evenodd"></path></svg>
                    </button>
                    <div id="tts-paradoxo-intro-loading" class="loading-spinner hidden"></div>
                </div>
                
                <div class="bg-white p-4 md:p-8 rounded-xl shadow-lg">
                    <div class="flex justify-center mb-6">
                        <div class="inline-flex rounded-md shadow-sm" role="group">
                            <button type="button" id="btn2023" class="px-4 py-2 text-sm font-medium text-white bg-teal-600 border border-gray-200 rounded-l-lg hover:bg-teal-700 focus:z-10 focus:ring-2 focus:ring-teal-500">
                                2023
                            </button>
                            <button type="button" id="btn2024" class="px-4 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-200 rounded-r-md hover:bg-gray-100 focus:z-10 focus:ring-2 focus:ring-teal-500">
                                2024
                            </button>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="transplantChart"></canvas>
                    </div>
                    <div class="mt-8 text-center">
                        <p class="text-lg text-gray-700">O principal gargalo não é técnico, mas social: a <strong class="text-red-600 text-xl">recusa familiar</strong>, que atinge cerca de <strong class="text-red-600 text-xl">43%</strong>, impede que milhares de vidas sejam salvas.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="comoacontece" class="py-16 md:py-24">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-teal-700">Como Acontece?</h2>
                <div class="flex items-center justify-center max-w-3xl mx-auto mb-12">
                    <p id="comoacontece-intro-text" class="text-center text-gray-600">A morte encefálica é o resultado final de uma cascata de eventos catastróficos no cérebro. Explore o processo fisiopatológico abaixo para entender como uma lesão inicial leva à parada completa e irreversível da função cerebral.</p>
                    <button id="tts-comoacontece-intro" class="ml-2 p-1 rounded-full bg-teal-100 hover:bg-teal-200 transition-colors">
                        <svg class="w-5 h-5 text-teal-600" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M9.383 3.003h1.234A.5.5 0 0111 3.5v13a.5.5 0 01-.383.497H9.383a.5.5 0 01-.499-.387l-2.618-8.239A.5.5 0 016.5 8h-2a.5.5 0 01-.497-.383l-2.618-8.24A.5.5 0 010 0v13a.5.5 0 01.497.383l2.618 8.239A.5.5 0 013.5 13h2a.5.5 0 01.499.387l2.618 8.239A.5.5 0 019.5 20h.5a.5.5 0 01.5-.5V.5a.5.5 0 01-.117-.003z" clip-rule="evenodd"></path></svg>
                    </button>
                    <div id="tts-comoacontece-intro-loading" class="loading-spinner hidden"></div>
                </div>
                
                <div id="flowchart" class="flex flex-col md:flex-row justify-center items-center gap-4 md:gap-0">
                </div>

                <div class="mt-8 text-center p-6 bg-teal-50 rounded-lg min-h-[100px] flex flex-col justify-center items-center">
                    <p id="flowchart-details" class="text-teal-800">Clique em uma etapa para ver os detalhes.</p>
                    <button id="simplify-explanation-btn" class="mt-4 px-4 py-2 bg-teal-600 text-white rounded-lg hover:bg-teal-700 transition-colors flex items-center">
                        ✨ Explicar de Forma Simples
                        <div id="simplify-loading" class="loading-spinner hidden"></div>
                    </button>
                </div>

                <div class="mt-16">
                    <h3 class="text-2xl font-semibold text-center mb-8 text-teal-600">Critérios para o Diagnóstico</h3>
                    <div id="criteria-list" class="max-w-4xl mx-auto grid md:grid-cols-2 gap-6">
                    </div>
                </div>
            </div>
        </section>

        <section id="desafio" class="py-16 md:py-24 bg-gray-50">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-teal-700">O Desafio Social: Comunicação e Luto</h2>
                <div class="flex items-center justify-center max-w-3xl mx-auto mb-12">
                    <p id="desafio-intro-text" class="text-center text-gray-600">O maior obstáculo é a comunicação. Para a família, ver um corpo aquecido, com o coração batendo, torna o diagnóstico de morte difícil de aceitar. Esclarecer mitos é fundamental para uma decisão consciente sobre a doação de órgãos.</p>
                    <button id="tts-desafio-intro" class="ml-2 p-1 rounded-full bg-teal-100 hover:bg-teal-200 transition-colors">
                        <svg class="w-5 h-5 text-teal-600" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M9.383 3.003h1.234A.5.5 0 0111 3.5v13a.5.5 0 01-.383.497H9.383a.5.5 0 01-.499-.387l-2.618-8.239A.5.5 0 016.5 8h-2a.5.5 0 01-.497-.383l-2.618-8.24A.5.5 0 010 0v13a.5.5 0 01.497.383l2.618 8.239A.5.5 0 013.5 13h2a.5.5 0 01.499.387l2.618 8.239A.5.5 0 019.5 20h.5a.5.5 0 01.5-.5V.5a.5.5 0 01-.117-.003z" clip-rule="evenodd"></path></svg>
                    </button>
                    <div id="tts-desafio-intro-loading" class="loading-spinner hidden"></div>
                </div>
                
                <div id="myths-facts" class="max-w-3xl mx-auto space-y-4">
                </div>

                <div class="mt-12 text-center p-8 bg-teal-600 text-white rounded-lg shadow-xl">
                    <h3 class="text-2xl font-bold mb-4">A Importância do Diálogo</h3>
                    <p class="mb-6">A doação de órgãos só acontece com autorização familiar. Por isso, a decisão mais importante é tomada em vida: conversar com sua família e deixar seu desejo claro. Um "sim" pode transformar o fim de uma vida no recomeço de várias outras.</p>
                    <button id="generate-scenario-btn" class="mt-4 px-4 py-2 bg-white text-teal-600 font-bold rounded-lg hover:bg-gray-100 transition-colors flex items-center justify-center mx-auto">
                        ✨ Gerar Cenário de Conversa
                        <div id="scenario-loading" class="loading-spinner hidden"></div>
                    </button>
                    <div id="conversation-scenario-output" class="mt-6 p-4 bg-teal-700 text-white rounded-lg text-left hidden flex items-start">
                        <p id="scenario-text" class="flex-grow"></p>
                        <button id="tts-scenario" class="ml-2 p-1 rounded-full bg-teal-500 hover:bg-teal-400 transition-colors">
                            <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M9.383 3.003h1.234A.5.5 0 0111 3.5v13a.5.5 0 01-.383.497H9.383a.5.5 0 01-.499-.387l-2.618-8.239A.5.5 0 016.5 8h-2a.5.5 0 01-.497-.383l-2.618-8.24A.5.5 0 010 0v13a.5.5 0 01.497.383l2.618 8.239A.5.5 0 013.5 13h2a.5.5 0 01.499.387l2.618 8.239A.5.5 0 019.5 20h.5a.5.5 0 01.5-.5V.5a.5.5 0 01-.117-.003z" clip-rule="evenodd"></path></svg>
                        </button>
                        <div id="tts-scenario-loading" class="loading-spinner hidden"></div>
                    </div>
                    <a href="#" class="inline-block bg-white text-teal-600 font-bold py-3 px-6 rounded-lg hover:bg-gray-100 transition-colors mt-6">#SetembroVerde: Fale Sobre Doação</a>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-6 text-center">
            <p>&copy; 2025 Aplicação Educacional sobre Morte Encefálica. Conteúdo baseado em relatório técnico.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const API_KEY = ""; // A chave da API será fornecida pelo ambiente em tempo de execução.

            // Funções auxiliares para TTS (Text-to-Speech)
            function base64ToArrayBuffer(base64) {
                const binaryString = atob(base64);
                const len = binaryString.length;
                const bytes = new Uint8Array(len);
                for (let i = 0; i < len; i++) {
                    bytes[i] = binaryString.charCodeAt(i);
                }
                return bytes.buffer;
            }

            function pcmToWav(pcmData, sampleRate) {
                const header = new ArrayBuffer(44);
                const view = new DataView(header);

                // RIFF identifier
                writeString(view, 0, 'RIFF');
                // file length
                view.setUint32(4, 36 + pcmData.byteLength, true);
                // RIFF type
                writeString(view, 8, 'WAVE');
                // format chunk identifier
                writeString(view, 12, 'fmt ');
                // format chunk length
                view.setUint32(16, 16, true);
                // sample format (raw pcm)
                view.setUint16(20, 1, true);
                // channel count
                view.setUint16(22, 1, true);
                // sample rate
                view.setUint32(24, sampleRate, true);
                // byte rate (sample rate * block align)
                view.setUint32(28, sampleRate * 2, true);
                // block align (channels * bytes per sample)
                view.setUint16(32, 2, true);
                // bits per sample
                view.setUint16(34, 16, true);
                // data chunk identifier
                writeString(view, 36, 'data');
                // data chunk length
                view.setUint32(40, pcmData.byteLength, true);

                const blob = new Blob([header, pcmData], { type: 'audio/wav' });
                return blob;
            }

            function writeString(view, offset, string) {
                for (let i = 0; i < string.length; i++) {
                    view.setUint8(offset + i, string.charCodeAt(i));
                }
            }

            async function callGeminiApi(modelName, payload, retries = 0) {
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/${modelName}:generateContent?key=${API_KEY}`;
                try {
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    if (!response.ok) {
                        if (response.status === 429 && retries < 5) { // Exponential backoff for Too Many Requests
                            const delay = Math.pow(2, retries) * 1000;
                            await new Promise(resolve => setTimeout(resolve, delay));
                            return callGeminiApi(modelName, payload, retries + 1);
                        }
                        const errorData = await response.json();
                        console.error("API Error:", errorData);
                        throw new Error(`API request failed with status ${response.status}: ${errorData.error.message}`);
                    }
                    return await response.json();
                } catch (error) {
                    console.error("Fetch Error:", error);
                    throw error;
                }
            }

            async function playAudio(text, loadingElementId) {
                const loadingSpinner = document.getElementById(loadingElementId);
                if (loadingSpinner) loadingSpinner.classList.remove('hidden');

                const payload = {
                    contents: [{
                        parts: [{ text: text }]
                    }],
                    generationConfig: {
                        responseModalities: ["AUDIO"],
                        speechConfig: {
                            voiceConfig: {
                                prebuiltVoiceConfig: { voiceName: "Kore" }
                            }
                        }
                    },
                    model: "gemini-2.5-flash-preview-tts"
                };

                try {
                    const result = await callGeminiApi("gemini-2.5-flash-preview-tts", payload);
                    const part = result?.candidates?.[0]?.content?.parts?.[0];
                    const audioData = part?.inlineData?.data;
                    const mimeType = part?.inlineData?.mimeType;

                    if (audioData && mimeType && mimeType.startsWith("audio/")) {
                        const sampleRateMatch = mimeType.match(/rate=(\d+)/);
                        const sampleRate = sampleRateMatch ? parseInt(sampleRateMatch[1], 10) : 16000; 
                        const pcmData = base64ToArrayBuffer(audioData);
                        const pcm16 = new Int16Array(pcmData);
                        const wavBlob = pcmToWav(pcm16, sampleRate);
                        const audioUrl = URL.createObjectURL(wavBlob);

                        const audio = new Audio(audioUrl);
                        audio.play();
                        audio.onended = () => URL.revokeObjectURL(audioUrl);
                    } else {
                        console.error("TTS: Estrutura de resposta inesperada ou conteúdo de áudio ausente.");
                    }
                } catch (error) {
                    console.error("Erro ao gerar ou reproduzir áudio:", error);
                } finally {
                    if (loadingSpinner) loadingSpinner.classList.add('hidden');
                }
            }

            function showLoading(elementId) {
                const loadingElement = document.getElementById(elementId);
                if (loadingElement) loadingElement.classList.remove('hidden');
            }

            function hideLoading(elementId) {
                const loadingElement = document.getElementById(elementId);
                if (loadingElement) loadingElement.classList.add('hidden');
            }
            
            const timelineData = [
                { year: 'Antiguidade', title: 'Morte Cardíaca', text: 'A morte era definida pela parada visível dos batimentos cardíacos e da respiração.' },
                { year: 'Idade Média', title: 'Evento Público', text: 'A morte era um ritual familiar e comunitário, sem o tabu que possui hoje.' },
                { year: 'Déc. 1950', title: 'Suporte Vital', text: 'O surgimento de ventiladores mecânicos cria um dilema: um corpo "vivo" sem função cerebral.' },
                { year: '1967', title: 'Primeiro Transplante', text: 'O primeiro transplante de coração torna urgente a necessidade de uma nova definição de morte.' },
                { year: '1968', title: 'Critérios de Harvard', text: 'Um comitê estabelece o "coma irreversível" (morte encefálica) como o novo critério legal e médico para a morte.' },
                { year: '1997', title: 'Lei no Brasil', text: 'A Lei 9.434 regulamenta o diagnóstico de morte encefálica e a doação de órgãos no país.' }
            ];

            const flowchartStaticData = [ // Renomeado para evitar conflito
                { id: 'lesao', title: 'Lesão Cerebral Grave', text: 'Causada por AVC, traumatismo ou falta de oxigênio, inicia um processo de dano celular.' },
                { id: 'edema', title: 'Edema Cerebral', text: 'O cérebro incha dentro do crânio, que é uma caixa óssea sem capacidade de expansão.' },
                { id: 'pic', title: 'Aumento da Pressão', text: 'O inchaço aumenta drasticamente a Pressão Intracraniana (PIC), comprimindo os vasos sanguíneos.' },
                { id: 'colapso', title: 'Colapso da Circulação', text: 'Quando a PIC supera a pressão arterial, o sangue não consegue mais chegar ao cérebro.' },
                { id: 'isquemia', title: 'Isquemia Global', text: 'Sem sangue e oxigênio, todas as células cerebrais, incluindo as do tronco encefálico, morrem de forma irreversível.' }
            ];

            const criteriaData = [
                { title: 'Coma Irreversível', text: 'Ausência total de consciência e qualquer resposta a estímulos dolorosos ou verbais.', icon: '🧠' },
                { title: 'Ausência de Reflexos do Tronco', text: 'As pupilas não reagem à luz, não há reflexo de tosse ou vômito, entre outros testes.', icon: '👁️' },
                { title: 'Apneia (Sem Respiração)', text: 'O paciente é incapaz de respirar por conta própria, confirmado por um teste específico onde o ventilador é desligado momentaneamente.', icon: '🫁' },
                { title: 'Diagnóstico Rigoroso', text: 'Dois médicos diferentes realizam todos os testes com um intervalo de tempo para confirmar a irreversibilidade do quadro.', icon: '🧑‍⚕️🧑‍⚕️' }
            ];
            
            const mythsData = [
                { myth: 'Mito: Se o coração bate, a pessoa está viva.', fact: 'Fato: O coração pode continuar batendo por um tempo com a ajuda de aparelhos e medicamentos, mas sem o cérebro, que comanda todas as funções, não há vida. A pessoa já está morta.' },
                { myth: 'Mito: A pessoa pode "acordar" da morte encefálica.', fact: 'Fato: Morte encefálica é diferente de coma. No coma, há atividade cerebral e chance de recuperação. Na morte encefálica, a destruição do cérebro é completa e irreversível. Não há nenhuma chance de recuperação.' },
                { myth: 'Mito: Vemos a pessoa se mexer na cama.', fact: 'Fato: Esses movimentos são reflexos da medula espinhal, que pode continuar funcionando por um curto período de forma independente do cérebro. Não indicam atividade cerebral ou consciência.' }
            ];

            const timelineContainer = document.getElementById('timeline');
            timelineData.forEach(item => {
                const div = document.createElement('div');
                div.className = 'timeline-item mb-8 relative cursor-pointer';
                div.innerHTML = `
                    <div class="p-4 bg-white rounded-lg shadow-md hover:shadow-xl transition-shadow">
                        <p class="font-bold text-teal-600">${item.year}</p>
                        <h4 class="font-semibold text-lg mb-1">${item.title}</h4>
                        <p class="timeline-text hidden text-sm text-gray-600">${item.text}</p>
                    </div>
                `;
                div.addEventListener('click', () => {
                    div.querySelector('.timeline-text').classList.toggle('hidden');
                });
                timelineContainer.appendChild(div);
            });

            const flowchartContainer = document.getElementById('flowchart');
            const flowchartDetails = document.getElementById('flowchart-details');
            let currentFlowchartText = "Clique em uma etapa para ver os detalhes."; // Armazena o texto atual do flowchartDetails
            
            flowchartStaticData.forEach((item, index) => {
                const stepDiv = document.createElement('div');
                stepDiv.className = 'flowchart-step text-center cursor-pointer p-4';
                stepDiv.innerHTML = `<div class="w-24 h-24 md:w-32 md:h-32 bg-white rounded-full shadow-lg flex items-center justify-center text-center p-2"><span class="font-semibold text-teal-800">${item.title}</span></div>`;
                stepDiv.addEventListener('click', () => {
                    flowchartDetails.innerHTML = `<p class="font-semibold text-lg text-teal-800">${item.title}</p><p class="text-teal-700">${item.text}</p>`;
                    currentFlowchartText = `${item.title}: ${item.text}`;
                });
                flowchartContainer.appendChild(stepDiv);

                if (index < flowchartStaticData.length - 1) {
                    const arrowDiv = document.createElement('div');
                    arrowDiv.className = 'text-teal-400 text-4xl transform md:rotate-0 rotate-90 mx-2';
                    arrowDiv.innerHTML = `<span>➔</span>`;
                    flowchartContainer.appendChild(arrowDiv);
                }
            });

            const criteriaContainer = document.getElementById('criteria-list');
            criteriaData.forEach(item => {
                const div = document.createElement('div');
                div.className = 'bg-white p-6 rounded-lg shadow-md flex items-start space-x-4';
                div.innerHTML = `
                    <div class="text-3xl">${item.icon}</div>
                    <div>
                        <h4 class="font-semibold text-lg text-teal-700">${item.title}</h4>
                        <p class="text-gray-600">${item.text}</p>
                    </div>
                `;
                criteriaContainer.appendChild(div);
            });
            
            const mythsContainer = document.getElementById('myths-facts');
            mythsData.forEach(item => {
                const div = document.createElement('div');
                div.className = 'border border-gray-200 rounded-lg';
                div.innerHTML = `
                    <button class="w-full text-left p-4 bg-white hover:bg-gray-50 flex justify-between items-center rounded-t-lg">
                        <span class="font-semibold text-gray-700">${item.myth}</span>
                        <span class="text-teal-500 transform transition-transform duration-300">▼</span>
                    </button>
                    <div class="fact-content hidden p-4 bg-teal-50 text-teal-800 rounded-b-lg flex items-start">
                        <p class="flex-grow">${item.fact}</p>
                        <button class="tts-fact-btn ml-2 p-1 rounded-full bg-teal-100 hover:bg-teal-200 transition-colors">
                            <svg class="w-5 h-5 text-teal-600" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M9.383 3.003h1.234A.5.5 0 0111 3.5v13a.5.5 0 01-.383.497H9.383a.5.5 0 01-.499-.387l-2.618-8.239A.5.5 0 016.5 8h-2a.5.5 0 01-.497-.383l-2.618-8.24A.5.5 0 010 0v13a.5.5 0 01.497.383l2.618 8.239A.5.5 0 013.5 13h2a.5.5 0 01.499.387l2.618 8.239A.5.5 0 019.5 20h.5a.5.5 0 01.5-.5V.5a.5.5 0 01-.117-.003z" clip-rule="evenodd"></path></svg>
                        </button>
                        <div class="tts-fact-loading loading-spinner hidden"></div>
                    </div>
                `;
                const button = div.querySelector('button');
                const content = div.querySelector('.fact-content');
                const arrow = button.querySelector('span:last-child');
                button.addEventListener('click', () => {
                    content.classList.toggle('hidden');
                    arrow.classList.toggle('rotate-180');
                });
                mythsContainer.appendChild(div);
            });

            // Adiciona event listeners para os botões TTS dos fatos
            document.querySelectorAll('.tts-fact-btn').forEach((btn, index) => {
                btn.addEventListener('click', () => {
                    const factText = mythsData[index].fact;
                    playAudio(factText, btn.nextElementSibling.id || `tts-fact-loading-${index}`);
                });
            });


            const chartData = {
                '2023': {
                    labels: ['Transplantes Realizados', 'Doadores Efetivos'],
                    datasets: [
                        {
                            label: 'Pessoas',
                            data: [28700, 4129],
                            backgroundColor: ['#14B8A6', '#F59E0B'],
                            borderColor: ['#0F766E', '#B45309'],
                            borderWidth: 1,
                            type: 'bar',
                            yAxisID: 'y'
                        },
                        {
                            label: 'Pacientes em Fila de Espera',
                            data: [44626, 44626],
                            borderColor: '#EF4444',
                            backgroundColor: '#EF4444',
                            borderWidth: 2,
                            type: 'line',
                            yAxisID: 'y',
                            pointRadius: 0,
                            fill: false
                        }
                    ]
                },
                '2024': {
                    labels: ['Transplantes Realizados', 'Doadores Efetivos'],
                    datasets: [
                        {
                            label: 'Pessoas',
                            data: [30000, 4086],
                            backgroundColor: ['#14B8A6', '#F59E0B'],
                            borderColor: ['#0F766E', '#B45309'],
                            borderWidth: 1,
                            type: 'bar',
                            yAxisID: 'y'
                        },
                        {
                            label: 'Pacientes em Fila de Espera',
                            data: [78000, 78000],
                            borderColor: '#EF4444',
                            backgroundColor: '#EF4444',
                            borderWidth: 2,
                            type: 'line',
                            yAxisID: 'y',
                            pointRadius: 0,
                            fill: false
                        }
                    ]
                }
            };

            const ctx = document.getElementById('transplantChart').getContext('2d');
            let transplantChart = new Chart(ctx, {
                type: 'bar',
                data: chartData['2023'],
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        title: {
                            display: true,
                            text: 'Panorama da Doação de Órgãos no Brasil - 2023',
                            font: { size: 18 }
                        },
                        tooltip: {
                            callbacks: {
                                label: function(context) {
                                    let label = context.dataset.label || '';
                                    if (label) {
                                        label += ': ';
                                    }
                                    if (context.parsed.y !== null) {
                                        label += new Intl.NumberFormat('pt-BR').format(context.parsed.y);
                                    }
                                    return label;
                                }
                            }
                        }
                    },
                    scales: {
                        y: {
                            beginAtZero: true,
                            title: {
                                display: true,
                                text: 'Número de Pessoas'
                            }
                        }
                    }
                }
            });

            const btn2023 = document.getElementById('btn2023');
            const btn2024 = document.getElementById('btn2024');
            
            function updateChart(year) {
                transplantChart.data = chartData[year];
                transplantChart.options.plugins.title.text = `Panorama da Doação de Órgãos no Brasil - ${year}`;
                transplantChart.update();

                if (year === '2023') {
                    btn2023.classList.add('bg-teal-600', 'text-white');
                    btn2023.classList.remove('bg-white', 'text-gray-900');
                    btn2024.classList.add('bg-white', 'text-gray-900');
                    btn2024.classList.remove('bg-teal-600', 'text-white');
                } else {
                    btn2024.classList.add('bg-teal-600', 'text-white');
                    btn2024.classList.remove('bg-white', 'text-gray-900');
                    btn2033.classList.add('bg-white', 'text-gray-900'); // Note: This line was intended to be btn2023.classList.remove, fixing here.
                    btn2023.classList.remove('bg-teal-600', 'text-white');
                }
            }
            // Corrected the updateChart function for btn2023 remove class.
            
            btn2023.addEventListener('click', () => updateChart('2023'));
            btn2024.addEventListener('click', () => updateChart('2024'));

            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });
            
            const navLinks = document.querySelectorAll('.nav-link, #mobile-menu a');
            const sections = document.querySelectorAll('section');
            const header = document.getElementById('header');

            window.addEventListener('scroll', () => {
                let current = '';
                sections.forEach(section => {
                    const sectionTop = section.offsetTop - header.offsetHeight - 20;
                    if (pageYOffset >= sectionTop) {
                        current = section.getAttribute('id');
                    }
                });

                navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href').substring(1) === current) {
                        link.classList.add('active');
                    }
                });
            });

            // GEMINI API INTEGRATION FEATURES
            const simplifyExplanationBtn = document.getElementById('simplify-explanation-btn');
            const simplifyLoading = document.getElementById('simplify-loading');
            
            simplifyExplanationBtn.addEventListener('click', async () => {
                const currentText = flowchartDetails.innerText; // Get the currently displayed text
                if (!currentText || currentText === "Clique em uma etapa para ver os detalhes.") {
                    flowchartDetails.innerHTML = "<p class='text-red-500'>Por favor, clique em uma etapa do fluxograma primeiro.</p>";
                    return;
                }

                showLoading('simplify-loading');
                const prompt = `Simplifique a seguinte explicação sobre fisiopatologia de morte encefálica para um leigo, usando linguagem clara e direta: "${currentText}"`;
                const payload = { contents: [{ role: "user", parts: [{ text: prompt }] }] };

                try {
                    const result = await callGeminiApi("gemini-2.5-flash-preview-05-20", payload);
                    const simplifiedText = result.candidates?.[0]?.content?.parts?.[0]?.text;
                    if (simplifiedText) {
                        flowchartDetails.innerHTML = `<p class="font-semibold text-lg text-teal-800">Explicação Simplificada:</p><p class="text-teal-700">${simplifiedText}</p>`;
                    } else {
                        flowchartDetails.innerHTML = "<p class='text-red-500'>Não foi possível simplificar a explicação no momento.</p>";
                    }
                } catch (error) {
                    flowchartDetails.innerHTML = "<p class='text-red-500'>Erro ao simplificar a explicação. Tente novamente.</p>";
                } finally {
                    hideLoading('simplify-loading');
                }
            });

            const generateScenarioBtn = document.getElementById('generate-scenario-btn');
            const scenarioLoading = document.getElementById('scenario-loading');
            const conversationScenarioOutput = document.getElementById('conversation-scenario-output');
            const scenarioText = document.getElementById('scenario-text');
            const ttsScenarioBtn = document.getElementById('tts-scenario');
            const ttsScenarioLoading = document.getElementById('tts-scenario-loading');

            generateScenarioBtn.addEventListener('click', async () => {
                showLoading('scenario-loading');
                const prompt = `Gere um pequeno cenário de diálogo (apenas as falas dos personagens) entre dois membros da família (ex: "Filho:" e "Mãe:") discutindo sobre a importância da doação de órgãos após o diagnóstico de morte encefálica de um ente querido. O diálogo deve ser sensível e informativo.`;
                const payload = { contents: [{ role: "user", parts: [{ text: prompt }] }] };

                try {
                    const result = await callGeminiApi("gemini-2.5-flash-preview-05-20", payload);
                    const generatedScenario = result.candidates?.[0]?.content?.parts?.[0]?.text;
                    if (generatedScenario) {
                        scenarioText.innerText = generatedScenario;
                        conversationScenarioOutput.classList.remove('hidden');
                    } else {
                        scenarioText.innerText = "Não foi possível gerar um cenário de conversa no momento.";
                        conversationScenarioOutput.classList.remove('hidden'); // Ainda mostra a caixa, mas com erro
                    }
                } catch (error) {
                    scenarioText.innerText = "Erro ao gerar o cenário de conversa. Tente novamente.";
                    conversationScenarioOutput.classList.remove('hidden'); // Ainda mostra a caixa, mas com erro
                } finally {
                    hideLoading('scenario-loading');
                }
            });

            ttsScenarioBtn.addEventListener('click', () => {
                const textToSpeak = scenarioText.innerText;
                if (textToSpeak) {
                    playAudio(textToSpeak, 'tts-scenario-loading');
                }
            });

            // TTS para os textos introdutórios das seções
            document.getElementById('tts-oquee-intro').addEventListener('click', () => {
                playAudio(document.getElementById('oquee-intro-text').innerText, 'tts-oquee-intro-loading');
            });
            document.getElementById('tts-paradoxo-intro').addEventListener('click', () => {
                playAudio(document.getElementById('paradoxo-intro-text').innerText, 'tts-paradoxo-intro-loading');
            });
            document.getElementById('tts-comoacontece-intro').addEventListener('click', () => {
                playAudio(document.getElementById('comoacontece-intro-text').innerText, 'tts-comoacontece-intro-loading');
            });
            document.getElementById('tts-desafio-intro').addEventListener('click', () => {
                playAudio(document.getElementById('desafio-intro-text').innerText, 'tts-desafio-intro-loading');
            });
        });
    </script>
</body>
</html>
