# Status do produto

Atualizado em **8 de setembro de 2026**.

## Como interpretar

| Classificação | Significado |
|---|---|
| **Disponível** | Existe implementação no produto atual; pode ainda receber melhorias |
| **Piloto / validação** | Há implementação utilizável, mas depende de teste real, configuração ou validação operacional |
| **Base técnica** | Estrutura, telas ou conectores existem, mas o fluxo de negócio ainda não está completo |
| **Planejado** | Faz parte da direção de produto, sem compromisso público de data |
| **Conceito** | Hipótese de produto ou mercado ainda sujeita a descoberta e validação |

## Matriz resumida

| Domínio | Capacidade | Status | Observação |
|---|---|---|---|
| Plataforma | Multiempresa, organizações e módulos | Disponível | Isolamento por organização e autorização por módulo |
| Plataforma | Autenticação, convites e solicitação de acesso | Disponível | Fluxos distintos para sócios, administradores e colaboradores |
| Plataforma | RBAC e departamentos | Disponível | Proteção de menus, rotas, RPCs e políticas de dados |
| Plataforma | Branding por organização | Disponível | Logo e identidade visual configuráveis |
| Gestão | Dashboard operacional | Disponível | Indicadores e pendências integrados aos módulos |
| Gestão | Dashboard financeiro | Base técnica | Deve consumir somente fontes financeiras reais |
| CRM | Pipeline, leads e oportunidades | Disponível | Estágios, responsáveis e valores |
| Atendimento | Central de conversas | Disponível | Mensagens, mídia, grupos, atribuição e ações relacionadas |
| Clientes | Cadastro e ficha integrada | Disponível | Base comum entre verticais |
| Operação | Agenda e tarefas | Disponível | Responsáveis, prazos e vínculos operacionais |
| Serviços | Orçamentos | Disponível | Itens, valores, aprovação e vínculo de origem |
| Serviços | Ordens de serviço | Disponível | Origem rastreável e atualização de status |
| Serviços | Execução de campo completa | Planejado | Checklist, evidências, assinatura e conclusão móvel |
| Configuração | Service Blueprints | Disponível | Modelos de qualificação, documentos e etapas |
| Jurídico | Processos e equipe jurídica | Piloto / validação | Vínculos transacionais e controles multiempresa |
| Jurídico | Publicações DJEN e OAB | Piloto / validação | Ingestão incremental e tratamento operacional |
| Jurídico | DataJud | Piloto / validação | Fonte auxiliar para dados públicos |
| Jurídico | Prazo automático | Não disponível | Revisão humana é deliberadamente obrigatória |
| Google | Drive | Piloto / validação | Pastas e arquivos por organização |
| Google | Agenda | Piloto / validação | Eventos e sincronização |
| Google | Gmail, Docs, Planilhas, Forms, Meet e Keep | Base técnica | Conectores por ferramenta; profundidade varia por fluxo |
| Mensageria | WhatsApp Cloud API | Piloto / validação | Depende de configuração e aprovação comercial da Meta |
| Mensageria | WhatsApp Standard | Experimental | Transporte não oficial, sujeito a desconexão ou restrição |
| Financeiro | Asaas | Sandbox MVP | Verificação de conexão e base para evolução |
| IA | Interface SENA AI | Base técnica | Experiência inicial e respostas demonstrativas/contextuais |
| IA | Copiloto com ferramentas reais | Planejado | Primeira prioridade: agendamento supervisionado |
| IA | Autopilot | Planejado | Autonomia progressiva por política e risco |
| Mobile | PWA de campo | Planejado | Interface independente do desktop, dados compartilhados |
| Produtos físicos | Service Tag / TAP | Conceito | QR/NFC conectado a ativos, recorrência e relacionamento |

## Dependências externas relevantes

Algumas capacidades dependem de terceiros e não podem ser garantidas exclusivamente pelo Grupo SENA:

- autorização, tarifas e políticas da Meta;
- disponibilidade e escopos das APIs Google;
- disponibilidade, cobertura e condições das fontes do CNJ;
- homologação e regras do provedor financeiro;
- conectividade, hospedagem e infraestrutura do cliente;
- aceite e qualidade dos dados fornecidos pela organização.

## Regra de comunicação comercial

Uma funcionalidade só deve ser apresentada como operacional quando:

1. estiver habilitada no ambiente aplicável;
2. tiver sido testada com a integração externa necessária;
3. possuir responsável e procedimento de suporte;
4. seus limites estiverem documentados na proposta ou contrato;
5. controles de segurança e privacidade correspondentes estiverem ativos.
