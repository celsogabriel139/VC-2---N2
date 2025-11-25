🐭🏁 Simulação de Detecção & Perseguição 2D
“Ligeirinho vs. Frajola”

Este projeto implementa uma simulação interativa 2D que combina:

detecção de movimento por frame differencing;

estratégias inteligentes de perseguição;

visualização em tempo real;

métricas de desempenho e exportação de resultados.

O objetivo é modelar e analisar comportamentos de perseguição reativos, com diferentes velocidades, algoritmos e níveis de detecção.

📌 Funcionalidades Principais
🎯 Agente-Alvo (“Ligeirinho”)

Surge em uma borda aleatória da tela.

Move-se em trajetória linear com velocidade configurável.

Pode escapar se sair do cenário antes de ser capturado.

🐱 Agente-Perseguidor (“Frajola”)

Começa no centro da tela.

Utiliza diferentes estratégias de perseguição:

Pursuit Direto – segue o ponto detectado.

Previsão Linear (Lead) – prevê posição futura usando velocidade estimada.

Interceptação Analítica – calcula tempo de colisão estimado e intercepta.

👁️ Detecção de Movimento

Implementada via diferença entre frames consecutivos.

Pixels com alteração acima do threshold geram uma máscara de movimento.

A partir dela, o sistema calcula um centróide de detecção.

Suporta atraso de percepção (“reaction delay”).

📊 Métricas e Batch Mode

Registra automaticamente:

sucesso ou falha da perseguição;

frames até captura;

estratégia usada;

velocidades de cada agente.

Permite rodar 50 cenários automáticos.

Exporta tudo em CSV.

