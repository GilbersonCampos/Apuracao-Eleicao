# Apuração Eleição 2026 🇧🇷

Este é um painel (dashboard) web minimalista, moderno e responsivo desenvolvido para acompanhar a apuração das eleições de 2026 em tempo real. Ele consome diretamente os arquivos JSON oficiais divulgados pela infraestrutura do Tribunal Superior Eleitoral (TSE).

## Funcionalidades
- **Único Arquivo (`index.html`)**: Todo o HTML, CSS e JavaScript estão contidos em um só lugar.
- **Tema Escuro (Dark Mode)**: Design elegante, inspirado em dashboards modernos corporativos.
- **Divisão de Contextos**:
  - **Área Principal**: Acompanha a eleição Presidencial (Nacional ou por Estado).
  - **Área Estadual (Secundária)**: Permite selecionar um estado para visualizar um resumo rápido (Top 3) de Governador, Senador e Deputados daquela UF, sem perder a visão nacional.
- **Atualização Automática**: Atualiza silenciosamente os dados em segundo plano a cada 10 segundos, com animações suaves nas barras de progresso e valores.

## Como Executar

Como a aplicação faz requisições (Fetch API) para servidores externos, executá-la diretamente com dois cliques no arquivo `index.html` (`file:///...`) pode esbarrar em políticas de segurança dos navegadores (CORS). A forma recomendada é subir um pequeno servidor HTTP local.

### Opção 1: Usando Python (Recomendado)
A maioria dos computadores (especialmente Mac/Linux) já possui o Python instalado.
1. Abra o Terminal ou Prompt de Comando.
2. Navegue até a pasta onde este projeto está salvo.
3. Execute o comando:
   ```bash
   python -m http.server 8000