
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Súmate a la Brigada de Emergencia | Convocatoria</title>
    <!-- Tailwind CSS para diseño moderno -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome para iconografía enriquecida -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts - Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Aptos', sans-serif;
        }
        html {
            scroll-behavior: smooth;
        }
        /* Efecto de pulso de advertencia */
        .glow-red {
            box-shadow: 0 0 15px rgba(239, 68, 68, 0.5);
        }
        /* Animaciones personalizadas */
        .pulse-soft {
            animation: softPulse 2s infinite;
        }
        @keyframes softPulse {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.05); opacity: 0.95; }
        }
        /* Estilos específicos para cuando la edición está activa */
        .editable-active [contenteditable="true"] {
            outline: 2px dashed #ef4444 !important;
            outline-offset: 4px;
            background-color: rgba(239, 68, 68, 0.05);
            border-radius: 4px;
            cursor: pointer;
        }
        .editable-active [contenteditable="true"]:hover {
            background-color: rgba(239, 68, 68, 0.1);
        }
        /* Ocultar barra de scroll en paneles admin */
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
    </style>
</head>
<body class="bg-slate-950 text-slate-100 min-h-screen selection:bg-red-600 selection:text-white">

    <!-- BARRA DE NAVEGACIÓN -->
    <nav class="fixed w-full bg-slate-950/90 text-white backdrop-blur-md z-40 border-b border-slate-800 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 bg-red-600 rounded-xl flex items-center justify-center glow-red">
                    <i class="fa-solid fa-fire-extinguisher text-white text-lg animate-bounce"></i>
                </div>
                <div>
                    <span class="font-extrabold text-lg tracking-wider text-white block uppercase" contenteditable="false" data-edit="brand-title">BRIGADA DE RESPUESTA</span>
                    <span class="text-[10px] text-red-500 font-bold tracking-widest uppercase" contenteditable="false" data-edit="brand-subtitle">PRIMERA LÍNEA DE SEGURIDAD</span>
                </div>
            </div>
            
            <div class="hidden lg:flex space-x-8 font-medium text-sm items-center">
                <a href="#inicio" class="hover:text-red-500 transition-colors">Inicio</a>
                <a href="#mision" class="hover:text-red-500 transition-colors">Misión</a>
                <a href="#pilares" class="hover:text-red-500 transition-colors">Capacitación</a>
                <a href="#requisitos" class="hover:text-red-500 transition-colors">Requisitos</a>
                <a href="#postular" class="bg-red-600 hover:bg-red-700 px-5 py-2.5 rounded-xl text-white transition-all shadow-lg hover:shadow-red-600/40 font-bold">Postular Aquí</a>
            </div>

            <!-- Botones de Utilidades en Nav para pantallas chicas -->
            <div class="flex items-center space-x-2">
                <button onclick="toggleAdminPanel()" class="bg-slate-800 hover:bg-slate-700 text-slate-300 hover:text-white px-3 py-2 rounded-xl text-xs font-semibold flex items-center space-x-1.5 transition-all">
                    <i class="fa-solid fa-screwdriver-wrench"></i>
                    <span class="hidden sm:inline">Editor Visual</span>
                </button>
            </div>
        </div>
    </nav>

    <!-- HERO SECTION -->
    <section id="inicio" class="relative min-h-screen flex items-center justify-center bg-slate-950 text-white overflow-hidden pt-20">
        <!-- Fondo con superposición de gradientes y máscara industrial -->
        <div class="absolute inset-0 bg-cover bg-center opacity-30" style="background-image: url('https://images.unsplash.com/photo-1599740831618-24d14212e3e5?q=80&w=1920');"></div>
        <div class="absolute inset-0 bg-gradient-to-tr from-slate-950 via-slate-950/80 to-transparent"></div>
        <div class="absolute inset-0 bg-radial-gradient from-transparent to-slate-950 opacity-90"></div>
        
        <!-- Líneas y cuadrícula decorativa de fondo -->
        <div class="absolute inset-0 opacity-10 pointer-events-none" style="background-image: radial-gradient(circle, #475569 1px, transparent 1px); background-size: 24px 24px;"></div>

        <div class="relative z-10 text-center max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="inline-flex items-center space-x-2 bg-red-600/10 border border-red-500/30 text-red-400 text-xs uppercase tracking-widest font-extrabold px-4 py-2 rounded-full mb-6">
                <span class="w-2 h-2 rounded-full bg-red-500 animate-ping"></span>
                <span contenteditable="false" data-edit="convocatoria-tag">CONVOCATORIA 2026</span>
            </div>
            
            <h1 class="text-4xl sm:text-6xl lg:text-7xl font-black tracking-tight mb-6 leading-none">
                <span contenteditable="false" data-edit="hero-title-1" class="block text-white">EL VALOR DE PROTEGER</span>
                <span contenteditable="false" data-edit="hero-title-2" class="block text-transparent bg-clip-text bg-gradient-to-r from-red-500 to-amber-500">ESTÁ EN TUS MANOS</span>
            </h1>
            
            <p class="text-lg sm:text-xl text-slate-300 mb-10 max-w-3xl mx-auto leading-relaxed font-light" contenteditable="false" data-edit="hero-desc">
                Capacítate con estándares internacionales. Capacítate en habiliades sobre Control de Incendios, Rescate Técnico y Soporte Vital Básico.
                No necesitas experiencia, solo la valentia para dar un nuevo paso.
            </p>
            
            <div class="flex flex-col sm:flex-row justify-center items-center gap-4">
                <a href="#postular" class="w-full sm:w-auto bg-gradient-to-r from-red-600 to-red-700 hover:from-red-700 hover:to-red-800 text-white font-bold px-8 py-4 rounded-2xl shadow-xl shadow-red-600/30 transition-all transform hover:-translate-y-1 text-center">
                    Quiero Ser Brigadista
                </a>
            </div>

            <!-- Resumen de estadísticas en vivo -->
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mt-20 max-w-3xl mx-auto border-t border-slate-800/80 pt-10">
                <div class="text-center">
                    <span class="block text-3xl sm:text-4xl font-extrabold text-white" contenteditable="false" data-edit="stat-1-num">+60</span>
                    <span class="text-xs text-slate-400 uppercase tracking-widest mt-1 block" contenteditable="false" data-edit="stat-1-label">Brigadistas Activos</span>
                </div>
                <div class="text-center">
                    <span class="block text-3xl sm:text-4xl font-extrabold text-red-500" contenteditable="false" data-edit="stat-2-num">24/7</span>
                    <span class="text-xs text-slate-400 uppercase tracking-widest mt-1 block" contenteditable="false" data-edit="stat-2-label">Respuesta Inmediata</span>
                </div>
                <div class="text-center">
                    <span class="block text-3xl sm:text-4xl font-extrabold text-white" contenteditable="false" data-edit="stat-3-num">+400 hrs</span>
                    <span class="text-xs text-slate-400 uppercase tracking-widest mt-1 block" contenteditable="false" data-edit="stat-3-label">Entrenamiento Anual</span>
                </div>
                <div class="text-center">
                    <span class="block text-3xl sm:text-4xl font-extrabold text-amber-500" contenteditable="false" data-edit="stat-4-num">+120</span>
                    <span class="text-xs text-slate-400 uppercase tracking-widest mt-1 block" contenteditable="false" data-edit="stat-4-label">Emergencias Atendidas</span>
                </div>
            </div>
        </div>
    </section>

    <!-- PROPÓSITO / MISIÓN -->
    <section id="mision" class="py-24 px-4 sm:px-6 lg:px-8 bg-slate-900 border-y border-slate-800/60">
        <div class="max-w-5xl mx-auto text-center">
            <h2 class="text-xs font-bold text-red-500 uppercase tracking-widest mb-3">NUESTRO COMPROMISO</h2>
            <h3 class="text-3xl sm:text-4xl font-extrabold text-white mb-6" contenteditable="false" data-edit="mision-title">¿POR QUÉ ES VITAL ES SER PARTE DE NUESTRO EQUIPO?</h3>
            <p class="text-lg sm:text-xl text-slate-400 leading-relaxed max-w-3xl mx-auto font-light mb-16" contenteditable="false" data-edit="mision-lead">
                Pertenecer a la Brigada de Emergencias es una oportunidad para contribuir activamente a la seguridad de las personas y la protección de las instalaciones. Ser parte de este equipo significa desarrollar habilidades para actuar de manera rápida y efectiva ante situaciones de emergencia, fortaleciendo el trabajo en equipo, el liderazgo y la prevención. Cada brigadista cumple un rol fundamental en la construcción de un entorno más seguro, demostrando compromiso, responsabilidad y vocación de servicio hacia sus compañeros y la organización.
            </p>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-left">
                <!-- Tarjeta Misión 1 -->
                <div class="p-8 bg-slate-950 rounded-2xl border border-slate-800 shadow-xl relative group overflow-hidden">
                    <div class="absolute top-0 left-0 w-1 h-full bg-red-600"></div>
                    <div class="text-red-500 text-3xl mb-4"><i class="fa-solid fa-shield-halved"></i></div>
                    <h4 class="font-bold text-xl text-white mb-3" contenteditable="false" data-edit="card-m1-title">Prevención de Riesgos</h4>
                    <p class="text-white-400 text-sm leading-relaxed" contenteditable="false" data-edit="card-m1-desc">
                        Nuestra mejor respuesta es anticiparnos. Realizamos inspecciones semanales y reportamos desvíos de seguridad para evitar accidentes.
                    </p>
                </div>
                <!-- Tarjeta Misión 2 -->
                <div class="p-8 bg-slate-950 rounded-2xl border border-slate-800 shadow-xl relative group overflow-hidden">
                    <div class="absolute top-0 left-0 w-1 h-full bg-amber-500"></div>
                    <div class="text-amber-500 text-3xl mb-4"><i class="fa-solid fa-bolt"></i></div>
                    <h4 class="font-bold text-xl text-white mb-3" contenteditable="false" data-edit="card-m2-title">Respuesta ante Emergencias</h4>
                    <p class="text-white-400 text-sm leading-relaxed" contenteditable="false" data-edit="card-m2-desc">
                        En una crisis, cada segundo cuenta. Estamos organizados para movilizarnos, controlar incidentes en fase inicial y coordinarnos con recursos externos.
                    </p>
                </div>
                <!-- Tarjeta Misión 3 -->
                <div class="p-8 bg-slate-950 rounded-2xl border border-slate-800 shadow-xl relative group overflow-hidden">
                    <div class="absolute top-0 left-0 w-1 h-full bg-red-600"></div>
                    <div class="text-red-500 text-3xl mb-4"><i class="fa-solid fa-heart-pulse"></i></div>
                    <h4 class="font-bold text-xl text-white mb-3" contenteditable="false" data-edit="card-m3-title">Compromiso Coorporativo</h4>
                    <p class="text-white-400 text-sm leading-relaxed" contenteditable="false" data-edit="card-m3-desc">
                        Mantenemos un compromiso con los objetivos corporativos de la organización, contribuyendo activamente a la protección de las personas, la continuidad operacional y el fortalecimiento de una cultura preventiva.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- ÁREAS DE ENTRENAMIENTO / CAPACITACIÓN -->
    <section id="pilares" class="py-24 px-4 sm:px-6 lg:px-8 bg-slate-950">
        <div class="max-w-6xl mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-xs font-bold text-red-500 uppercase tracking-widest mb-3">CONOCIMIENTO INTEGRAL</h2>
                <h3 class="text-3xl sm:text-4xl font-extrabold text-white mb-4" contenteditable="false" data-edit="train-title">Especialidades Técnicas</h3>
                <p class="text-slate-400 max-w-2xl mx-auto font-light text-sm sm:text-base" contenteditable="false" data-edit="train-desc">
                    Al unirte a la brigada, no asumes tareas genéricas. Podrás especializarte en uno o más frentes técnicos de alto rendimiento:
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Tarjeta Especialidad 1 -->
                <div class="bg-gradient-to-b from-slate-900 to-slate-950 p-8 rounded-3xl border border-slate-800 hover:border-red-600/50 transition-all duration-300 flex flex-col justify-between group">
                    <div>
                        <div class="w-14 h-14 bg-red-600/10 text-red-500 rounded-2xl flex items-center justify-center text-2xl font-bold mb-6 group-hover:bg-red-600 group-hover:text-white transition-all duration-300 shadow-inner">
                            <i class="fa-solid fa-fire"></i>
                        </div>
                        <h4 class="text-xl font-bold text-white mb-3" contenteditable="false" data-edit="spec-1-title">Tácticas de Control de Fuego</h4>
                        <p class="text-slate-400 text-sm leading-relaxed mb-6" contenteditable="false" data-edit="spec-1-desc">
                            Manejo avanzado de sistemas hidráulicos de extinción, uso de agentes especiales, ventilación táctica y control de incendios estructurales y químicos.
                        </p>
                    </div>
                    <button onclick="openSpecialtyInfo('fuego')" class="w-full text-center py-2.5 rounded-xl border border-slate-800 text-xs font-semibold text-slate-300 hover:text-white hover:bg-slate-900 transition">
                        Ver plan de estudios
                    </button>
                </div>
                <!-- Tarjeta Especialidad 2 -->
                <div class="bg-gradient-to-b from-slate-900 to-slate-950 p-8 rounded-3xl border border-slate-800 hover:border-amber-500/50 transition-all duration-300 flex flex-col justify-between group">
                    <div>
                        <div class="w-14 h-14 bg-amber-500/10 text-amber-500 rounded-2xl flex items-center justify-center text-2xl font-bold mb-6 group-hover:bg-amber-500 group-hover:text-black transition-all duration-300 shadow-inner">
                            <i class="fa-solid fa-kit-medical"></i>
                        </div>
                        <h4 class="text-xl font-bold text-white mb-3" contenteditable="false" data-edit="spec-2-title">Soporte Vital Prehospitalario</h4>
                        <p class="text-slate-400 text-sm leading-relaxed mb-6" contenteditable="false" data-edit="spec-2-desc">
                            Atención avanzada de trauma, reanimación cardiopulmonar con DEA, control de hemorragias críticas, rescate en altura e inmovilizaciones seguras.
                        </p>
                    </div>
                    <button onclick="openSpecialtyInfo('medico')" class="w-full text-center py-2.5 rounded-xl border border-slate-800 text-xs font-semibold text-slate-300 hover:text-white hover:bg-slate-900 transition">
                        Ver plan de estudios
                    </button>
                </div>
                <!-- Tarjeta Especialidad 3 -->
                <div class="bg-gradient-to-b from-slate-900 to-slate-950 p-8 rounded-3xl border border-slate-800 hover:border-red-600/50 transition-all duration-300 flex flex-col justify-between group">
                    <div>
                        <div class="w-14 h-14 bg-red-600/10 text-red-500 rounded-2xl flex items-center justify-center text-2xl font-bold mb-6 group-hover:bg-red-600 group-hover:text-white transition-all duration-300 shadow-inner">
                            <i class="fa-solid fa-skull-crossbones"></i>
                        </div>
                        <h4 class="text-xl font-bold text-white mb-3" contenteditable="false" data-edit="spec-3-title">Control de Materiales Peligrosos</h4>
                        <p class="text-slate-400 text-sm leading-relaxed mb-6" contenteditable="false" data-edit="spec-3-desc">
                            Respuesta segura a escapes e incidentes químicos, uso correcto de trajes de encapsulado completo (Nivel A, B y C) y decontaminación.
                        </p>
                    </div>
                    <button onclick="openSpecialtyInfo('quimico')" class="w-full text-center py-2.5 rounded-xl border border-slate-800 text-xs font-semibold text-slate-300 hover:text-white hover:bg-slate-900 transition">
                        Ver plan de estudios
                    </button>
                </div>
            </div>
        </div>
    </section>


    <!-- REQUISITOS -->
    <section id="requisitos" class="py-24 px-4 sm:px-6 lg:px-8 bg-slate-950">
        <div class="max-w-5xl mx-auto">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                
                <div>
                    <span class="text-amber-500 uppercase font-bold text-xs tracking-widest block mb-2">QUÉ BUSCAMOS</span>
                    <h3 class="text-3xl sm:text-4xl font-extrabold text-white mb-6" contenteditable="false" data-edit="req-title">Requisitos para Unirte</h3>
                    <p class="text-slate-400 font-light mb-8 leading-relaxed" contenteditable="false" data-edit="req-desc">
                        No requerimos experiencia militar, policial ni médica previa. Nuestro centro de formación se encarga de instruirte desde cero. Buscamos cualidades personales que representen nuestros valores.
                    </p>

                    <div class="space-y-4">
                        <div class="flex items-start space-x-3">
                            <div class="w-6 h-6 rounded-full bg-emerald-500/10 text-emerald-500 flex items-center justify-center flex-shrink-0 mt-0.5">
                                <i class="fa-solid fa-check text-xs"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-200 text-sm sm:text-base">Contrato Activo</h4>
                                <p class="text-xs sm:text-sm text-slate-400">Pertenecer formalmente al staff activo de la compañía en cualquier área u oficina.</p>
                            </div>
                        </div>
                        <div class="flex items-start space-x-3">
                            <div class="w-6 h-6 rounded-full bg-emerald-500/10 text-emerald-500 flex items-center justify-center flex-shrink-0 mt-0.5">
                                <i class="fa-solid fa-check text-xs"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-200 text-sm sm:text-base">Salud Compatible</h4>
                                <p class="text-xs sm:text-sm text-slate-400">Aprobar la evaluación médica ocupacional (revisamos pulso, respiración y compatibilidad física sin costo).</p>
                            </div>
                        </div>
                        <div class="flex items-start space-x-3">
                            <div class="w-6 h-6 rounded-full bg-emerald-500/10 text-emerald-500 flex items-center justify-center flex-shrink-0 mt-0.5">
                                <i class="fa-solid fa-check text-xs"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-200 text-sm sm:text-base">Compromiso con el Entrenamiento</h4>
                                <p class="text-xs sm:text-sm text-slate-400">Disponer de 4 horas mensuales (en horario laboral pagado) para capacitaciones y simulacros.</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Acordeón interactivo de Preguntas Frecuentes -->
                <div class="bg-slate-900 p-6 sm:p-8 rounded-3xl border border-slate-800">
                    <h4 class="text-xl font-bold text-white mb-6">Preguntas Frecuentes</h4>
                    <div class="space-y-4">
                        
                        <div class="border-b border-slate-800 pb-3">
                            <button onclick="toggleAccordion(1)" class="w-full flex justify-between items-center text-left py-2 font-medium text-slate-200 hover:text-white transition-all">
                                <span>¿El entrenamiento ocurre fuera de mi horario?</span>
                                <i id="accordion-icon-1" class="fa-solid fa-chevron-down text-slate-500 text-xs transition-transform"></i>
                            </button>
                            <div id="accordion-content-1" class="hidden pt-2 text-xs sm:text-sm text-slate-400 leading-relaxed">
                                No. Todo el tiempo dedicado a la brigada, entrenamientos externos e internos se contabiliza como horas laborales de trabajo normal y está cubierto por tu seguro corporativo.
                            </div>
                        </div>

                        <div class="border-b border-slate-800 pb-3">
                            <button onclick="toggleAccordion(2)" class="w-full flex justify-between items-center text-left py-2 font-medium text-slate-200 hover:text-white transition-all">
                                <span>¿Hay incentivos para brigadistas?</span>
                                <i id="accordion-icon-2" class="fa-solid fa-chevron-down text-slate-500 text-xs transition-transform"></i>
                            </button>
                            <div id="accordion-content-2" class="hidden pt-2 text-xs sm:text-sm text-slate-400 leading-relaxed">
                                Sí. Además de recibir certificaciones internacionales de primeros auxilios y rescate con validez curricular, los brigadistas reciben un bono de asignación especial según permanencia y prioridad de capacitación.
                            </div>
                        </div>

                        <div class="border-b border-slate-800 pb-3">
                            <button onclick="toggleAccordion(3)" class="w-full flex justify-between items-center text-left py-2 font-medium text-slate-200 hover:text-white transition-all">
                                <span>¿Qué pasa si tengo miedo al fuego o la sangre?</span>
                                <i id="accordion-icon-3" class="fa-solid fa-chevron-down text-slate-500 text-xs transition-transform"></i>
                            </button>
                            <div id="accordion-content-3" class="hidden pt-2 text-xs sm:text-sm text-slate-400 leading-relaxed">
                                Es totalmente normal. Por eso enseñamos de manera progresiva. Si no deseas participar directamente en fuego, puedes capacitarte en soporte vital de oficina, logística o gestión de comunicaciones de emergencia.
                            </div>
                        </div>

                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- FORMULARIO DE POSTULACIÓN -->
    <section id="postular" class="py-24 px-4 sm:px-6 lg:px-8 bg-slate-950 relative border-t border-slate-900">
        <div class="max-w-xl mx-auto relative z-10">
            <div class="text-center mb-10">
                <h3 class="text-3xl font-extrabold text-white mb-3" contenteditable="false" data-edit="form-title">Inicia tu Camino de Honor</h3>
                <p class="text-slate-400 font-light text-sm" contenteditable="false" data-edit="form-desc">Completa este formulario. Tu postulación ingresará inmediatamente a evaluación del Departamento de Prevención.</p>
            </div>

            <!-- Formulario interactivo con almacenamiento local simulado -->
            <form id="brigadeForm" onsubmit="handleFormSubmission(event)" class="bg-slate-900 p-8 sm:p-10 rounded-3xl border border-slate-800 space-y-6 shadow-2xl relative overflow-hidden">
                <div class="absolute top-0 inset-x-0 h-1.5 bg-gradient-to-r from-red-600 via-amber-500 to-red-600"></div>
                
                <div>
                    <label class="block text-xs uppercase tracking-wider font-semibold text-slate-400 mb-2">Nombre Completo</label>
                    <div class="relative">
                        <span class="absolute inset-y-0 left-0 pl-3 flex items-center text-slate-500"><i class="fa-solid fa-user"></i></span>
                        <input id="form-fullname" type="text" required placeholder="Ej: Juan Pérez" class="w-full bg-slate-950 border border-slate-800 rounded-xl pl-10 pr-4 py-3 text-white placeholder-slate-600 focus:outline-none focus:border-red-500 focus:ring-1 focus:ring-red-500 transition-all">
                    </div>
                </div>
                
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-xs uppercase tracking-wider font-semibold text-slate-400 mb-2">Correo Electrónico</label>
                        <div class="relative">
                            <span class="absolute inset-y-0 left-0 pl-3 flex items-center text-slate-500"><i class="fa-solid fa-envelope"></i></span>
                            <input id="form-email" type="email" required placeholder="tu@correo.com" class="w-full bg-slate-950 border border-slate-800 rounded-xl pl-10 pr-4 py-3 text-white placeholder-slate-600 focus:outline-none focus:border-red-500 focus:ring-1 focus:ring-red-500 transition-all">
                        </div>
                    </div>
                    <div>
                        <label class="block text-xs uppercase tracking-wider font-semibold text-slate-400 mb-2">Teléfono Móvil</label>
                        <div class="relative">
                            <span class="absolute inset-y-0 left-0 pl-3 flex items-center text-slate-500"><i class="fa-solid fa-phone"></i></span>
                            <input id="form-phone" type="tel" required placeholder="+569..." class="w-full bg-slate-950 border border-slate-800 rounded-xl pl-10 pr-4 py-3 text-white placeholder-slate-600 focus:outline-none focus:border-red-500 focus:ring-1 focus:ring-red-500 transition-all">
                        </div>
                    </div>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-xs uppercase tracking-wider font-semibold text-slate-400 mb-2">Área de Trabajo</label>
                        <input id="form-department" type="text" required placeholder="Ej: Operaciones / Logística" class="w-full bg-slate-950 border border-slate-800 rounded-xl px-4 py-3 text-white placeholder-slate-600 focus:outline-none focus:border-red-500 focus:ring-1 focus:ring-red-500 transition-all">
                    </div>
                    <div>
                        <label class="block text-xs uppercase tracking-wider font-semibold text-slate-400 mb-2">Preferencia de Rol</label>
                        <select id="form-pref-role" class="w-full bg-slate-950 border border-slate-800 rounded-xl px-4 py-3 text-white focus:outline-none focus:border-red-500 focus:ring-1 focus:ring-red-500 transition-all">
                            <option value="Tácticas de Control de Fuego">Control de Incendios</option>
                            <option value="Soporte Vital Prehospitalario">Primeros Auxilios</option>
                            <option value="Control de Materiales Peligrosos">Incidentes Químicos</option>
                            <option value="Cualquiera">Por determinar en capacitación</option>
                        </select>
                    </div>
                </div>

                <div>
                    <label class="block text-xs uppercase tracking-wider font-semibold text-slate-400 mb-2">¿Tienes algún entrenamiento previo?</label>
                    <textarea id="form-prev-exp" rows="2" placeholder="Ej: Cruz roja, Boy scouts, o ninguno..." class="w-full bg-slate-950 border border-slate-800 rounded-xl px-4 py-3 text-white placeholder-slate-600 focus:outline-none focus:border-red-500 focus:ring-1 focus:ring-red-500 transition-all resize-none"></textarea>
                </div>

                <button type="submit" class="w-full bg-red-600 hover:bg-red-700 text-white font-bold py-4 rounded-xl shadow-lg shadow-red-600/30 transition-all transform hover:-translate-y-0.5 flex justify-center items-center space-x-2">
                    <i class="fa-solid fa-paper-plane"></i>
                    <span>Enviar Postulación Militar / Civil</span>
                </button>
            </form>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-slate-950 py-12 px-4 sm:px-6 lg:px-8 border-t border-slate-900 text-center">
        <div class="max-w-4xl mx-auto">
            <div class="flex justify-center space-x-6 mb-6">
                <span class="text-slate-600 hover:text-red-500 transition-all"><i class="fa-brands fa-instagram text-lg"></i></span>
                <span class="text-slate-600 hover:text-red-500 transition-all"><i class="fa-brands fa-facebook text-lg"></i></span>
                <span class="text-slate-600 hover:text-red-500 transition-all"><i class="fa-brands fa-youtube text-lg"></i></span>
            </div>
            <p class="text-xs text-slate-500" contenteditable="false" data-edit="footer-c1">&copy; 2026 Departamento de Prevención y Control de Incendios (PCI).</p>
            <p class="text-[10px] text-slate-600 mt-1" contenteditable="false" data-edit="footer-c2">Este sitio web autogestionado actúa como canal de captación de brigadas industriales.</p>
        </div>
    </footer>

    <!-- MODAL DE INFORMACIÓN DE ESPECIALIDAD -->
    <div id="info-modal" class="fixed inset-0 bg-black/80 flex items-center justify-center p-4 z-50 hidden backdrop-blur-sm">
        <div class="bg-slate-900 border border-slate-800 w-full max-w-lg rounded-3xl overflow-hidden shadow-2xl relative">
            <div class="p-6 sm:p-8">
                <div class="flex justify-between items-start mb-6">
                    <div class="flex items-center space-x-3">
                        <div id="modal-badge-container" class="w-10 h-10 rounded-xl flex items-center justify-center text-lg">
                            <i id="modal-icon" class="fa-solid fa-fire"></i>
                        </div>
                        <div>
                            <h4 id="modal-title" class="text-xl font-bold text-white">Especialidad</h4>
                            <span id="modal-subtitle" class="text-[10px] uppercase font-bold text-slate-500 tracking-wider">Plan de formación</span>
                        </div>
                    </div>
                    <button onclick="closeModal('info-modal')" class="text-slate-400 hover:text-white"><i class="fa-solid fa-xmark text-lg"></i></button>
                </div>
                
                <div class="space-y-4 mb-6">
                    <p id="modal-description" class="text-sm text-slate-400 leading-relaxed"></p>
                    <div class="bg-slate-950 p-4 rounded-2xl border border-slate-800">
                        <h5 class="text-xs font-bold text-slate-300 uppercase tracking-widest mb-2"><i class="fa-solid fa-list-check mr-1.5 text-red-500"></i>Temas del Entrenamiento</h5>
                        <ul id="modal-topics" class="text-xs text-slate-400 space-y-1.5 pl-5 list-disc"></ul>
                    </div>
                </div>

                <div class="flex justify-end">
                    <button onclick="closeModal('info-modal')" class="bg-slate-800 hover:bg-slate-700 text-slate-200 font-bold px-5 py-2.5 rounded-xl text-sm transition">
                        Entendido
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- MODAL DE ÉXITO DE REGISTRO -->
    <div id="success-modal" class="fixed inset-0 bg-black/80 flex items-center justify-center p-4 z-50 hidden backdrop-blur-sm">
        <div class="bg-slate-900 border border-slate-800 w-full max-w-md rounded-3xl overflow-hidden shadow-2xl relative text-center">
            <div class="p-8">
                <div class="w-16 h-16 bg-emerald-500/10 text-emerald-500 rounded-full flex items-center justify-center mx-auto mb-6 text-3xl">
                    <i class="fa-solid fa-circle-check"></i>
                </div>
                <h4 class="text-2xl font-bold mb-2 text-white">¡Postulación Recibida!</h4>
                <p class="text-sm text-slate-400 mb-6">Tu perfil ha sido guardado exitosamente. Un prevencionista del comité de emergencias evaluará tu ficha y se contactará contigo para coordinar la inducción inicial.</p>
                
                <button onclick="closeModal('success-modal')" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3 rounded-xl text-sm transition shadow-lg shadow-emerald-600/20">
                    Cerrar Ventana
                </button>
            </div>
        </div>
    </div>

    <!-- PANEL ADJUNTO: ADMINISTRACIÓN Y EDICIÓN -->
    <div id="admin-panel" class="fixed bottom-6 right-6 z-50 max-w-sm w-full bg-slate-900 border border-slate-800 rounded-3xl shadow-2xl hidden overflow-hidden">
        <!-- Encabezado del Panel -->
        <div class="bg-slate-950 p-4 border-b border-slate-800 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <i class="fa-solid fa-screwdriver-wrench text-red-500"></i>
                <span class="font-bold text-xs tracking-wider uppercase">Centro de Control de OnePage</span>
            </div>
            <button onclick="toggleAdminPanel()" class="text-slate-400 hover:text-white"><i class="fa-solid fa-xmark"></i></button>
        </div>
        
        <!-- Cuerpo del Panel con Tabs -->
        <div class="p-5 space-y-5 max-h-[400px] overflow-y-auto no-scrollbar">
            <!-- Sección Modo Editor -->
            <div class="bg-slate-950/50 p-4 rounded-2xl border border-slate-800">
                <div class="flex items-center justify-between mb-3">
                    <h5 class="text-xs font-bold text-slate-300 uppercase tracking-widest">Edición Visual</h5>
                    <span id="editor-status" class="text-[9px] font-bold text-amber-500 uppercase px-2 py-0.5 rounded-md bg-amber-500/10 border border-amber-500/20">Inactivo</span>
                </div>
                <p class="text-[11px] text-slate-400 leading-relaxed mb-4">Activa esta opción para poder hacer clic y editar directamente los textos de la página en tiempo real antes de exportarla.</p>
                <button id="toggle-edit-btn" onclick="toggleEditMode()" class="w-full py-2.5 rounded-xl bg-red-600 hover:bg-red-700 text-white font-bold text-xs transition flex justify-center items-center space-x-1.5">
                    <i class="fa-solid fa-pen-to-square"></i>
                    <span>Activar Edición Libre</span>
                </button>
            </div>

            <!-- Sección Exportador -->
            <div class="bg-slate-950/50 p-4 rounded-2xl border border-slate-800">
                <h5 class="text-xs font-bold text-slate-300 uppercase tracking-widest mb-1">Exportar OnePage</h5>
                <p class="text-[11px] text-slate-400 leading-relaxed mb-4">Descarga una copia limpia del archivo HTML con todos los cambios textuales que realizaste.</p>
                <button onclick="exportModifiedHTML()" class="w-full py-2.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-200 hover:text-white font-bold text-xs border border-slate-700 transition flex justify-center items-center space-x-1.5">
                    <i class="fa-solid fa-download"></i>
                    <span>Descargar index.html Editado</span>
                </button>
            </div>

            <!-- Sección de Solicitudes Recibidas (Persistidas en LocalStorage) -->
            <div class="bg-slate-950/50 p-4 rounded-2xl border border-slate-800">
                <div class="flex justify-between items-center mb-2">
                    <h5 class="text-xs font-bold text-slate-300 uppercase tracking-widest">Postulantes (<span id="count-applications">0</span>)</h5>
                    <button onclick="clearApplications()" class="text-[9px] text-red-400 hover:text-red-300 uppercase">Limpiar</button>
                </div>
                <div id="applications-container" class="space-y-2 text-[11px] text-slate-400 max-h-[120px] overflow-y-auto no-scrollbar">
                    <p class="italic text-slate-600 text-center py-2">No hay postulantes registrados aún.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // Variables de estado global
        let editModeActive = false;

        // Base de Datos en Memoria de Especialidades
        const specialtyDatabase = {
            fuego: {
                title: "Tácticas de Control de Fuego",
                colorClass: "bg-red-600/15 text-red-500 border border-red-500/20",
                icon: "fa-fire",
                description: "Este programa te especializa en el combate de fuegos estructurales, líquidos inflamables e incendios de gases. Recibirás adiestramiento con equipos de respiración autónoma (ERA) y despliegue rápido de líneas de agua.",
                topics: [
                    "Teoría del fuego y termodinámica básica",
                    "Uso y dosificación correcta de agentes extintores químicos",
                    "Cálculo de pérdidas por fricción en sistemas hidráulicos",
                    "Apertura forzada de accesos y ventilación forzada",
                    "Estrategias de búsqueda y rescate en estructuras colapsadas"
                ]
            },
            medico: {
                title: "Soporte Vital Prehospitalario",
                colorClass: "bg-amber-500/15 text-amber-500 border border-amber-500/20",
                icon: "fa-kit-medical",
                description: "Especialización enfocada en la preservación de la vida en entornos industriales. Aprenderás a diagnosticar rápidamente lesiones bajo presión y administrar maniobras críticas prehospitalarias.",
                topics: [
                    "Soporte Vital Básico (SVB) y uso del Desfibrilador (DEA)",
                    "Protocolos de Control de Hemorragias Masivas (Torniquetes)",
                    "Manejo de la vía aérea básica y oxigenoterapia",
                    "Clasificación masiva de heridos en catástrofes (Método START/Triage)",
                    "Inmovilización espinal y traslado seguro en camillas rígidas"
                ]
            },
            quimico: {
                title: "Control de Materiales Peligrosos",
                colorClass: "bg-emerald-500/15 text-emerald-500 border border-emerald-500/20",
                icon: "fa-skull-crossbones",
                description: "Te prepararás para enfrentar escenarios con derrames químicos corrosivos, fugas de gases nocivos e incidentes de contaminación industrial. Se enseña el uso de equipamiento de aislamiento completo.",
                topics: [
                    "Sustancias químicas peligrosas según sistema globalmente armonizado",
                    "Uso de trajes de protección química Nivel A (Encapsulados)",
                    "Estrategias de contención pasiva (Diques y Absorbentes)",
                    "Construcción y operación de líneas de descontaminación de campo",
                    "Toma de muestras operacionales de toxicidad ambiental"
                ]
            }
        };

        // Inicialización en Carga del Documento
        window.onload = function() {
            loadApplications();
        };

        // --- SISTEMA DEL ACORDEÓN ---
        function toggleAccordion(id) {
            const content = document.getElementById(`accordion-content-${id}`);
            const icon = document.getElementById(`accordion-icon-${id}`);
            if (content.classList.contains('hidden')) {
                content.classList.remove('hidden');
                icon.classList.add('rotate-180');
            } else {
                content.classList.add('hidden');
                icon.classList.remove('rotate-180');
            }
        }

        // --- SISTEMA DE MODALES ---
        function openSpecialtyInfo(key) {
            const data = specialtyDatabase[key];
            if (!data) return;

            document.getElementById('modal-title').innerText = data.title;
            document.getElementById('modal-description').innerText = data.description;
            
            // Reconstruir lista de temas
            const topicsContainer = document.getElementById('modal-topics');
            topicsContainer.innerHTML = '';
            data.topics.forEach(topic => {
                const li = document.createElement('li');
                li.innerText = topic;
                topicsContainer.appendChild(li);
            });

            // Ajustar iconos e insignias
            const badge = document.getElementById('modal-badge-container');
            const icon = document.getElementById('modal-icon');
            badge.className = `w-10 h-10 rounded-xl flex items-center justify-center text-lg ${data.colorClass}`;
            icon.className = `fa-solid ${data.icon}`;

            document.getElementById('info-modal').classList.remove('hidden');
        }

        function closeModal(id) {
            document.getElementById(id).classList.add('hidden');
        }

        // --- SISTEMA DE FORMULARIO & PERSISTENCIA LOCAL DE SOLICITUDES ---
        function handleFormSubmission(event) {
            event.preventDefault();

            const applicant = {
                id: Date.now(),
                fullname: document.getElementById('form-fullname').value,
                email: document.getElementById('form-email').value,
                phone: document.getElementById('form-phone').value,
                department: document.getElementById('form-department').value,
                role: document.getElementById('form-pref-role').value,
                prevExperience: document.getElementById('form-prev-exp').value || "Ninguno",
                date: new Date().toLocaleDateString()
            };

            // Cargar existentes
            let currentApps = [];
            try {
                currentApps = JSON.parse(localStorage.getItem('brigade_applications') || '[]');
            } catch (e) {
                currentApps = [];
            }

            // Agregar nuevo
            currentApps.push(applicant);
            localStorage.setItem('brigade_applications', JSON.stringify(currentApps));

            // Actualizar interfaz del panel
            loadApplications();

            // Limpiar formulario y mostrar éxito
            document.getElementById('brigadeForm').reset();
            document.getElementById('success-modal').classList.remove('hidden');
        }

        function loadApplications() {
            let list = [];
            try {
                list = JSON.parse(localStorage.getItem('brigade_applications') || '[]');
            } catch (e) {
                list = [];
            }

            // Actualizar contador
            document.getElementById('count-applications').innerText = list.length;

            const container = document.getElementById('applications-container');
            container.innerHTML = '';

            if (list.length === 0) {
                container.innerHTML = '<p class="italic text-slate-600 text-center py-2">No hay postulantes registrados aún.</p>';
                return;
            }

            // Generar tarjetas para la consola admin
            list.forEach(app => {
                const item = document.createElement('div');
                item.className = "p-3 bg-slate-950 rounded-xl border border-slate-800 space-y-1";
                item.innerHTML = `
                    <div class="flex justify-between font-bold text-white text-[10px]">
                        <span>${app.fullname}</span>
                        <span class="text-red-500">${app.date}</span>
                    </div>
                    <div class="text-[9px] text-slate-400">
                        <span class="block"><strong>Dept:</strong> ${app.department} | <strong>Rol:</strong> ${app.role}</span>
                        <span class="block"><strong>Tel:</strong> ${app.phone}</span>
                    </div>
                `;
                container.appendChild(item);
            });
        }

        function clearApplications() {
            localStorage.removeItem('brigade_applications');
            loadApplications();
        }

        // --- INTERFAZ DEL PANEL DE CONTROL DE EDICIÓN ---
        function toggleAdminPanel() {
            const panel = document.getElementById('admin-panel');
            if (panel.classList.contains('hidden')) {
                panel.classList.remove('hidden');
            } else {
                panel.classList.add('hidden');
            }
        }

        // --- MOTOR DE EDICIÓN VISUAL DIRECTA (CONTENTEDITABLE) ---
        function toggleEditMode() {
            editModeActive = !editModeActive;
            const body = document.body;
            const btn = document.getElementById('toggle-edit-btn');
            const statusLabel = document.getElementById('editor-status');

            if (editModeActive) {
                body.classList.add('editable-active');
                
                // Activar contenteditable en todos los nodos marcados como editables
                document.querySelectorAll('[data-edit]').forEach(el => {
                    el.setAttribute('contenteditable', 'true');
                });

                // Cambiar estética de botones
                btn.innerHTML = '<i class="fa-solid fa-lock"></i> <span>Desactivar Edición</span>';
                btn.classList.replace('bg-red-600', 'bg-amber-600');
                btn.classList.replace('hover:bg-red-700', 'hover:bg-amber-700');
                
                statusLabel.innerText = "Activo";
                statusLabel.className = "text-[9px] font-bold text-emerald-500 uppercase px-2 py-0.5 rounded-md bg-emerald-500/10 border border-emerald-500/20";
            } else {
                body.classList.remove('editable-active');
                
                // Apagar el atributo editable
                document.querySelectorAll('[data-edit]').forEach(el => {
                    el.setAttribute('contenteditable', 'false');
                });

                // Restaurar estética original
                btn.innerHTML = '<i class="fa-solid fa-pen-to-square"></i> <span>Activar Edición Libre</span>';
                btn.classList.replace('bg-amber-600', 'bg-red-600');
                btn.classList.replace('hover:bg-amber-700', 'hover:bg-red-700');

                statusLabel.innerText = "Inactivo";
                statusLabel.className = "text-[9px] font-bold text-amber-500 uppercase px-2 py-0.5 rounded-md bg-amber-500/10 border border-amber-500/20";
            }
        }

        // --- FUNCIÓN DE EXPORTACIÓN CLEAN HTML ---
        function exportModifiedHTML() {
            // Asegurarnos de apagar la edición activa para que no exporte los bordes punteados
            if (editModeActive) {
                toggleEditMode();
            }

            // Ocultar temporalmente el panel admin para que no interfiera en el HTML final exportado
            const adminPanel = document.getElementById('admin-panel');
            const wasHidden = adminPanel.classList.contains('hidden');
            adminPanel.classList.add('hidden');

            // Obtener el HTML limpio de todo el documento
            let docHTML = "<!DOCTYPE html>\n" + document.documentElement.outerHTML;

            // Si estaba abierto el panel antes de exportar, lo volvemos a poner como estaba en la vista del usuario
            if (!wasHidden) {
                adminPanel.classList.remove('hidden');
            }

            // Crear Blob y detonar la descarga local
            const blob = new Blob([docHTML], { type: 'text/html' });
            const tempLink = document.createElement('a');
            tempLink.href = URL.createObjectURL(blob);
            tempLink.download = 'brigada-emergencia-editada.html';
            document.body.appendChild(tempLink);
            tempLink.click();
            document.body.removeChild(tempLink);
        }
    </script>
</body>
</html>
