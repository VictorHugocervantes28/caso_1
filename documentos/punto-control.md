# Punto de control — Caso 1 Luciérnaga

## Datos del libro de cálculo
- Punto 2: medias observadas A=20 s, B=28 s, C=40 s, D=24 s, E=18 s. Valoraciones: A=1, B=1.1, C=1, D=0.95, E=1. Tiempo normal: A=20, B=30.8, C=40, D=22.8, E=18 s. Suplemento 1.15.
- Punto 3: partición 1: A+B+C = 23+32.2+46 = 101.2 s; D+ensayo+E = 26.22+30+20.7 = 76.92 s. Capacidad para 420 min: floor(25200/101.2)=249 unidades.
- Punto 3: partición 2, suma de las celdas = 32.2+46+26.22+30+20.7 = 155.12 s. El archivo registra 156.5 s; debe contrastarse con el anexo patrón.
- Punto 5: ciclos de referencia=90.8 s, A=82.8 s, B=72 s. Capacidades con 420 min: 277, 304 y 350 unidades/día respectivamente (redondeo hacia abajo).
- Punto 5: inversión A=€180 y B=€950; amortización indicada a 20 turnos: €9 y €47.50 por turno.

## Cálculos de Parte 2 (semanas 8–11)
Alturas de codo: 90, 94, 98, 102, 106, 110 cm. Superficie entre 5 y 10 cm bajo codo. Intersección de rangos individuales: máximo de límites inferiores = 100 cm; mínimo de límites superiores = 80 cm. No existe una altura fija que satisfaga simultáneamente a las seis personas. Una mesa ajustable con recorrido total de 80–105 cm cubre los intervalos individuales (90→80–85; 94→84–89; 98→88–93; 102→92–97; 106→96–101; 110→100–105). Alcance cómodo mínimo observado =34 cm; colocar contenedor frecuente dentro de 34 cm, medidos desde el borde de referencia definido en el diseño. No llamar percentiles a extremos de muestra.
Muestreo: manual 91/120=75.83%; espera ensayo 10/120=8.33%; falta material 11/120=9.17%; ajuste 8/120=6.67%; no manual=(10+11+8)/120=24.17%.
Tamaño orientativo: n=(1.96²×0.25×0.75)/(0.08²)=112.55; redondear hacia arriba: 113. No demuestra independencia de observaciones ni autoriza por sí solo un suplemento adicional.

## Supuestos de la aplicación
- Ciclos por alternativa del Punto 5: referencia 90.8 s, A 82.8 s, B 72 s.
- Piloto B: para permitir entrada del tiempo normal C, la aplicación usa TC_B=72+(C_ingresado−30) s. Es una hipótesis de modelado, no una fórmula explícita del Excel; validar con anexo patrón.
- Ventana predeterminada 420 min porque el libro calcula con 25,200 s.
- Inventario límite 350 unidades.
- Productividad: unidades realizables por hora de ventana neta. No se interpreta como productividad laboral individual.
- Coste equivalente por turno: A €9, B €47.50, referencia €0 incremental.
- El cálculo es de régimen, no simulación.

## Discrepancias a resolver antes del código definitivo
1. Punto 3 registra 156.5 s para la partición 2, pero las cargas detalladas suman 155.12 s.
2. El tiempo normal C del Punto 2 es 40 s; el piloto B tiene entrada predeterminada de 30 s. La app mantiene ambos conceptos separados.
3. Los ciclos de Punto 5 no incluyen una descomposición completa por estación para las alternativas. La app no inventa esa distribución: presenta cargas de la partición inicial y el ciclo agregado de la alternativa seleccionada.
4. La altura de mesa fija de 90 cm no cubre a las seis personas si el criterio es una superficie entre 5 y 10 cm bajo el codo. El recorrido ajustable propuesto es 80–105 cm.
