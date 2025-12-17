<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Servicios Eléctricos Residenciales | Seguridad y Confort</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- FontAwesome para Iconos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        
        .hero-bg {
            background-image: linear-gradient(rgba(15, 23, 42, 0.7), rgba(15, 23, 42, 0.7)), url('https://images.unsplash.com/photo-1565538810643-b5bdb714032a?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
        }

        .service-card:hover {
            transform: translateY(-5px);
        }

        /* Animación suave para el botón de WhatsApp */
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 40px;
            right: 40px;
            background-color: #25d366;
            color: #FFF;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 3px #999;
            z-index: 100;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }

        .whatsapp-float:hover {
            background-color: #128c7e;
            transform: scale(1.1);
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800">

    <!-- Navegación -->
    <nav class="bg-white shadow-md fixed w-full z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20">
                <div class="flex items-center">
                    <!-- Logo / Nombre -->
                    <div class="flex-shrink-0 flex items-center gap-2">
                        <i class="fa-solid fa-bolt text-yellow-500 text-3xl"></i>
                        <div>
                            <span class="font-bold text-xl tracking-tight text-slate-900 block leading-none">AUTOMPROC</span>
                            <span class="text-xs text-slate-500 uppercase tracking-widest">Residencial</span>
                        </div>
                    </div>
                </div>
                
                <!-- Menú Escritorio -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#inicio" class="text-slate-600 hover:text-blue-900 font-medium transition">Inicio</a>
                    <a href="#servicios" class="text-slate-600 hover:text-blue-900 font-medium transition">Servicios</a>
                    <a href="#seguridad" class="text-slate-600 hover:text-blue-900 font-medium transition">Tips de Seguridad</a>
                    <a href="#contacto" class="bg-blue-900 text-white px-5 py-2.5 rounded-md font-semibold hover:bg-blue-800 transition shadow-lg shadow-blue-900/30">
                        Solicitar Revisión
                    </a>
                </div>

                <!-- Botón Menú Móvil -->
                <div class="flex items-center md:hidden">
                    <button id="mobile-menu-btn" class="text-slate-600 hover:text-slate-900 focus:outline-none p-2">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Menú Móvil Desplegable -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#inicio" class="block px-3 py-2 text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-900 rounded-md">Inicio</a>
                <a href="#servicios" class="block px-3 py-2 text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-900 rounded-md">Servicios</a>
                <a href="#seguridad" class="block px-3 py-2 text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-900 rounded-md">Tips de Seguridad</a>
                <a href="#contacto" class="block px-3 py-2 text-base font-medium text-blue-600 font-bold hover:bg-blue-50 rounded-md">Contáctanos</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="inicio" class="hero-bg h-screen flex items-center justify-center text-center px-4 relative">
        <div class="max-w-4xl mx-auto animate-fade-in-up">
            <span class="inline-block py-1 px-3 rounded-full bg-yellow-500/20 text-yellow-400 text-sm font-semibold mb-6 border border-yellow-500/30">
                ⚡ Expertos en Electricidad Residencial
            </span>
            <h1 class="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">
                Potencia, Seguridad y Estilo <br/> para su Hogar
            </h1>
            <p class="text-lg md:text-xl text-slate-200 mb-10 max-w-2xl mx-auto">
                Desde la instalación de un tomacorriente hasta la renovación completa de su tablero eléctrico. Modernizamos su vivienda para proteger lo que más importa.
            </p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#contacto" class="bg-yellow-500 text-slate-900 px-8 py-4 rounded-lg font-bold text-lg hover:bg-yellow-400 transition transform hover:scale-105 shadow-xl">
                    Agendar Inspección
                </a>
                <a href="#servicios" class="bg-transparent border-2 border-white text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-white/10 transition">
                    Ver Servicios
                </a>
            </div>
        </div>
        
        <!-- Flecha bajar -->
        <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce text-white/50">
            <i class="fa-solid fa-chevron-down text-2xl"></i>
        </div>
    </section>

    <!-- Sección de Servicios -->
    <section id="servicios" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-blue-900 font-bold text-3xl md:text-4xl mb-4">Nuestros Servicios Principales</h2>
                <p class="text-slate-600 max-w-2xl mx-auto text-lg">Soluciones integrales para modernizar la instalación eléctrica de su casa.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-10">
                <!-- Servicio 1: Tomacorrientes -->
                <div class="service-card bg-slate-50 rounded-2xl p-8 border border-slate-100 shadow-sm transition duration-300 hover:shadow-xl group">
                    <div class="w-16 h-16 bg-blue-100 rounded-xl flex items-center justify-center mb-6 group-hover:bg-blue-900 transition duration-300">
                        <i class="fa-solid fa-plug text-2xl text-blue-900 group-hover:text-white transition"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-slate-900 mb-4">Tomacorrientes Modernos</h3>
                    <ul class="space-y-3 text-slate-600">
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Instalación de <strong>puntos USB</strong> directos en pared.</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Protección <strong>GFCI</strong> para baños y cocinas (anti-descargas).</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Reemplazo de enchufes flojos o quemados.</span>
                        </li>
                    </ul>
                </div>

                <!-- Servicio 2: Iluminación -->
                <div class="service-card bg-slate-50 rounded-2xl p-8 border border-slate-100 shadow-sm transition duration-300 hover:shadow-xl group">
                    <div class="w-16 h-16 bg-yellow-100 rounded-xl flex items-center justify-center mb-6 group-hover:bg-yellow-500 transition duration-300">
                        <i class="fa-regular fa-lightbulb text-2xl text-yellow-600 group-hover:text-white transition"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-slate-900 mb-4">Iluminación LED & Diseño</h3>
                    <ul class="space-y-3 text-slate-600">
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Transición a <strong>LED</strong> (Ahorre hasta 80% en luz).</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Instalación de <strong>Ojos de Buey</strong> empotrados.</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Dimmers y sensores de movimiento exteriores.</span>
                        </li>
                    </ul>
                </div>

                <!-- Servicio 3: Tableros -->
                <div class="service-card bg-slate-50 rounded-2xl p-8 border border-slate-100 shadow-sm transition duration-300 hover:shadow-xl group">
                    <div class="w-16 h-16 bg-red-100 rounded-xl flex items-center justify-center mb-6 group-hover:bg-red-600 transition duration-300">
                        <i class="fa-solid fa-server text-2xl text-red-600 group-hover:text-white transition"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-slate-900 mb-4">Tableros Eléctricos</h3>
                    <ul class="space-y-3 text-slate-600">
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Actualización de cajas de fusibles antiguas.</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span><strong>Aumento de carga</strong> para Aire Acondicionado.</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa-solid fa-check text-green-500 mt-1 mr-2"></i>
                            <span>Balanceo de cargas y corrección de fallas.</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Seguridad (Tip del Experto) -->
    <section id="seguridad" class="py-20 bg-blue-900 text-white relative overflow-hidden">
        <!-- Elemento decorativo de fondo -->
        <i class="fa-solid fa-shield-halved absolute -right-10 -bottom-10 text-9xl text-white/5 rotate-12"></i>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 flex flex-col md:flex-row items-center gap-12">
            <div class="md:w-1/2">
                <div class="inline-block bg-yellow-500 text-blue-900 font-bold px-4 py-1 rounded-full text-sm mb-4">
                    <i class="fa-solid fa-triangle-exclamation mr-2"></i> TIP DE SEGURIDAD
                </div>
                <h2 class="text-3xl md:text-4xl font-bold mb-6">La Prueba del "Test/Reset"</h2>
                <p class="text-blue-100 text-lg leading-relaxed mb-6">
                    Vaya a su baño o cocina. ¿El tomacorriente tiene dos botones (Test y Reset)? Si no los tiene, <strong>no está protegido contra la humedad</strong>. 
                </p>
                <p class="text-blue-100 text-lg leading-relaxed mb-8">
                    Si los tiene, presione "Test". ¿Se cortó la energía? Si no lo hizo, el mecanismo está dañado y su familia está en riesgo.
                </p>
                <a href="#contacto" class="inline-block border-2 border-yellow-500 text-yellow-500 hover:bg-yellow-500 hover:text-blue-900 font-bold px-8 py-3 rounded-lg transition">
                    Solicitar Cambio de GFCI
                </a>
            </div>
            <div class="md:w-1/2 bg-white/10 p-8 rounded-2xl backdrop-blur-sm border border-white/20">
                <div class="flex items-start gap-4">
                    <div class="bg-red-500 rounded-full p-3 flex-shrink-0">
                        <i class="fa-solid fa-fire-extinguisher text-white text-xl"></i>
                    </div>
                    <div>
                        <h4 class="font-bold text-xl mb-2">¿Sabía qué?</h4>
                        <p class="text-blue-100">
                            Más del 30% de los incendios domésticos son causados por fallas eléctricas, cables antiguos o tableros sobrecargados. La prevención es la mejor inversión.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Contacto -->
    <section id="contacto" class="py-24 bg-slate-50">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col md:flex-row">
                
                <!-- Info Contacto -->
                <div class="bg-slate-900 p-10 md:w-2/5 text-white flex flex-col justify-between">
                    <div>
                        <h3 class="text-2xl font-bold mb-6">Contáctenos</h3>
                        <p class="text-slate-400 mb-8">Estamos listos para atender sus emergencias o proyectos de renovación.</p>
                        
                        <div class="space-y-6">
                            <div class="flex items-center gap-4">
                                <div class="w-10 h-10 bg-blue-800 rounded-lg flex items-center justify-center text-yellow-400">
                                    <i class="fa-solid fa-phone"></i>
                                </div>
                                <div>
                                    <p class="text-xs text-slate-400 uppercase">Llámenos</p>
                                    <p class="font-bold">+502 1234-5678</p>
                                </div>
                            </div>
                            
                            <div class="flex items-center gap-4">
                                <div class="w-10 h-10 bg-blue-800 rounded-lg flex items-center justify-center text-yellow-400">
                                    <i class="fa-solid fa-envelope"></i>
                                </div>
                                <div>
                                    <p class="text-xs text-slate-400 uppercase">Correo</p>
                                    <p class="font-bold">info@automproc.com</p>
                                </div>
                            </div>

                            <div class="flex items-center gap-4">
                                <div class="w-10 h-10 bg-blue-800 rounded-lg flex items-center justify-center text-yellow-400">
                                    <i class="fa-solid fa-location-dot"></i>
                                </div>
                                <div>
                                    <p class="text-xs text-slate-400 uppercase">Zona de Cobertura</p>
                                    <p class="font-bold">Toda la Ciudad y Alrededores</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-10">
                        <p class="text-sm text-slate-500">Síguenos en redes:</p>
                        <div class="flex gap-4 mt-3">
                            <a href="#" class="text-white hover:text-yellow-400 transition"><i class="fa-brands fa-facebook text-xl"></i></a>
                            <a href="#" class="text-white hover:text-yellow-400 transition"><i class="fa-brands fa-instagram text-xl"></i></a>
                            <a href="#" class="text-white hover:text-yellow-400 transition"><i class="fa-brands fa-whatsapp text-xl"></i></a>
                        </div>
                    </div>
                </div>

                <!-- Formulario -->
                <div class="p-10 md:w-3/5">
                    <h3 class="text-2xl font-bold text-slate-800 mb-6">Solicitar Cotización</h3>
                    <form id="contactForm" onsubmit="handleSubmit(event)">
                        <div class="space-y-4">
                            <div>
                                <label class="block text-sm font-medium text-slate-700 mb-1">Nombre Completo</label>
                                <input type="text" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-900 focus:border-blue-900 outline-none transition" placeholder="Juan Pérez">
                            </div>
                            
                            <div>
                                <label class="block text-sm font-medium text-slate-700 mb-1">Teléfono</label>
                                <input type="tel" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-900 focus:border-blue-900 outline-none transition" placeholder="Para contactarle por WhatsApp">
                            </div>

                            <div>
                                <label class="block text-sm font-medium text-slate-700 mb-1">Servicio de Interés</label>
                                <select class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-900 focus:border-blue-900 outline-none transition">
                                    <option>Revisión General / Diagnóstico</option>
                                    <option>Instalación de Tomacorrientes</option>
                                    <option>Iluminación LED</option>
                                    <option>Tablero Eléctrico / Breakers</option>
                                    <option>Otro</option>
                                </select>
                            </div>

                            <div>
                                <label class="block text-sm font-medium text-slate-700 mb-1">Mensaje</label>
                                <textarea rows="3" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-900 focus:border-blue-900 outline-none transition" placeholder="Describa brevemente su problema..."></textarea>
                            </div>

                            <button type="submit" class="w-full bg-blue-900 text-white font-bold py-3 rounded-lg hover:bg-blue-800 transition shadow-lg transform active:scale-95">
                                Enviar Solicitud
                            </button>
                        </div>
                    </form>
                    
                    <!-- Mensaje de éxito oculto por defecto -->
                    <div id="successMessage" class="hidden mt-4 p-4 bg-green-100 text-green-700 rounded-lg border border-green-200">
                        <div class="flex items-center gap-2">
                            <i class="fa-solid fa-circle-check"></i>
                            <p class="font-bold">¡Mensaje Enviado!</p>
                        </div>
                        <p class="text-sm mt-1">Gracias por contactarnos. Uno de nuestros técnicos le escribirá pronto.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-8 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 text-center">
            <p>&copy; 2023 Automproc Industrial. Todos los derechos reservados.</p>
            <p class="text-sm mt-2">Expertos en Automatización y Servicios Residenciales.</p>
        </div>
    </footer>

    <!-- Botón Flotante WhatsApp -->
    <a href="https://wa.me/1234567890" target="_blank" class="whatsapp-float" title="Chat en WhatsApp">
        <i class="fa-brands fa-whatsapp"></i>
    </a>

    <!-- Scripts simples -->
    <script>
        // Lógica del menú móvil
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
        });

        // Simulación de envío de formulario
        function handleSubmit(e) {
            e.preventDefault();
            const form = document.getElementById('contactForm');
            const successMsg = document.getElementById('successMessage');
            
            // Simular carga
            const btnSubmit = form.querySelector('button');
            const originalText = btnSubmit.innerText;
            btnSubmit.innerText = 'Enviando...';
            btnSubmit.disabled = true;

            setTimeout(() => {
                form.reset();
                successMsg.classList.remove('hidden');
                btnSubmit.innerText = originalText;
                btnSubmit.disabled = false;
                
                // Ocultar mensaje después de 5 segundos
                setTimeout(() => {
                    successMsg.classList.add('hidden');
                }, 5000);
            }, 1500);
        }
    </script>
</body>
</html>
