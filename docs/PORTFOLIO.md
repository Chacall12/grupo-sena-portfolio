# Portfólio e produtos

Este documento detalha como as frentes do Grupo SENA se relacionam. A classificação de maturidade deve ser lida em conjunto com o [Status do produto](STATUS.md).

## Ecossistema

```text
                         GRUPO SENA
                              │
                  Gestão + tecnologia aplicada
                              │
                           SENA OS
                  núcleo operacional multiempresa
                  ┌───────────┼───────────┐
                  │           │           │
             SENA Legal  SENA Serviços  SENA AI
                  │           │           │
             jurídico      campo/OS    Autopilot
                  └───────────┼───────────┘
                              │
                 SENA Mobile e produtos conectados
```

## 1. SENA OS

### O que é

Plataforma de inteligência operacional que reúne os registros essenciais de uma empresa e organiza o trabalho entre atendimento, comercial, administrativo, execução e gestão.

### Problemas que resolve

- informação presa em conversas, planilhas e pessoas;
- duplicidade de cadastro e perda de contexto do cliente;
- oportunidade vendida que não vira execução rastreável;
- atividade executada sem evidência ou sem comunicação ao financeiro;
- documentos espalhados e agendas desconectadas;
- gestor sem visão de prioridade, gargalo ou responsabilidade.

### Núcleo funcional

#### Atendimento

- conversas e mensagens;
- mídia, contatos compartilhados e referências clicáveis;
- atribuição de responsável;
- criação de registros relacionados a partir da conversa;
- suporte a grupos quando o transporte permite;
- controle da janela operacional do WhatsApp.

#### Comercial

- leads e oportunidades;
- pipeline configurável;
- responsáveis, valores e estágios;
- vínculo entre conversa, cliente e oportunidade;
- orçamento com itens, total e aprovação.

#### Operação

- agenda e compromissos;
- tarefas, prioridades, vencimentos e responsáveis;
- ordem de serviço vinculada à origem;
- atualização de status de execução;
- Service Blueprints para padronizar entrega e onboarding.

#### Relacionamento

- ficha do cliente;
- histórico relacionado;
- dados cadastrais e contatos;
- documentos e arquivos;
- visão integrada de agenda, tarefa e serviço.

#### Gestão

- dashboard operacional;
- base de indicadores financeiros;
- equipe, departamentos e permissões;
- identidade visual por organização;
- notificações, auditoria e administração.

## 2. SENA Legal

### Posicionamento

Vertical operacional para escritórios e equipes jurídicas. O objetivo é controlar o fluxo entre processo, publicação, advogado, tarefa, agenda e histórico — não substituir os sistemas oficiais de peticionamento.

### Capacidades do piloto

- processos por organização;
- clientes, tribunal, classe, assunto, status e movimentações;
- múltiplos advogados por processo;
- equipe jurídica e advogado principal;
- OABs monitoradas por UF;
- ingestão incremental de publicações do DJEN;
- consulta auxiliar de processos públicos pelo DataJud;
- deduplicação por identificador/hash externo;
- checkpoints, retry e fila de sincronização;
- status de sincronização amigável à interface móvel;
- publicação vinculada a processo e advogado quando possível;
- fila de itens sem vínculo para tratamento humano;
- criação de tarefa e registro de providência;
- trilha de auditoria sem duplicar conteúdo sensível em logs.

### Controles jurídicos e de segurança

- ausência de dado público não é tratada como inexistência;
- processos sigilosos permanecem em modo manual;
- datas ausentes não são inventadas;
- prazo não é calculado automaticamente no piloto;
- worker externo respeita limites, `Retry-After` e processamento econômico;
- credenciais pessoais de sistemas judiciais não fazem parte da solução atual.

## 3. SENA Serviços

### Posicionamento

Vertical para empresas que vendem e executam serviços. Reutiliza o núcleo do SENA OS e adiciona uma jornada operacional própria.

### Jornada principal

```text
Conversa
  → Cliente
  → Oportunidade
  → Orçamento
  → Aprovação
  → Agendamento
  → Ordem de serviço
  → Execução e evidências
  → Conclusão
  → Cobrança
  → Recorrência
```

### Base atual

- orçamento vinculado ao cliente e ao atendimento;
- itens, quantidade, preço unitário e total;
- aprovação e geração de ordem de serviço;
- OS originada por conversa, tarefa, agenda ou orçamento;
- acompanhamento por status;
- vínculos que preservam a origem da demanda.

### Expansões planejadas

- checklists por tipo de serviço;
- fotos, áudio, assinatura e evidências de campo;
- materiais utilizados e relatório de conclusão;
- disparo da próxima etapa financeira;
- ativos/equipamentos por cliente;
- manutenção preventiva e recorrência;
- roteirização e capacidade de equipes;
- experiência móvel dedicada.

## 4. SENA AI

### Experiência inicial

A interface existente representa a camada de inteligência contextual do produto: briefing, perguntas operacionais, identificação de pendências e prioridades sugeridas. A conexão com dados reais e modelos de produção deve ocorrer gradualmente.

### Copiloto supervisionado

O primeiro agente útil deve receber ferramentas pequenas e explícitas, por exemplo:

```text
consultar_cliente
consultar_profissionais
consultar_disponibilidade
consultar_contexto_da_conversa
criar_pre_agendamento
```

O agente interpreta, consulta e propõe. A pessoa confirma a resposta e a ação.

### SENA Autopilot

Autonomia é uma capacidade posterior, liberada por tipo de ação. Cada política deve definir:

- quem pode habilitar;
- para quais organizações e módulos;
- dados e ferramentas permitidos;
- número máximo de passos;
- orçamento e consumo;
- quando exigir confirmação;
- quando interromper e escalar;
- como auditar e reverter.

## 5. SENA Mobile

Experiência PWA planejada para profissionais em campo. Compartilha autenticação, dados e permissões com o desktop, mas possui interface própria, orientada a execução.

Casos prioritários:

- “Meu dia” e próximas atividades;
- abrir cliente, endereço e instruções da OS;
- iniciar, pausar e concluir serviço;
- checklist e observações;
- câmera, anexos e evidências;
- assinatura ou aceite quando aplicável;
- baixa de tarefa e criação automática da próxima etapa;
- uso jurídico em diligências, audiências e oitivas.

## 6. Produtos conectados

### SENA Service Tag

Etiqueta QR ou NFC associada a um ativo ou serviço. Pode permitir que cliente e equipe consultem informações autorizadas, histórico de manutenção, garantia, contato do prestador e novo chamado.

### SENA TAP

Família conceitual de pontos físicos de entrada — avaliações, contato, captura de lead, recorrência ou solicitação de serviço — conectados ao SENA OS.

Esses itens estão em fase conceitual e dependem de validação de mercado, privacidade, experiência pública e modelo comercial.

## Serviços profissionais

O software pode ser acompanhado por:

- diagnóstico operacional;
- desenho de processo e responsabilidades;
- configuração e implantação;
- Service Blueprints;
- integração assistida;
- migração de dados compatíveis;
- treinamento por perfil;
- suporte e melhoria contínua;
- acompanhamento de indicadores de adoção e resultado.

Escopo, SLA, limites e preço são definidos por proposta.
