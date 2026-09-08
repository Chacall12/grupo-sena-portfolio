# Roadmap

O roadmap é orientado por resultados e critérios de passagem. A ordem pode mudar conforme pilotos, dependências externas, segurança, capacidade da equipe e retorno comercial. Não há datas públicas comprometidas.

## Direção

```text
Confiabilidade do núcleo
        → operação real
        → integrações profundas
        → execução móvel
        → IA supervisionada
        → autonomia progressiva
        → novos produtos e verticais
```

## Etapa 1 — Consolidar o SENA Core

### Objetivo

Fazer a jornada compartilhada funcionar de ponta a ponta com dados reais e sem dependência de massa demonstrativa.

### Entregas

- atendimento, cliente, pipeline, agenda e tarefas integrados;
- orçamento e OS preservando a origem do registro;
- equipe, convites, papéis e departamentos estáveis;
- Service Blueprints reutilizáveis;
- financeiro alimentado apenas por fontes confiáveis;
- métricas, logs, recuperação e suporte operacional.

### Critério de passagem

Uma organização piloto consegue executar sua rotina principal, localizar o histórico do cliente e identificar responsável/próxima ação sem controles paralelos essenciais.

## Etapa 2 — Validar as verticais

### SENA Legal

- testar processos e publicações com conjunto real controlado;
- comparar cobertura do DJEN com a rotina atual;
- tratar publicações sem vínculo e cancelamentos;
- validar fila, checkpoint, retry e estados de sincronização;
- medir tempo de tratamento e falhas cadastrais detectadas;
- manter prazo e sigilo sob revisão humana.

### SENA Serviços

- validar conversa → orçamento → aprovação → agenda → OS;
- registrar execução, conclusão e próxima etapa;
- medir tempo entre conclusão e faturamento;
- incluir checklists e evidências por Service Blueprint.

### Critério de passagem

Cada vertical demonstra resultado em operação real e possui limites comunicáveis em proposta comercial.

## Etapa 3 — Aprofundar integrações

- completar ativação da WhatsApp Cloud API oficial;
- estabilizar webhooks, mídia, templates e estados de entrega;
- decidir o papel comercial da alternativa Standard considerando seu risco;
- transformar conectores Google em fluxos úteis de Drive, Agenda, Gmail e documentos;
- evoluir Asaas de sandbox para fluxo financeiro homologado;
- revisar consentimento, revogação, escopos e exclusão de cada integração;
- documentar SLAs e contingências de terceiros.

## Etapa 4 — SENA Mobile

- PWA instalável com rota e layout próprios;
- “Meu dia”, tarefas, agenda e OS atribuídas;
- câmera, anexos, observações e evidências;
- iniciar, pausar e concluir atividade;
- checklist por serviço;
- sincronização com o mesmo backend e permissões do desktop;
- tratamento progressivo de conectividade limitada.

### Critério de passagem

Um profissional de campo conclui uma atividade real pelo celular e o administrativo recebe status e evidências sem redigitação.

## Etapa 5 — Agente de IA supervisionado

### Infraestrutura

- gateway/agente isolado em ambiente server-side;
- provedor de modelo substituível;
- ferramentas explícitas para cliente, profissionais, agenda e conversa;
- consumo e custo registrados por organização;
- orçamento mensal e limites por execução;
- avaliação, replay seguro e conjunto de testes.

### Primeiro caso de uso

```text
Mensagem de agendamento
   → classificar intenção
   → consultar cliente e profissionais
   → consultar horários
   → sugerir resposta
   → operador confirma
   → criar pré-agendamento
   → cliente confirma
   → registrar evento
```

### Critério de passagem

O agente responde corretamente a um conjunto representativo, usa apenas ferramentas autorizadas, respeita orçamento e nunca executa ação sensível sem a política correspondente.

## Etapa 6 — SENA Autopilot

- liberar autonomia por ação, não por módulo inteiro;
- começar com ações reversíveis e de baixo impacto;
- implementar níveis de confiança e confirmação;
- criar kill switch por organização;
- medir aceitação, correção, reversão e escalonamento;
- expandir para reagendamento, cobrança, documentos e OS somente após validação.

## Etapa 7 — Ativos e produtos conectados

- cadastro de ativos/equipamentos;
- histórico de manutenção e garantias;
- SENA Service Tag por QR/NFC;
- novo chamado e recorrência vinculados ao ativo;
- SENA TAP para avaliação e relacionamento;
- estudos de novas verticais e canais.

## Ideias posteriores, sujeitas a validação

- SENA Bridge para sincronização assistida em ambientes autenticados, quando juridicamente e tecnicamente apropriado;
- roteirização e otimização de capacidade;
- manutenção preventiva baseada em histórico;
- portal externo do cliente;
- marketplace de Service Blueprints;
- analytics comparativo com anonimização e base legal adequadas.

## Itens que não devem ser antecipados

- autonomia ampla antes de ferramentas e políticas estreitas;
- prazo jurídico sem calendário e confirmação profissional;
- armazenamento de certificado digital ou credencial judicial pessoal;
- uso comercial de fonte pública sem validar termos e base jurídica;
- dependência financeira de dados estimados;
- venda de integração externa antes da homologação;
- aplicativo nativo quando a PWA ainda atende o caso prioritário.
