# QuizBiblico
Placar eletrônico interativo e sistema de Quiz Bíblico em tempo real com suporte a botões físicos sem fio via ESP32 (ESP-NOW), tela dupla (Organizador + Plateia/Projetor), cronômetro regressivo, efeitos sonoros nativos e importação de perguntas por categoria/livro via JSON ou Excel.

https://anderson8153.github.io/bible-challenge-quiz/

🏆 Bible Challenge: Placar Eletrônico & Sistema de Quiz (ESP32 + Web App)

Sistema completo de placar eletrônico e gerenciamento de perguntas desenvolvido para competições de Quiz Bíblico ao vivo. O projeto integra um Web App moderno (HTML/Tailwind/JS) com hardware ESP32 via protocolo sem fio ESP-NOW, oferecendo baixa latência (< 5ms) e exibição simultânea em duas telas.

✨ Principais Funcionalidades

📺 Sistema Dual-Screen (Tela Dupla):

Painel do Organizador: Controle de pontuação, cronômetro, sorteio de perguntas, visualização de gabarito oficial e log de eventos.

Tela da Plateia (Projetor/TV): Interface limpa e responsiva em tela cheia que exibe o placar, cronômetro circular, perguntas e destaque visual instantâneo de quem apertou o botão primeiro.

⚡ Integração Sem Fio com ESP32 (ESP-NOW & Web Serial API):

Comunicação direta via porta USB do navegador (sem necessidade de servidores externos ou internet no momento do evento).

Arquitetura com 2 ESP32s (Transmissor no palco com botões físicos NF e Receptor conectado ao computador).

Detecção automática de desconexão do dispositivo USB.

📖 Banco de Perguntas Inteligente:

Importação de arquivos .json e planilhas Excel (.xlsx, .xls, .csv).

Filtro hierárquico por Categoria / Testamento e Subcategoria / Livro.

Sorteio Aleatório Sem Repetição com histórico persistente e opção de reinício.

🔊 Áudio & Atalhos:

Efeitos sonoros sintetizados nativamente via Web Audio API (buzzer, acerto, erro, contagem regressiva e tempo esgotado).

Atalhos de teclado para operação rápida (A para Jogador 1, L para Jogador 2, Espaço para pausar/retomar o tempo).

🛠️ Tecnologias Utilizadas

Frontend: HTML5, Tailwind CSS, JavaScript (ES6+), BroadcastChannel API, Web Serial API, Web Audio API.

Leitura de Planilhas: SheetJS (xlsx).

Hardware / Firmware: C++ (Arduino IDE), ESP32, Protocolo ESP-NOW.

🚀 Como Usar

Acesse a aplicação pelo navegador (Google Chrome ou Microsoft Edge) via HTTPS ou localhost.

Conecte o ESP32 Receptor na porta USB do computador e clique em "Dispositivo Off • Conectar" no topo da tela.

Clique em "Abrir Tela da Plateia" e arraste a janela gerada para o segundo monitor ou projetor (pressione F11 ou dê um duplo clique para tela cheia).

Abra as Configurações (⚙️) para importar sua lista de perguntas (.json ou .xlsx), selecionar o tema/livro e ajustar o tempo da rodada.

📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.
