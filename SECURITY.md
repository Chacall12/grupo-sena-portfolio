# Política de segurança

## Relato responsável

Se você identificar uma possível vulnerabilidade relacionada ao Grupo SENA ou ao SENA OS, envie um relato privado para **contato@gruposena.com**.

Inclua, quando possível:

- descrição do comportamento observado;
- impacto potencial;
- passos mínimos para reprodução;
- ambiente, navegador ou integração envolvida;
- evidências sem dados pessoais desnecessários.

Não abra uma issue pública com credenciais, dados de clientes, documentos jurídicos, tokens, URLs assinadas ou instruções completas de exploração.

## Escopo deste repositório

Este é um repositório institucional. Ele não contém o código-fonte da plataforma nem deve receber:

- arquivos `.env`;
- chaves de API ou tokens OAuth;
- credenciais de banco ou serviço;
- certificados, PINs ou chaves privadas;
- dumps de banco;
- mensagens, contatos ou documentos de clientes;
- identificadores internos de infraestrutura;
- logs brutos de produção.

## Princípios do produto

- isolamento multiempresa;
- menor privilégio;
- RLS e validação no backend;
- segredos somente em ambiente server-side ou cofre apropriado;
- armazenamento privado para documentos e dados de alto risco;
- auditoria com minimização de conteúdo;
- validação de upload;
- dependências e workflows auditados;
- backup cifrado e testes de recuperação;
- confirmação humana em ações sensíveis.

## Conduta durante testes

- utilize somente contas e dados para os quais possui autorização;
- não interrompa serviços nem degrade integrações de terceiros;
- não realize engenharia social;
- não tente acessar dados de outra organização;
- não publique a falha antes de permitir triagem e correção razoáveis;
- respeite as políticas dos provedores conectados.

O recebimento de um relato não cria recompensa financeira, contrato ou autorização para testes invasivos.
