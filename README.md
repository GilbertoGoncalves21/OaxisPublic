Oaxis — Plataforma SaaS de Gestão ESG (em construção)

O Oaxis é uma plataforma SaaS de Gestão ESG (Environmental, Social & Governance) com arquitetura multi-tenant, focada em facilitar a governança, a gestão documental e o acompanhamento de indicadores ambientais e sociais em empresas de diferentes portes.

Status do projeto: Em desenvolvimento ativo desde abril/2025 (versão pré-alpha).

=====================================================================
🔗 Acesso de demonstração
=====================================================================
URL: https://oaxis.com.br
Usuário (treinamento): treinamento@treinamento
Senha: 1234

Observação: este é um ambiente de demonstração. Não utilize dados sensíveis/privados.

=====================================================================
🚧 Por que “Criar conta” e “Recuperar senha” ainda não estão 100%?
=====================================================================
O ambiente atual de demonstração está hospedado com restrições que não permitem envio de e-mails transacionais (SMTP), o que impacta diretamente:
- Fluxo de verificação de e-mail ao criar conta;
- Fluxo de recuperação de senha;
- Funcionalidades que dependem de armazenamento de arquivos ainda estão desabilitadas neste ambiente de demo.

Em produção final, esses serviços serão provisionados com infraestrutura própria (ex.: VPS dedicada) e provedores de e-mail/armazenamento adequados.

=====================================================================
🧩 Principais módulos previstos
=====================================================================
- Dashboard ESG – visão consolidada de indicadores.
- Documentos – gestão de políticas, evidências e relatórios.
- Relatórios – geração e exportação de relatórios ESG.
- Governança – papéis, responsabilidades e trilhas de auditoria.
- Ambiental & Social – registro e acompanhamento de indicadores.
- Administração – usuários, perfis e permissões (RBAC).

O roadmap será expandido conforme validações com clientes piloto.

=====================================================================
🏗️ Arquitetura & Tecnologias
=====================================================================
Frontend
- Angular (v18) + Angular Material
- SPA responsiva, componentização, formulários reativos
- Integração via REST/JSON

Backend
- Kotlin + Spring Boot 3
- Spring Security (JWT), filtros por tenant
- JPA/Hibernate com Criteria API
- Padrões de Clean Code e camadas de serviço
- Testes (JUnit)

Banco de Dados
- PostgreSQL 15
  - Modelo multi-tenant
  - Tabelas padronizadas (ex.: id_codigo, status, dt_cadastro)
  - Índices nomeados explicitamente

Infraestrutura (atual e planejada)
- Ambiente de demo com restrições (sem SMTP e storage)
- Contêineres Docker (planejado)
- Reverse proxy Nginx (planejado)
- VPS dedicada para produção (planejado), com:
  - SMTP/serviço de e-mail transacional
  - Armazenamento de arquivos (objetos/evidências)
  - Observabilidade e logs centralizados

=====================================================================
🔐 Segurança & Conformidade (em andamento)
=====================================================================
- Autenticação e autorização com JWT.
- Perfis e permissões por módulo/ação (RBAC).
- Log de auditoria e trilhas de alterações (planejado).
- Boas práticas de hardening na publicação (planejado).

=====================================================================
🗺️ Roadmap resumido
=====================================================================
1. MVP navegável com módulos base e RBAC — EM CONSTRUÇÃO
2. Documentos com upload/versões (ativar após storage/SMTP) — PLANEJADO
3. Relatórios ESG com exportação (PDF/CSV) — PLANEJADO
4. Logs de auditoria e painéis de conformidade — PLANEJADO
5. Integrações externas (ex.: planilhas, ERPs) — PLANEJADO

Legenda: entregue/em andamento · planejado

=====================================================================
🧪 Como testar a demo
=====================================================================
1) Acesse https://oaxis.com.br
2) Use as credenciais de treinamento:
   - Usuário: treinamento@treinamento
   - Senha: 1234
3) Navegue pelos módulos disponíveis e simule fluxos básicos (consulta, navegação, filtros).
4) Não utilize informações reais/sensíveis.

=====================================================================
🤝 Contribuição
=====================================================================
No momento, não estamos recebendo PRs públicos. Sugestões e feedbacks podem ser enviados via Issues do repositório ou formulário de contato (quando disponível).

=====================================================================
📝 Licença
=====================================================================
Projeto proprietário. Todos os direitos reservados.
O acesso à demo é concedido apenas para avaliação e treinamento.

=====================================================================
📣 Contato
=====================================================================
- Site: https://oaxis.com.br
- (Em breve) Página de contato e materiais adicionais.

Nota ao leitor do repositório: Este repositório é apenas o README público de apresentação do Oaxis. O código-fonte permanece privado enquanto o produto evolui para o MVP estável.
