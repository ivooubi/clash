<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CLASH.DATA</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
            color: #ffffff;
        }

        body {
            background-color: #1a1a1a;
            line-height: 1.6;
        }

        header {
            background-color: #2c2c2c;
            padding: 20px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(255, 255, 255, 0.1);
        }

        header h1 {
            font-size: 3rem;
            font-weight: 600;
            color: #ffffff;
            text-transform: uppercase;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
        }

        nav {
            margin: 20px 0;
        }

        nav a {
            color: #ffffff;
            text-decoration: none;
            margin: 0 20px;
            font-weight: 400;
            font-size: 1.2rem;
            text-transform: uppercase;
            text-shadow: 0 0 8px rgba(255, 255, 255, 0.5);
            transition: transform 0.3s ease, opacity 0.3s ease;
        }

        nav a:hover {
            transform: scale(1.1);
            opacity: 0.8;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .game-info {
            background-color: #2c2c2c;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 30px;
            box-shadow: 0 2px 8px rgba(255, 255, 255, 0.05);
            animation: fadeIn 1s ease-in;
        }

        .game-info h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
        }

        .game-info p, .game-info ul {
            color: #e0e0e0;
        }

        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .card {
            background-color: #2c2c2c;
            border-radius: 8px;
            padding: 15px;
            box-shadow: 0 2px 8px rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 12px rgba(255, 255, 255, 0.15);
        }

        .card h3 {
            font-size: 1.2rem;
            margin: 10px 0;
        }

        .card p {
            font-size: 0.9rem;
            color: #e0e0e0;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #2c2c2c;
            margin-top: 30px;
            box-shadow: 0 -2px 4px rgba(255, 255, 255, 0.1);
        }

        footer p {
            font-size: 0.9rem;
            color: #e0e0e0;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 600px) {
            header h1 {
                font-size: 2rem;
            }

            .game-info h2 {
                font-size: 1.5rem;
            }

            .cards-grid {
                grid-template-columns: 1fr;
            }

            nav a {
                font-size: 1rem;
                margin: 0 10px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>CLASH.DATA</h1>
        <nav>
            <a href="#info">INFORMACIÓN</a>
            <a href="#cards">CARTAS</a>
        </nav>
    </header>

    <div class="container">
        <section id="info" class="game-info">
            <h2>Sobre Clash Royale</h2>
            <p>
                Clash Royale es un juego de estrategia móvil en tiempo real desarrollado por Supercell. Combina elementos de juegos de cartas, defensa de torres y batallas multijugador. Los jugadores construyen mazos con cartas que representan tropas, hechizos y edificios, y luchan en partidas 1v1 o 2v2 para destruir las torres enemigas mientras protegen las propias. El juego destaca por su jugabilidad estratégica, gráficos coloridos y animaciones fluidas que crean una experiencia inmersiva. Gestiona tu elixir sabiamente y mejora tus cartas para ascender en las clasificaciones.
            </p>
            <p>
                Características principales:
                <ul>
                    <li>Recoge y mejora 123 cartas únicas.</li>
                    <li>Combate en tiempo real contra jugadores de todo el mundo.</li>
                    <li>Gestiona el elixir para desplegar tropas y hechizos estratégicamente.</li>
                </ul>
            </p>
        </section>

        <section id="cards">
            <h2>Cartas de Clash Royale</h2>
            <div class="cards-grid" id="cards-grid">
                <!-- Cartas de ejemplo -->
                <div class="card">
                    <h3>MONTAPUERCOS</h3>
                    <p><strong>Tipo:</strong> Tropa</p>
                    <p><strong>Costo de Elixir:</strong> 4</p>
                    <p><strong>Nivel Máximo:</strong> 14</p>
                    <p><strong>Descripción:</strong> Tropa rápida que ataca edificios, ideal para ataques directos a torres.</p>
                </div>
                <div class="card">
                    <h3>BOLA DE FUEGO</h3>
                    <p><strong>Tipo:</strong> Hechizo</p>
                    <p><strong>Costo de Elixir:</strong> 4</p>
                    <p><strong>Nivel Máximo:</strong> 14</p>
                    <p><strong>Descripción:</strong> Inflige daño en área, efectiva contra grupos de tropas y estructuras.</p>
                </div>
                <div class="card">
                    <h3>MOSQUETERA</h3>
                    <p><strong>Tipo:</strong> Tropa</p>
                    <p><strong>Costo de Elixir:</strong> 4</p>
                    <p><strong>Nivel Máximo:</strong> 14</p>
                    <p><strong>Descripción:</strong> Tropa de rango que dispara a objetivos terrestres y aéreos.</p>
                </div>
                <!-- Más cartas se cargan dinámicamente -->
            </div>
        </section>
    </div>

    <footer>
        <p>© 2025 clash.data - Todos los derechos reservados</p>
    </footer>

    <script>
        // Lista completa de cartas con descripciones personalizadas
        const cardsData = [
            { name: "Montapuercos", type: "Tropa", elixir: 4, maxLevel: 14, description: "Tropa rápida que ataca edificios, ideal para ataques directos a torres." },
            { name: "Bola de Fuego", type: "Hechizo", elixir: 4, maxLevel: 14, description: "Inflige daño en área, efectiva contra grupos de tropas y estructuras." },
            { name: "Mosquetera", type: "Tropa", elixir: 4, maxLevel: 14, description: "Tropa de rango que dispara a objetivos terrestres y aéreos." },
            { name: "Jefe Bandida", type: "Tropa (Campeón)", elixir: 6, maxLevel: 14, description: "Atacante cuerpo a cuerpo que embiste, se vuelve invisible y retrocede para esquivar ataques." },
            { name: "Bruja", type: "Tropa", elixir: 5, maxLevel: 14, description: "Invoca esqueletos periódicamente y ataca con magia a distancia." },
            { name: "Gigante Rúnico", type: "Tropa", elixir: 6, maxLevel: 14, description: "Tropa tanque que potencia el daño de unidades cercanas con su aura rúnica." },
            { name: "Berserker", type: "Tropa", elixir: 4, maxLevel: 14, description: "Ataca rápidamente, ideal contra enjambres y unidades medianas." },
            { name: "Arquera Mágica", type: "Tropa (Legendaria)", elixir: 4, maxLevel: 14, description: "Dispara flechas que atraviesan múltiples enemigos a distancia." },
            { name: "Goblinstein", type: "Tropa (Campeón)", elixir: 5, maxLevel: 14, description: "Campeón con habilidad de relámpago que daña y aturde enemigos cercanos." },
            { name: "Esqueletos", type: "Tropa", elixir: 1, maxLevel: 14, description: "Tres esqueletos frágiles pero baratos, perfectos para distracciones o ciclado de mazo." },
            { name: "Flechas", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Hechizo que elimina enjambres de tropas terrestres y aéreas en un área grande." },
            { name: "Caballero", type: "Tropa", elixir: 3, maxLevel: 14, description: "Tropa cuerpo a cuerpo con buena salud y daño moderado, ideal como mini-tanque." },
            { name: "Espíritu Eléctrico", type: "Tropa", elixir: 1, maxLevel: 14, description: "Unidad barata que aturde y daña unidades cercanas al saltar." },
            { name: "Zap", type: "Hechizo", elixir: 2, maxLevel: 14, description: "Hechizo de bajo costo que aturde y daña ligeramente en un área pequeña." },
            { name: "Ejército de Esqueletos", type: "Tropa", elixir: 3, maxLevel: 14, description: "Invoca un grupo de esqueletos para abrumar al enemigo o distraer tropas." },
            { name: "Cañón", type: "Edificio", elixir: 3, maxLevel: 14, description: "Edificio defensivo que dispara a tropas terrestres con alta velocidad." },
            { name: "Guardias", type: "Tropa", elixir: 3, maxLevel: 14, description: "Tres esqueletos con escudos, resistentes a hechizos y ataques de área." },
            { name: "Barril de Bárbaro", type: "Hechizo", elixir: 2, maxLevel: 14, description: "Lanza un barril que libera un bárbaro al romperse, ideal para distracciones." },
            { name: "Valquiria", type: "Tropa", elixir: 4, maxLevel: 14, description: "Ataca en área con un giro, perfecta contra enjambres de tropas terrestres." },
            { name: "Pescador", type: "Tropa", elixir: 3, maxLevel: 14, description: "Tropa que usa su ancla para atraer enemigos y atacar con daño moderado." },
            { name: "Gigante Real", type: "Tropa", elixir: 6, maxLevel: 14, description: "Tropa tanque con un cañón que dispara a objetivos terrestres y aéreos." },
            { name: "Bombardero", type: "Tropa", elixir: 2, maxLevel: 14, description: "Lanza bombas que infligen daño en área a tropas terrestres." },
            { name: "Tornado", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Atrae tropas y edificios a un punto, ideal para combinar con hechizos de área." },
            { name: "Bola de Nieve Gigante", type: "Hechizo", elixir: 2, maxLevel: 14, description: "Lanza una bola de nieve que daña y empuja a las tropas enemigas." },
            { name: "Barril de Duendes", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Lanza un barril que libera duendes para atacar torres o tropas." },
            { name: "Arqueros", type: "Tropa", elixir: 3, maxLevel: 14, description: "Dos arqueros que atacan a distancia a objetivos terrestres y aéreos." },
            { name: "Lanzadardos", type: "Tropa", elixir: 3, maxLevel: 14, description: "Tropa de rango que dispara dardos rápidos a objetivos individuales." },
            { name: "Tesla", type: "Edificio", elixir: 4, maxLevel: 14, description: "Torre defensiva que ataca con electricidad y se oculta cuando no dispara." },
            { name: "Murciélagos", type: "Tropa", elixir: 2, maxLevel: 14, description: "Cinco murciélagos voladores que atacan rápidamente a tropas y edificios." },
            { name: "Ejecutor", type: "Tropa", elixir: 5, maxLevel: 14, description: "Lanza un hacha que regresa, infligiendo daño en área en su trayectoria." },
            { name: "Fantasma Real", type: "Tropa (Legendaria)", elixir: 3, maxLevel: 14, description: "Se vuelve invisible hasta atacar, ideal para emboscadas." },
            { name: "Mago de Hielo", type: "Tropa (Legendaria)", elixir: 3, maxLevel: 14, description: "Ralentiza enemigos con ataques de hielo, efectivo para control." },
            { name: "Tumba", type: "Edificio", elixir: 3, maxLevel: 14, description: "Invoca esqueletos periódicamente para distraer o atacar enemigos." },
            { name: "Cerdos Reales", type: "Tropa", elixir: 5, maxLevel: 14, description: "Cuatro cerdos rápidos que atacan edificios, ideales para asaltos." },
            { name: "Monje", type: "Tropa (Campeón)", elixir: 5, maxLevel: 14, description: "Refleja hechizos y ataca con un combo de golpes poderosos." },
            { name: "Chispitas", type: "Tropa", elixir: 6, maxLevel: 14, description: "Dispara un rayo que se recarga, infligiendo daño masivo a un solo objetivo." },
            { name: "Príncipe", type: "Tropa", elixir: 5, maxLevel: 14, description: "Carga con su lanza, causando el doble de daño al embestir." },
            { name: "Sabueso de Lava", type: "Tropa (Legendaria)", elixir: 7, maxLevel: 14, description: "Tanque volador que libera cachorros de lava al ser destruido." },
            { name: "Ballesta", type: "Edificio", elixir: 6, maxLevel: 14, description: "Dispara flechas de largo alcance, ideal para atacar torres enemigas." },
            { name: "Duendes", type: "Tropa", elixir: 2, maxLevel: 14, description: "Tres duendes rápidos que atacan cuerpo a cuerpo con daño moderado." },
            { name: "Reclutas Reales", type: "Tropa", elixir: 7, maxLevel: 14, description: "Seis soldados con escudos que atacan en formación." },
            { name: "Reina Arquera", type: "Tropa (Campeón)", elixir: 5, maxLevel: 14, description: "Dispara flechas a distancia y se vuelve invisible con su habilidad." },
            { name: "Gigante", type: "Tropa", elixir: 5, maxLevel: 14, description: "Tanque terrestre con alta salud que ataca edificios." },
            { name: "Terremoto", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Daña edificios y ralentiza tropas en un área específica." },
            { name: "Mortero", type: "Edificio", elixir: 4, maxLevel: 14, description: "Dispara proyectiles de largo alcance que dañan tropas terrestres y edificios." },
            { name: "Entrega Real", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Lanza un barril que invoca reclutas reales al romperse." },
            { name: "Gólem de Hielo", type: "Tropa", elixir: 2, maxLevel: 14, description: "Tropa con baja salud que ralentiza enemigos al ser destruida." },
            { name: "Máquina Voladora", type: "Tropa", elixir: 4, maxLevel: 14, description: "Unidad aérea que dispara a distancia a objetivos terrestres y aéreos." },
            { name: "Bebé Dragón", type: "Tropa", elixir: 4, maxLevel: 14, description: "Dragón volador que inflige daño en área a tropas y edificios." },
            { name: "P.E.K.K.A", type: "Tropa", elixir: 7, maxLevel: 14, description: "Tropa pesada con ataques devastadores, ideal contra tanques." },
            { name: "Dragón Infernal", type: "Tropa", elixir: 4, maxLevel: 14, description: "Enfoca un rayo que aumenta su daño con el tiempo a un solo objetivo." },
            { name: "Dragones Esqueleto", type: "Tropa", elixir: 4, maxLevel: 14, description: "Dos dragones voladores que atacan con daño en área." },
            { name: "Barril de Esqueletos", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Lanza un barril que libera esqueletos voladores al romperse." },
            { name: "Mago", type: "Tropa", elixir: 5, maxLevel: 14, description: "Lanza bolas de fuego que dañan en área a tropas terrestres y aéreas." },
            { name: "Espíritu de Hielo", type: "Tropa", elixir: 1, maxLevel: 14, description: "Unidad barata que congela enemigos brevemente al ser destruida." },
            { name: "Esbirros", type: "Tropa", elixir: 3, maxLevel: 14, description: "Tres unidades aéreas rápidas que atacan objetivos terrestres y aéreos." },
            { name: "Bola de Cañón", type: "Hechizo", elixir: 3, maxLevel: 14, description: "Lanza una bola que empuja y daña a tropas y edificios." },
            { name: "Taladro de Duendes", type: "Edificio", elixir: 4, maxLevel: 14, description: "Se entierra y libera duendes para atacar tropas y torres cercanas." },
            { name: "Gigante Eléctrico", type: "Tropa", elixir: 8, maxLevel: 14, description: "Tanque que aturde a enemigos cercanos con descargas eléctricas." },
            { name: "Maldición de Duendes", type: "Hechizo", elixir: 2, maxLevel: 14, description: "Invoca duendes en un área para atacar enemigos rápidamente." },
            { name: "Bárbaros", type: "Tropa", elixir: 5, maxLevel: 14, description: "Cuatro bárbaros fuertes que atacan cuerpo a cuerpo con alto daño." },
            { name: "Espejo", type: "Hechizo", elixir: 1, maxLevel: 14, description: "Duplica la última carta jugada con un nivel superior." },
            { name: "Bandida", type: "Tropa (Legendaria)", elixir: 3, maxLevel: 14, description: "Carga rápidamente hacia su objetivo, esquivando ataques." },
            { name: "Jinete de Carnero", type: "Tropa", elixir: 5, maxLevel: 14, description: "Carga contra edificios y libera dos bárbaros al ser destruida." },
            { name: "Jaula de Duendes", type: "Edificio", elixir: 4, maxLevel: 14, description: "Libera un duende forzudo que ataca con fuerza a tropas y edificios." },
            { name: "Congelamiento", type: "Hechizo", elixir: 4, maxLevel: 14, description: "Congela tropas y edificios en un área, deteniendo su movimiento y ataque." },
            { name: "Veneno", type: "Hechizo", elixir: 4, maxLevel: 14, description: "Inflige daño continuo en un área, efectivo contra enjambres." },
            { name: "Maga de la Noche", type: "Tropa (Legendaria)", elixir: 4, maxLevel: 14, description: "Invoca murciélagos y ataca con magia a distancia." },
            { name: "Torre de Bombas", type: "Edificio", elixir: 4, maxLevel: 14, description: "Lanza bombas que dañan en área a tropas terrestres." },
            { name: "Bárbaros de Élite", type: "Tropa", elixir: 6, maxLevel: 14, description: "Dos bárbaros más fuertes y rápidos que los normales." },
            { name: "Gólem de Elixir", type: "Tropa", elixir: 6, maxLevel: 14, description: "Tanque que se divide en golemitas y gotas de elixir al ser destruido." },
            { name: "Mini P.E.K.K.A", type: "Tropa", elixir: 4, maxLevel: 14, description: "Atacante rápido con alto daño, ideal contra tanques." },
            { name: "Fénix", type: "Tropa (Legendaria)", elixir: 4, maxLevel: 14, description: "Unidad aérea que renace como huevo tras ser destruida." },
            { name: "Colector de Elixir", type: "Edificio", elixir: 6, maxLevel: 14, description: "Genera elixir adicional durante la partida." },
            { name: "Máquina de Duendes", type: "Tropa", elixir: 5, maxLevel: 14, description: "Vehículo que invoca duendes y ataca con un taladro." },
            { name: "Gigante Goblin", type: "Tropa", elixir: 6, maxLevel: 14, description: "Tanque que lleva un saco y genera duendes al ser destruido." },
            { name: "Mega Caballero", type: "Tropa (Legendaria)", elixir: 7, maxLevel: 14, description: "Tropa pesada con un ataque inicial en área al saltar." },
            { name: "Tres Mosqueteras", type: "Tropa", elixir: 9, maxLevel: 14, description: "Tres mosqueteras que disparan a objetivos terrestres y aéreos." },
            { name: "Cementerio", type: "Hechizo", elixir: 5, maxLevel: 14, description: "Invoca esqueletos en un área para atacar torres o tropas." },
            { name: "Torre Infernal", type: "Edificio", elixir: 5, maxLevel: 14, description: "Dispara un rayo que aumenta su daño con el tiempo." },
            { name: "Ariete de Batalla", type: "Tropa", elixir: 4, maxLevel: 14, description: "Carga contra edificios y libera dos bárbaros al romperse." },
            { name: "Arbusto Sospechoso", type: "Tropa", elixir: 4, maxLevel: 14, description: "Se transforma en duendes al ser atacado o llegar a un edificio." },
            { name: "Príncipe Oscuro", type: "Tropa", elixir: 4, maxLevel: 14, description: "Ataca en área y tiene un escudo que absorbe daño." },
            { name: "Horda de Esbirros", type: "Tropa", elixir: 5, maxLevel: 14, description: "Seis esbirros voladores que atacan rápidamente." },
            { name: "Princesa", type: "Tropa (Legendaria)", elixir: 3, maxLevel: 14, description: "Dispara flechas de largo alcance que dañan en área." },
            { name: "Rey Esqueleto", type: "Tropa (Campeón)", elixir: 4, maxLevel: 14, description: "Invoca esqueletos con su habilidad y ataca en área." },
            { name: "Caballero Dorado", type: "Tropa (Campeón)", elixir: 4, maxLevel: 14, description: "Carga hacia enemigos con su habilidad y ataca cuerpo a cuerpo." },
            { name: "Minero Poderoso", type: "Tropa (Campeón)", elixir: 4, maxLevel: 14, description: "Se entierra y aparece en cualquier lugar para atacar torres." },
            { name: "Cohete", type: "Hechizo", elixir: 6, maxLevel: 14, description: "Inflige alto daño en un área pequeña, ideal contra torres y tropas." },
            { name: "Cañón con Ruedas", type: "Edificio", elixir: 5, maxLevel: 14, description: "Dispara a tropas terrestres y se mueve al ser destruido." },
            { name: "Choza de Duendes", type: "Edificio", elixir: 5, maxLevel: 14, description: "Genera duendes lanceros periódicamente para atacar." },
            { name: "Espíritu de Fuego", type: "Tropa", elixir: 2, maxLevel: 14, description: "Unidad kamikaze que explota, dañando en área al impactar." },
            { name: "Espíritu de Curación", type: "Tropa", elixir: 1, maxLevel: 14, description: "Cura tropas aliadas en un área al explotar." },
            { name: "Mago Eléctrico", type: "Tropa (Legendaria)", elixir: 4, maxLevel: 14, description: "Ataca con relámpagos que aturden y encadenan enemigos." },
            { name: "Leñador", type: "Tropa (Legendaria)", elixir: 4, maxLevel: 14, description: "Ataca rápidamente y deja un hechizo de furia al ser destruido." },
            { name: "Bruja Madre", type: "Tropa (Legendaria)", elixir: 4, maxLevel: 14, description: "Transforma tropas enemigas en cerdos al atacar." },
            { name: "Pescador Eléctrico", type: "Tropa", elixir: 4, maxLevel: 14, description: "Lanza un gancho que ralentiza y daña a enemigos lejanos." },
            { name: "Bruja Eléctrica", type: "Tropa (Legendaria)", elixir: 5, maxLevel: 14, description: "Invoca cerdos reales y ataca con relámpagos que aturden." },
            { name: "Pequeño Príncipe", type: "Tropa (Campeón)", elixir: 3, maxLevel: 14, description: "Dispara rápido y usa un guardia real para protegerse." },
            { name: "Chispazo", type: "Hechizo", elixir: 6, maxLevel: 14, description: "Lanza un rayo que aturde y daña a tres objetivos con mayor salud." },
            { name: "Evolución de Bruja", type: "Tropa", elixir: 5, maxLevel: 14, description: "Bruja mejorada que invoca más esqueletos y ataca con mayor daño." },
            { name: "Evolución de Esqueletos", type: "Tropa", elixir: 1, maxLevel: 14, description: "Esqueletos mejorados con mayor salud y daño explosivo al morir." },
            { name: "Evolución de Murciélagos", type: "Tropa", elixir: 2, maxLevel: 14, description: "Murciélagos mejorados que atacan más rápido y en mayor número." },
            { name: "Evolución de Arqueros", type: "Tropa", elixir: 3, maxLevel: 14, description: "Arqueros mejorados con flechas más rápidas y mayor resistencia." },
            { name: "Evolución de Bárbaros", type: "Tropa", elixir: 5, maxLevel: 14, description: "Bárbaros mejorados con mayor salud y un ataque en área." },
            { name: "Evolución de Gigante Real", type: "Tropa", elixir: 6, maxLevel: 14, description: "Gigante real mejorado con un cañón más potente y mayor salud." },
            { name: "Evolución de Mortero", type: "Edificio", elixir: 4, maxLevel: 14, description: "Mortero mejorado que dispara proyectiles con mayor daño en área." },
            { name: "Evolución de Reclutas Reales", type: "Tropa", elixir: 7, maxLevel: 14, description: "Reclutas mejorados con escudos más fuertes y mayor daño." },
            { name: "Evolución de P.E.K.K.A", type: "Tropa", elixir: 7, maxLevel: 14, description: "P.E.K.K.A mejorada con ataques más rápidos y mayor resistencia." },
            { name: "Evolución de Mega Caballero", type: "Tropa (Legendaria)", elixir: 7, maxLevel: 14, description: "Mega caballero mejorado con un salto más destructivo." },
            { name: "Evolución de Valquiria", type: "Tropa", elixir: 4, maxLevel: 14, description: "Valquiria mejorada con un giro más rápido y mayor daño en área." },
            { name: "Evolución de Chispitas", type: "Tropa", elixir: 6, maxLevel: 14, description: "Chispitas mejorada con un rayo más rápido y mayor alcance." }
        ];

        // Lista completa de nombres de cartas para verificar
        const allCardNames = [
            "Montapuercos", "Bola de Fuego", "Mosquetera", "Jefe Bandida", "Bruja", "Gigante Rúnico", "Berserker",
            "Arquera Mágica", "Goblinstein", "Esqueletos", "Flechas", "Caballero", "Espíritu Eléctrico", "Zap",
            "Ejército de Esqueletos", "Cañón", "Guardias", "Barril de Bárbaro", "Valquiria", "Pescador", "Gigante Real",
            "Bombardero", "Tornado", "Bola de Nieve Gigante", "Barril de Duendes", "Arqueros", "Lanzadardos", "Tesla",
            "Murciélagos", "Ejecutor", "Fantasma Real", "Mago de Hielo", "Tumba", "Cerdos Reales", "Monje", "Chispitas",
            "Príncipe", "Sabueso de Lava", "Ballesta", "Duendes", "Reclutas Reales", "Reina Arquera", "Gigante", "Terremoto",
            "Mortero", "Entrega Real", "Gólem de Hielo", "Máquina Voladora", "Bebé Dragón", "P.E.K.K.A", "Dragón Infernal",
            "Dragones Esqueleto", "Barril de Esqueletos", "Mago", "Espíritu de Hielo", "Esbirros", "Bola de Cañón",
            "Taladro de Duendes", "Gigante Eléctrico", "Maldición de Duendes", "Bárbaros", "Espejo", "Bandida",
            "Jinete de Carnero", "Jaula de Duendes", "Congelamiento", "Veneno", "Maga de la Noche", "Torre de Bombas",
            "Bárbaros de Élite", "Gólem de Elixir", "Mini P.E.K.K.A", "Fénix", "Colector de Elixir", "Máquina de Duendes",
            "Gigante Goblin", "Mega Caballero", "Tres Mosqueteros", "Cementerio", "Torre Infernal", "Ariete de Batalla",
            "Arbusto Sospechoso", "Príncipe Oscuro", "Horda de Esbirros", "Princesa", "Rey Esqueleto", "Caballero Dorado",
            "Minero Poderoso", "Cohete", "Cañón con Ruedas", "Choza de Duendes", "Espíritu de Fuego", "Espíritu de Curación",
            "Mago Eléctrico", "Leñador", "Bruja Madre", "Pescador Eléctrico", "Bruja Eléctrica", "Pequeño Príncipe", "Chispazo",
            "Evolución de Bruja", "Evolución de Esqueletos", "Evolución de Murciélagos", "Evolución de Arqueros",
            "Evolución de Bárbaros", "Evolución de Gigante Real", "Evolución de Mortero", "Evolución de Reclutas Reales",
            "Evolución de P.E.K.K.A", "Evolución de Mega Caballero", "Evolución de Valquiria", "Evolución de Chispitas"
        ];

        // Función para cargar todas las cartas
        function loadCards() {
            const grid = document.getElementById('cards-grid');
            // Limpiar la cuadrícula
            grid.innerHTML = '';
            // Añadir todas las cartas
            cardsData.forEach(card => {
                const cardElement = document.createElement('div');
                cardElement.classList.add('card');
                cardElement.innerHTML = `
                    <h3>${card.name.toUpperCase()}</h3>
                    <p><strong>Tipo:</strong> ${card.type}</p>
                    <p><strong>Costo de Elixir:</strong> ${card.elixir}</p>
                    <p><strong>Nivel Máximo:</strong> ${card.maxLevel}</p>
                    <p><strong>Descripción:</strong> ${card.description}</p>
                `;
                grid.appendChild(cardElement);
            });
        }

        // Función para asignar tipo de carta
        function getCardType(name) {
            const troops = ["Montapuercos", "Mosquetera", "Jefe Bandida", "Bruja", "Gigante Rúnico", "Berserker", "Arquera Mágica", "Goblinstein", "Esqueletos", "Caballero", "Espíritu Eléctrico", "Ejército de Esqueletos", "Guardias", "Valquiria", "Pescador", "Gigante Real", "Bombardero", "Arqueros", "Lanzadardos", "Murciélagos", "Ejecutor", "Fantasma Real", "Mago de Hielo", "Cerdos Reales", "Monje", "Chispitas", "Príncipe", "Sabueso de Lava", "Duendes", "Reclutas Reales", "Reina Arquera", "Gigante", "Gólem de Hielo", "Máquina Voladora", "Bebé Dragón", "P.E.K.K.A", "Dragón Infernal", "Dragones Esqueleto", "Barril de Esqueletos", "Mago", "Espíritu de Hielo", "Esbirros", "Bárbaros", "Bandida", "Jinete de Carnero", "Maga de la Noche", "Bárbaros de Élite", "Mini P.E.K.K.A", "Fénix", "Máquina de Duendes", "Gigante Goblin", "Mega Caballero", "Tres Mosqueteros", "Príncipe Oscuro", "Horda de Esbirros", "Princesa", "Rey Esqueleto", "Caballero Dorado", "Minero Poderoso", "Mago Eléctrico", "Leñador", "Bruja Madre", "Pescador Eléctrico", "Bruja Eléctrica", "Pequeño Príncipe"];
            const spells = ["Bola de Fuego", "Flechas", "Zap", "Tornado", "Bola de Nieve Gigante", "Barril de Duendes", "Terremoto", "Entrega Real", "Congelamiento", "Veneno", "Cohete", "Cementerio", "Maldición de Duendes", "Espíritu de Curación", "Chispazo"];
            const buildings = ["Cañón", "Tesla", "Tumba", "Ballesta", "Mortero", "Choza de Duendes", "Torre de Bombas", "Colector de Elixir", "Torre Infernal", "Ariete de Batalla", "Cañón con Ruedas", "Jaula de Duendes"];
            if (troops.includes(name) || name.startsWith("Evolución de")) {
                if (name.includes("Jefe Bandida") || name.includes("Goblinstein") || name.includes("Monje") || name.includes("Reina Arquera") || name.includes("Rey Esqueleto") || name.includes("Caballero Dorado") || name.includes("Minero Poderoso") || name.includes("Pequeño Príncipe")) return "Tropa (Campeón)";
                if (name.includes("Arquera Mágica") || name.includes("Fantasma Real") || name.includes("Mago de Hielo") || name.includes("Bandida") || name.includes("Maga de la Noche") || name.includes("Princesa") || name.includes("Mago Eléctrico") || name.includes("Leñador") || name.includes("Bruja Madre") || name.includes("Bruja Eléctrica") || name.includes("Mega Caballero") || name.includes("Fénix")) return "Tropa (Legendaria)";
                return "Tropa";
            }
            if (spells.includes(name)) return "Hechizo";
            if (buildings.includes(name)) return "Edificio";
            return "Tropa"; // Valor por defecto
        }

        // Cargar todas las cartas al iniciar
        loadCards();

        // Animación suave al hacer scroll a las secciones
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href').substring(1);
                const targetElement = document.getElementById(targetId);
                targetElement.scrollIntoView({ behavior: 'smooth' });
            });
        });
    </script>
</body>
</html># clash
