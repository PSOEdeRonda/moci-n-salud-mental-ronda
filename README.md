<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moción Salud Mental Juvenil - Ronda</title>
    <!-- Incluir Tailwind CSS para el diseño -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Incluir Font Awesome para el icono del logo y los votos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Incluir Lucide Icons para iconos adicionales -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        /* Configuración de fuente y colores basada en el diseño de impacto */
        :root {
            --color-psoe: #E6002E; /* Rojo principal */
            --color-pp: #0087DC; /* Azul PP para contraste */
            --color-bg-dark: #1a1a1a;
            --color-text-light: #f3f4f6;
        }
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f9fafb;
            line-height: 1.6;
            scroll-behavior: smooth; /* Para el scroll suave */
        }
        .header-bg {
            background-color: var(--color-psoe);
        }
        .text-psoe { color: var(--color-psoe); }
        .bg-psoe { background-color: var(--color-psoe); }
        .bg-pp { background-color: var(--color-pp); }
        .shadow-psoe { box-shadow: 0 10px 15px -3px rgba(230, 0, 46, 0.4), 0 4px 6px -2px rgba(230, 0, 46, 0.2); }

        /* Estilo para las tarjetas de las medidas */
        .measure-card {
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
            border-left: 5px solid var(--color-psoe);
        }
        .measure-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.1);
        }
        /* Estilo para las tarjetas de datos */
        .data-card {
            border: 2px solid #ddd;
            transition: box-shadow 0.3s;
        }
        .data-card:hover {
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.15);
        }

        /* Clase para la animación de la notificación de copia */
        .fade-in-out {
            animation: fadeInOut 3s ease-in-out;
        }
        @keyframes fadeInOut {
            0% { opacity: 0; transform: translateY(-10px); }
            10% { opacity: 1; transform: translateY(0); }
            90% { opacity: 1; transform: translateY(0); }
            100% { opacity: 0; transform: translateY(-10px); }
        }
    </style>
</head>
<body class="min-h-screen flex flex-col">

    <!-- Header / Navegación (Anchor para Volver al Inicio) -->
    <header id="top" class="header-bg text-white py-4 shadow-xl sticky top-0 z-50">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center justify-center space-y-2">

            <!-- INICIO: Logo de Texto Actualizado -->
            <div class="text-center">
                <a href="#top" class="hover:opacity-90 transition duration-300">
                    <span class="text-white text-xl sm:text-2xl font-black tracking-widest uppercase">PSOE de Ronda</span>
                    <span class="text-white text-sm sm:text-lg font-medium block mt-[-4px]">Grupo Municipal Socialista</span>
                </a>
            </div>
            <!-- FIN: Logo de Texto Actualizado -->
            
            <!-- Botón de Acción Centrado Debajo del Texto -->
            <a href="#votacion-section" class="bg-white text-psoe py-2 px-4 rounded-full font-bold text-sm shadow-md hover:bg-red-100 transition duration-300">
                Ver Votación
            </a>
        </div>
    </header>

    <!-- Sección Principal (Introducción y Datos de Impacto) -->
    <main class="flex-grow pt-10 pb-16">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">

            <!-- Título Principal y Resumen -->
            <div class="text-center mb-12">
                <span class="text-sm font-semibold uppercase tracking-widest text-psoe">MOCIÓN OCTUBRE 2025</span>
                <h2 class="text-4xl sm:text-5xl font-extrabold text-gray-900 mt-2 mb-4">
                    PLAN MUNICIPAL DE SALUD MENTAL JUVENIL
                </h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">
                    Una respuesta urgente y estructural a la crisis de salud mental que afecta a nuestra juventud.
                </p>
            </div>

            <!-- SECCIÓN: Datos que Motivan la Moción (Visual) -->
            <section class="mb-16">
                <h3 class="text-3xl font-extrabold text-gray-800 text-center mb-8 border-b-2 border-red-100 pb-3">
                    <i data-lucide="bar-chart-3" class="w-6 h-6 inline-block mr-2 text-psoe"></i>
                    Datos que nos Obligan a Actuar
                </h3>

                <div class="grid md:grid-cols-3 gap-6">

                    <!-- Dato 1: Suicidio (Peligro Máximo) -->
                    <div class="data-card bg-white p-6 rounded-xl shadow-lg text-center">
                        <div class="text-6xl font-extrabold text-psoe mb-2">
                            1ª
                        </div>
                        <p class="text-lg font-bold text-gray-800">Causa de Muerte Externa</p>
                        <p class="text-sm text-gray-600 mt-1">
                            El suicidio es la primera causa de muerte no natural entre jóvenes de **15 a 29 años** en España.
                        </p>
                        <span class="text-xs text-red-500 font-semibold mt-2 block">
                            (Confederación Salud Mental España)
                        </span>
                    </div>
                    
                    <!-- Dato 2: Prevalencia OMS (Impacto Global) -->
                    <div class="data-card bg-white p-6 rounded-xl shadow-lg text-center">
                        <div class="text-6xl font-extrabold text-gray-800 mb-2">
                            1 de 7
                        </div>
                        <p class="text-lg font-bold text-gray-800">Adolescentes Afectados</p>
                        <p class="text-sm text-gray-600 mt-1">
                            La OMS estima que 1 de cada 7 adolescentes en el mundo padece **algún problema de salud mental**.
                        </p>
                        <span class="text-xs text-red-500 font-semibold mt-2 block">
                            (Organización Mundial de la Salud - OMS)
                        </span>
                    </div>

                    <!-- Dato 3: Patologías Frecuentes (Ministerio) -->
                    <div class="data-card bg-white p-6 rounded-xl shadow-lg text-center">
                        <div class="text-6xl font-extrabold text-psoe mb-2">
                            ↑
                        </div>
                        <p class="text-lg font-bold text-gray-800">Ansiedad y Depresión</p>
                        <p class="text-sm text-gray-600 mt-1">
                            Los trastornos de **ansiedad y depresión** son las patologías más frecuentes y se han incrementado en la juventud.
                        </p>
                        <span class="text-xs text-red-500 font-semibold mt-2 block">
                            (Ministerio de Sanidad)
                        </span>
                    </div>
                </div>
            </section>
            <!-- FIN SECCIÓN DE DATOS -->

            <!-- Título de las Medidas -->
            <div class="text-center mb-10">
                <h3 class="text-3xl font-extrabold text-gray-800 mb-2 border-b-2 border-red-100 pb-3">
                    <i data-lucide="check-square" class="w-6 h-6 inline-block mr-2 text-psoe"></i>
                    Las 7 Medidas Propuestas
                </h3>
                <p class="text-gray-600 text-lg">
                    Un plan integral y municipal para dotar a Ronda de los recursos que su juventud necesita.
                </p>
            </div>

            <!-- Grid de las 7 Medidas -->
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">

                <!-- Medida 1 -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card">
                    <i data-lucide="users" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">1. Apoyo Psicológico Gratuito</h3>
                    <p class="text-gray-600 text-sm">Puesta en marcha de un servicio de atención, coordinación con centros educativos y recursos sanitarios (presencial y online).</p>
                </div>

                <!-- Medida 2 -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card">
                    <i data-lucide="school" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">2. Talleres de Bienestar Emocional</h3>
                    <p class="text-gray-600 text-sm">Desarrollo de talleres sobre gestión emocional, autoestima, uso responsable de redes sociales y prevención del suicidio.</p>
                </div>

                <!-- Medida 3 -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card">
                    <i data-lucide="lock-keyhole" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">3. Espacio Confidencial y Anónimo</h3>
                    <p class="text-gray-600 text-sm">Creación de un lugar seguro con profesionales especializados donde los jóvenes puedan acudir sin miedo.</p>
                </div>

                <!-- Medida 4 -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card">
                    <i data-lucide="eye-off" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">4. Lucha contra el Estigma</h3>
                    <p class="text-gray-600 text-sm">Impulso de campañas municipales de sensibilización en medios locales y redes sociales.</p>
                </div>

                <!-- Medida 5 -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card">
                    <i data-lucide="handshake" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">5. Convenios de Colaboración</h3>
                    <p class="text-gray-600 text-sm">Establecer acuerdos con colegios profesionales de psicología, asociaciones de salud mental, AMPAS y entidades especializadas, para la calidad del servicio.</p>
                </div>

                <!-- Medida 6 -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card">
                    <i data-lucide="monitor" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">6. Observatorio Municipal</h3>
                    <p class="text-gray-600 text-sm">Creación de un observatorio con el sistema sanitario, centros educativos y colectivos sociales, que permita detectar tendencias y necesidades de forma temprana.</p>
                </div>

                <!-- Medida 7 (Medida de Transparencia) - CENTRADA Y MISMO ANCHO -->
                <!-- En pantallas grandes (lg), comienza en la columna 2 y ocupa solo 1 columna para centrarse -->
                <div class="bg-white p-6 rounded-xl shadow-lg measure-card lg:col-start-2 lg:col-span-1 md:col-span-2">
                    <i data-lucide="file-text" class="w-8 h-8 text-psoe mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-800 mb-2">7. Rendición de Cuentas Anual</h3>
                    <p class="text-gray-600 text-sm">Presentación de un informe anual al Pleno para garantizar la transparencia y el control público del Plan.</p>
                </div>
            </div>

            <!-- Botón de Difusión y CTA -->
            <div class="text-center mt-16">
                <p class="text-2xl font-bold text-gray-800 mb-4">¿Apoyas estas medidas?</p>
                <button id="copyUrlBtn" class="bg-psoe text-white py-3 px-8 rounded-lg font-extrabold text-xl hover:bg-red-700 transition duration-300 transform hover:scale-105 shadow-psoe">
                    <i data-lucide="share-2" class="w-6 h-6 inline-block mr-3"></i>
                    <span id="copyText">Difunde esta información</span>
                </button>
                <div id="notification-area" class="mt-4 h-6 relative"></div> <!-- Área para la notificación de copia -->
            </div>
            
        </div>
    </main>
    
    <!-- Sección de Votación (Impacto Visual) -->
    <section id="votacion-section" class="py-16 bg-gray-900 text-white border-t-8 border-psoe">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            
            <h2 class="text-4xl sm:text-5xl font-extrabold mb-8 uppercase tracking-wider">
                El Resultado de la Votación
            </h2>
            
            <div class="bg-white text-gray-900 p-8 rounded-xl shadow-2xl">
                <p class="text-xl font-medium mb-6">
                    Moción presentada en el Pleno de octubre de 2025.
                </p>
                
                <div class="flex flex-col sm:flex-row justify-center items-center space-y-6 sm:space-y-0 sm:space-x-12">
                    
                    <!-- Voto a Favor -->
                    <div class="flex flex-col items-center">
                        <div class="w-24 h-24 sm:w-32 sm:h-32 bg-psoe rounded-full flex items-center justify-center text-white mb-3 shadow-psoe">
                            <i class="fas fa-check text-4xl sm:text-5xl"></i>
                        </div>
                        <p class="text-3xl sm:text-4xl font-extrabold text-psoe">A FAVOR</p>
                        <p class="text-lg font-semibold mt-1">Grupo Socialista</p>
                    </div>

                    <div class="text-4xl font-bold text-gray-500 hidden sm:block">VS</div>
                    
                    <!-- Voto En Contra -->
                    <div class="flex flex-col items-center">
                        <div class="w-24 h-24 sm:w-32 sm:h-32 bg-pp rounded-full flex items-center justify-center text-white mb-3 shadow-lg" style="box-shadow: 0 10px 15px -3px rgba(0, 135, 220, 0.4);">
                            <i class="fas fa-times text-4xl sm:text-5xl"></i>
                        </div>
                        <p class="text-3xl sm:text-4xl font-extrabold text-pp">EN CONTRA</p>
                        <p class="text-lg font-semibold mt-1">Equipo de Gobierno (PP)</p>
                    </div>

                </div>
                
                <p class="text-xl font-bold text-gray-800 mt-10">
                    La moción fue <strong class="text-red-600 uppercase">rechazada</strong> por el voto en contra del Partido Popular.
                </p>
            </div>
            
            <!-- Botón de retorno -->
            <a href="#top" id="backToTopBtn" class="inline-block mt-10 text-white font-semibold text-lg hover:underline transition duration-300 cursor-pointer">
                <i data-lucide="arrow-up" class="w-5 h-5 inline-block mr-2"></i>
                Volver arriba
            </a>
            
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-6">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-sm">&copy; 2025 Grupo Municipal Socialista de Ronda. Todos los derechos reservados.</p>
        </div>
    </footer>

    <!-- JavaScript para la funcionalidad de copiar URL y la carga de iconos -->
    <script>
        // Inicializar los iconos de Lucide
        lucide.createIcons();
        
        // El texto que se va a copiar al portapapeles
        const diffusionText = `https://psoederonda.github.io/moci-n-salud-mental-ronda/ y difunde.`;

        // Funcionalidad para forzar el scroll al inicio de forma suave
        document.getElementById('backToTopBtn').addEventListener('click', function(event) {
            event.preventDefault(); 
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Funcionalidad para copiar el texto de difusión
        document.getElementById('copyUrlBtn').addEventListener('click', function() {
            
            if (navigator.clipboard) {
                navigator.clipboard.writeText(diffusionText).then(() => {
                    showNotification('¡Mensaje de difusión copiado!');
                }).catch(err => {
                    fallbackCopyTextToClipboard(diffusionText);
                });
            } else {
                fallbackCopyTextToClipboard(diffusionText);
            }
        });

        function showNotification(message) {
            const notificationArea = document.getElementById('notification-area');
            const copyTextSpan = document.getElementById('copyText');
            
            const originalText = copyTextSpan.textContent;
            copyTextSpan.textContent = "¡COPIADO!";

            const notification = document.createElement('div');
            notification.textContent = message;
            notification.className = 'bg-green-500 text-white py-2 px-4 rounded-lg shadow-md text-center text-sm font-semibold fade-in-out absolute left-1/2 transform -translate-x-1/2';
            
            notificationArea.innerHTML = '';
            notificationArea.appendChild(notification);
            
            setTimeout(() => {
                notificationArea.innerHTML = '';
                copyTextSpan.textContent = originalText;
            }, 3000);
        }

        function fallbackCopyTextToClipboard(text) {
            const tempInput = document.createElement('textarea');
            tempInput.value = text;
            tempInput.style.position = 'absolute';
            tempInput.style.left = '-9999px';
            document.body.appendChild(tempInput);
            tempInput.select();

            try {
                document.execCommand('copy'); 
                showNotification('¡Mensaje de difusión copiado!');
            } catch (err) {
                showNotification('Error: Copia manual necesaria.');
                console.error('Error al copiar el texto: ', err);
            } finally {
                document.body.removeChild(tempInput);
            }
        }
        
        // Inicializar los iconos después de que el DOM esté cargado
        document.addEventListener('DOMContentLoaded', () => {
            lucide.createIcons();
        });

    </script>
</body>
</html>
