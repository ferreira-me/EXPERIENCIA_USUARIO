# Folha de Apoio – Construção de Fluxo de Usuário (Preenchida)

**Persona escolhida:** Ana, 28 anos, moradora de área de risco  
**Objetivo da Persona:** Receber um alerta confiável de enchente em tempo hábil

## Etapas do Fluxo

| Etapa  | Ação do Usuário                               | Sistema/Aplicativo responde                     | Sentimento esperado                       |
|-------:|-----------------------------------------------|-------------------------------------------------|-------------------------------------------|
| Início | Ana abre o app ao ver nuvens escuras          | Tela inicial carregada                          | Ansiosa, busca segurança                  |
| 1      | Ativa a localização no app                    | App solicita permissão de GPS                   | Confiante                                 |
| 2      | Recebe notificação de alerta de enchente      | Push notification clara e objetiva              | Preocupada, porém informada               |
| 3      | Lê os detalhes do alerta                      | Mapa da região e instruções oficiais do INPE    | Tranquilidade (tem instruções confiáveis) |
| Fim    | Compartilha o alerta com vizinhos             | Botão rápido (WhatsApp, SMS)                    | Engajada e solidária                      |

## Decisões (se houver)

| Decisão           | Condição                  | Caminho A (Sim)                     | Caminho B (Não)                         |
|-------------------|---------------------------|-------------------------------------|-----------------------------------------|
| Permissão de GPS  | Usuário aceita ou recusa  | Aceita → localização automática     | Recusa → selecionar cidade manualmente  |

## Oportunidades de Melhoria

| Etapa/Decisão                | Possível ponto de dor                 | Oportunidade de melhoria                 |
|-----------------------------|---------------------------------------|------------------------------------------|
| Etapa 2 – Notificação       | Mensagem muito longa                  | Usar ícones + texto curto                |
| Etapa 3 – Detalhes do alerta| Dúvida quanto à confiabilidade        | Mostrar logo e fonte oficial do INPE     |
| Decisão – GPS recusado      | Seleção manual pode ser cansativa     | Sugerir salvar cidade favorita           |

> Observação: esta folha serve de base para os fluxos em `flows/`.
