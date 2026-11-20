Hoja de Ruta 2027 · Plan de Comunicación (División Proceso RRHH)

Aplicação web interativa para gestão e acompanhamento visual do Plano de Comunicação 2027 da División Proceso RRHH, construída em HTML5 + Konva.js + Tailwind CSS e ligada em tempo real ao Supabase (PostgreSQL).

Funcionalidades Principais

Cronograma Interativo (Konva.js): Visualização anual de janeiro a dezembro (S1 a S52 ISO) com barras por bloco temático e marcadores das semanas agendadas.

Gestão por Grupos Destinatários: Ativação seletiva dos grupos MD, MD + JJ, Propietarios e CdM dentro do intervalo de cada linha, com preenchimento automático segundo as regras de periodicidade ou marcação manual semana a semana.

Controlo de Execução: Marcação de semanas como já comunicadas (clique direito sobre a semana no modal) e sincronização em tempo real com a base de dados.

Gestão Dinâmica de Blocos e Linhas: Criação de novos blocos temáticos com cor personalizada, adição, edição de intervalos (S_inicio–S_fin) e eliminação de linhas diretamente na interface.

Radar Semanal: Consulta consolidada de todas as comunicações previstas e respetivas mensagens-chave para qualquer semana ISO do ano.

Arquitetura & Stack

Frontend: Ficheiro único estático (index.html), sem necessidade de servidor backend próprio.

Renderização Gráfica: Konva.js v9 com camadas separadas (grid, hover e bars) para navegação fluida a 60 FPS.

Estilos: Tailwind CSS (CDN) + Font Awesome.

Base de Dados & Realtime: Supabase (@supabase/supabase-js v2).