# SIRIUSA-B

O Sirius A&B é um Progressive Web App (PWA) multiplataforma de apoio ao cuidado domiciliar (Home Care), autogestão de saúde e segurança ativa, desenvolvido no Instituto Benjamin Constant (IBC) como projeto da disciplina de Prática Profissional Supervisionada I, no Curso Técnico de Nível Médio em Inteligência Artificial.

A aplicação funciona tanto pelo navegador quanto instalada diretamente na tela inicial de smartphones (Android/iOS) e computadores, oferecendo suporte offline e isolamento total de dados por conta autenticada.

Públicos-Alvo e Perfis de Uso

O sistema opera com perfis dedicados (Paciente Independente e Cuidador) e bancos de dados separados por e-mail para atender três cenários principais:

Monitoramento de Idosos (Perfil Cuidador): Controle rigoroso de horários de medicação, alertas sonoros e nativos na hora da dose, acompanhamento de pressão arterial/glicemia e agenda de consultas.

Suporte para Mães Atípicas (Perfil Cuidador): Diário de cuidados com reconhecimento de voz real (Web Speech API) para registrar rotinas terapêuticas e sintomas com agilidade, gerando resumos clínicos automáticos exportáveis em .txt para consultas médicas.

Pessoas que Moram Sós (Perfil Paciente Independente): Autogestão de saúde integrada ao módulo de Segurança Ativa, com verificações periódicas programáveis e acionamento automático de contatos de emergência caso não haja resposta.

Funcionalidades Implementadas

Scanner Inteligente de Receitas e Caixas (OCR Real): Utiliza Tesseract.js v5 com pré-processamento de contraste em <canvas> para ler fotos de embalagens ou receitas médicas, identificando automaticamente múltiplos medicamentos, dosagens (mg, ml, mcg, gotas) e horários sugeridos.

Análise de Interações Medicamentosas e Contraindicações: Cruza os fármacos cadastrados na rotina e alerta sobre combinações de risco (Grave ou Moderado), explicando o mecanismo de risco e as contraindicações preventivas.

Notificações e Alertas de Medicamentos: Dispara aviso sonoro e notificação nativa no celular ou computador no horário programado de cada dose não confirmada.

Monitoramento de Sinais Vitais e Padrões de Saúde: Registro de Pressão Arterial, Frequência Cardíaca (bpm), Glicemia (mg/dL) e Escala Visual de Humor, com gráficos evolutivos (Chart.js) e relatórios estatísticos de médias e variações por período.

Diário de Cuidados com Ditado por Voz e Exportação .txt: Transcrição de voz nativa em português (pt-BR), geração automática de relatórios clínicos consolidados e exportação direta em arquivo .txt.

Segurança Ativa (Verificação Periódica e Emergência):

Agendador contínuo em tempo real com horários configuráveis (Manhã e Noite).

Emissão de alarme sonoro sintetizado (Web Audio API) e contagem regressiva na tela: se o usuário não clicar em "ESTOU BEM" dentro do tempo limite, o protocolo aciona os contatos de emergência cadastrados e o SAMU (192).

Chatbot de Suporte Integrado: Assistente virtual embarcado na interface para orientar o usuário sobre todas as funcionalidades do aplicativo.

Autenticação com Senha Fixa e Privacidade (LGPD): Cadastro, login validado, recuperação de senha e particionamento local por e-mail (localStorage).

Aplicativo Instalável (PWA): Manifesto Web e Service Worker embutidos no código para instalação em tela cheia e funcionamento offline.

Tecnologias Utilizadas

Interface & Responsividade: HTML5, Tailwind CSS, Font Awesome 6

Lógica & Persistência: JavaScript (ES6+), Web Storage API (localStorage)

Visão Computacional (OCR): Tesseract.js v5 + HTML5 Canvas (pré-processamento de contraste)

Visualização de Dados: Chart.js

APIs Nativas do Navegador: Web Speech API (voz), Web Audio API (alarme sonoro), Notifications API e Service Workers (PWA)

Como Acessar ou Instalar

Acesso Online (GitHub Pages):

Abra o link oficial no navegador (Google Chrome, Edge ou Safari):

https://anaquadros2005-alt.github.io/SIRIUSAB/

Instalar como Aplicativo (Celular ou PC):

Toque no botão "Instalar App" na tela inicial (ou abra o menu do navegador -> "Instalar aplicativo" / "Adicionar à Tela de Início").

Execução Local:

Baixe o repositório e abra o arquivo index.html diretamente no navegador.

Equipe de Desenvolvimento e Divisão Técnica

Ana Paula Quadros Desidério: Arquitetura geral, PWA instalável, autenticação e banco de dados particionado por e-mail, sinais vitais, diário por voz, relatórios exportáveis e chatbot.

Beatriz de Sousa Falcão: Pipeline de imagens, Scanner OCR múltiplo de receitas/embalagens (Tesseract.js) e motor de análise de interações e contraindicações medicamentosas.

Ítalo Augusto Costa dos Santos: Módulo de Segurança Ativa, agendador em tempo real, notificações de medicação, alarme sonoro (Web Audio API) e protocolo de emergência.

Informações Acadêmicas

Instituição: Instituto Benjamin Constant – IBC

Curso: Curso Técnico de Nível Médio em Inteligência Artificial

Disciplina: Prática Profissional Supervisionada I (2026)

