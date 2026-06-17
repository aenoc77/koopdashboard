<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Estratégico KOOP v7.0</title>
    <style>
        /* Paleta Cromática Premium [cite: 106, 108, 110, 111] */
        :root {
            --verde-bosque: #0B3C35;
            --blanco-tiza: #F7F5F0;
            --gris-grafito: #222222;
            --oro-viejo: #D4AF37;
            --terracota: #C87A53;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--blanco-tiza);
            color: var(--gris-grafito);
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        header {
            background-color: var(--verde-bosque);
            color: var(--blanco-tiza);
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 5px solid var(--oro-viejo);
        }

        header h1 {
            margin: 0;
            font-size: 1.8rem;
            letter-spacing: 1px;
        }

        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }

        /* Navegación por Pestañas */
        .tabs {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
            border-bottom: 2px solid var(--verde-bosque);
            padding-bottom: 10px;
        }

        .tab-btn {
            background-color: transparent;
            border: none;
            color: var(--gris-grafito);
            font-size: 1.1rem;
            font-weight: bold;
            padding: 10px 20px;
            cursor: pointer;
            transition: all 0.3s ease;
            border-radius: 5px 5px 0 0;
        }

        .tab-btn.active {
            background-color: var(--verde-bosque);
            color: var(--blanco-tiza);
        }

        .tab-btn:hover:not(.active) {
            background-color: #e0ded9;
        }

        /* Contenido de las Pestañas */
        .tab-content {
            display: none;
            background-color: #ffffff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            border-left: 4px solid var(--oro-viejo);
        }

        .tab-content.active {
            display: block;
        }

        h2 {
            color: var(--verde-bosque);
            margin-top: 0;
        }

        /* Tarjetas de Información */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .card {
            background-color: var(--blanco-tiza);
            border: 1px solid #e0ded9;
            padding: 20px;
            border-radius: 6px;
            border-top: 4px solid var(--terracota);
        }

        .card h3 {
            margin-top: 0;
            color: var(--verde-bosque);
        }

        .highlight {
            font-weight: bold;
            color: var(--terracota);
        }
        
        .metric-value {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--verde-bosque);
            margin: 10px 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>KOOP Technologies S.A.</h1>
        <span style="font-weight: bold; color: var(--oro-viejo);">Alineación Estratégica v7.0 [cite: 36]</span>
    </header>

    <div class="container">
        <div class="tabs">
            <button class="tab-btn active" onclick="openTab('ruta')">🚀 Hoja de Ruta</button>
            <button class="tab-btn" onclick="openTab('sandbox')">📊 Sandbox Regulatorio</button>
            <button class="tab-btn" onclick="openTab('modelo')">⚙️ Ingeniería Financiera</button>
        </div>

        <div id="ruta" class="tab-content active">
            <h2>Pipeline Crítico de Lanzamiento [cite: 67]</h2>
            <p>Acciones planificadas para cumplir con el Sandbox institucional supervisado por el Regulador Cripto[cite: 11].</p>
            
            <div class="card-grid">
                <div class="card">
                    <h3>Fase 1: Preparación (Días 1-30)</h3>
                    <p>Integración de firmas digitales para contratos de mandato, APIs de KYC biométrico y pruebas del trigger PostgreSQL[cite: 67].</p>
                </div>
                <div class="card">
                    <h3>Fase 2: Expediente Institucional (Días 31-45)</h3>
                    <p>Presentación formal de KOOP Technologies S.A. ante el Regulador Cripto, respaldada por la corporación Epignosis[cite: 68].</p>
                </div>
                <div class="card">
                    <h3>Fase 3: Mesa Técnica (Días 46-60)</h3>
                    <p>Demostración en vivo de los contratos inteligentes, billeteras Safe y la consola exclusiva para el "Súper Auditor Gubernamental"[cite: 69].</p>
                </div>
                <div class="card" style="border-top-color: var(--oro-viejo);">
                    <h3>Fase 4: Lanzamiento (Día 61+)</h3>
                    <p>Despliegue oficial de la aplicación móvil Android para los primeros 100 usuarios confinados en el Sandbox[cite: 70].</p>
                </div>
            </div>
        </div>

        <div id="sandbox" class="tab-content">
            <h2>Parámetros de Confinamiento del Sandbox</h2>
            <p>Límites duros forzados de forma estricta por el software en producción para blindar a la corporación durante la validación del MVP[cite: 62].</p>
            
            <div class="card-grid">
                <div class="card">
                    <h3>Tope de Usuarios Piloto</h3>
                    <div class="metric-value">Máximo 100</div>
                    <p>Usuarios verificados permitidos. Completado el cupo, las Edge Functions denegarán nuevos registros[cite: 62, 63].</p>
                </div>
                <div class="card">
                    <h3>Techo de TVL en Bóveda</h3>
                    <div class="metric-value">$50,000 USDC</div>
                    <p>Límite acumulativo. Cualquier exceso rebotará de forma inmediata en la rampa fiduciaria local[cite: 64, 65].</p>
                </div>
                <div class="card">
                    <h3>Límite Transaccional</h3>
                    <div class="metric-value">$500 USDC / mes</div>
                    <p>Restricción mensual por usuario para movilizar, ahorrar o financiarse[cite: 66].</p>
                </div>
            </div>
        </div>

        <div id="modelo" class="tab-content">
            <h2>El Split de Intereses Inmutable (50/30/20)</h2>
            <p>Modelo validado en el plan de negocio v7.0 y blindado contractualmente en el código final de Solidity[cite: 7, 8].</p>
            
            <div class="card-grid">
                <div class="card">
                    <h3>Soporte Técnico / Operativo</h3>
                    <div class="metric-value">50%</div>
                    <p>Porción que se destina a la rentabilidad de la empresa (KOOP)[cite: 7].</p>
                </div>
                <div class="card">
                    <h3>Rendimiento de Socios</h3>
                    <div class="metric-value">30%</div>
                    <p>Devolución al pozo común de los socios aportantes[cite: 7, 86].</p>
                </div>
                <div class="card">
                    <h3>Fondo de Reserva Técnica</h3>
                    <div class="metric-value">20%</div>
                    <p>Inmovilizado por código para robustecer la cobertura contra riesgos de mora[cite: 7, 103].</p>
                </div>
            </div>
        </div>

    </div>

    <script>
        function openTab(tabName) {
            // Ocultar todos los contenidos de pestaña
            var i, tabcontent, tablinks;
            tabcontent = document.getElementsByClassName("tab-content");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
                tabcontent[i].classList.remove("active");
            }

            // Desactivar todos los botones
            tablinks = document.getElementsByClassName("tab-btn");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].classList.remove("active");
            }

            // Mostrar la pestaña actual y añadir clase active al botón
            document.getElementById(tabName).style.display = "block";
            document.getElementById(tabName).classList.add("active");
            event.currentTarget.classList.add("active");
        }
    </script>
</body>
</html>
