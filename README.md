# Oaxis — Plataforma SaaS de Gestão ESG (em construção)

O **Oaxis** é uma plataforma SaaS de **Gestão ESG (Environmental, Social & Governance)** com arquitetura **multi-tenant**, focada em facilitar a governança, a gestão documental e o acompanhamento de indicadores ambientais e sociais em empresas de diferentes portes.

> **Status do projeto:** Em desenvolvimento ativo desde **abril/2025** (versão pré-alpha).

---

## 🔗 Acesso de demonstração

- **URL:** https://oaxis.com.br  
- **Usuário (treinamento):** `treinamento@treinamento`  
- **Senha:** `1234`

> **Aviso:** ambiente de **demonstração**. Não use dados sensíveis/privados.

---

## 🚧 Por que “Criar conta” e “Recuperar senha” ainda não estão 100%?

O ambiente atual de demo está hospedado com restrições que **não permitem envio de e-mails transacionais (SMTP)**, o que impacta:
- Verificação de e-mail ao **criar conta**;
- Fluxo de **recuperação de senha**;
- Funcionalidades que dependem de **armazenamento de arquivos** (desabilitadas na demo).

> Em produção final isso será provisionado em VPS dedicada com SMTP e storage adequados.

---

## 🧩 Principais módulos previstos

- **Dashboard ESG** — visão consolidada de indicadores  
- **Documentos** — gestão de políticas, evidências e relatórios  
- **Relatórios** — geração e exportação (PDF/CSV)  
- **Governança** — papéis, responsabilidades e trilhas de auditoria  
- **Ambiental & Social** — registro e acompanhamento de indicadores  
- **Administração** — usuários, perfis e permissões (RBAC)

> O roadmap será expandido conforme validações com clientes piloto.

---

## 🏗️ Arquitetura & Tecnologias

**Frontend**
- Angular 18 + Angular Material  
- SPA responsiva, componentização, formulários reativos  
- Integração via REST/JSON

**Backend**
- Kotlin + Spring Boot 3  
- Spring Security (JWT), filtros por tenant  
- JPA/Hibernate (Criteria API)  
- Clean Code e camadas de serviço  
- Testes (JUnit)

**Banco de Dados**
- PostgreSQL 15  
- Modelo **multi-tenant**  
- Tabelas padronizadas (ex.: `id_codigo`, `status`, `dt_cadastro`)  
- Índices nomeados explicitamente

**Infra (atual e planejada)**
- Demo com restrições (sem SMTP e storage)  
- Docker & Nginx (planejado)  
- VPS dedicada (planejado): SMTP, storage de arquivos, observabilidade e logs

---

## 🔐 Segurança & Conformidade (em andamento)

- Autenticação e autorização com **JWT**  
- Perfis e permissões por módulo/ação (**RBAC**)  
- **Log de auditoria** (planejado)  
- Boas práticas de **hardening** (planejado)

---

## 🗺️ Roadmap resumido

1. **MVP navegável** com módulos base e RBAC — ✅ em construção  
2. **Documentos** com upload/versões (após storage/SMTP) — ⏳  
3. **Relatórios ESG** com exportação (PDF/CSV) — ⏳  
4. **Logs de auditoria** e painéis de conformidade — ⏳  
5. **Integrações** externas (ex.: planilhas, ERPs) — ⏳

---

## 🧪 Como testar a demo

1. Acesse **https://oaxis.com.br**  
2. Use as credenciais: `treinamento@treinamento` / `1234`  
3. Navegue e simule fluxos básicos (consulta, filtros)  
4. **Não** utilize informações reais/sensíveis

---

## 🤝 Contribuição

No momento, não recebemos PRs públicos. Sugestões e feedbacks: **Issues** do repositório.

---

## 📝 Licença

Projeto **proprietário**. Todos os direitos reservados.  
O acesso à **demo** é apenas para **avaliação** e **treinamento**.

---

## 📣 Contato

- Site: https://oaxis.com.br  
- (Sistema ainda em construção)
- Deseja saber mais, entre em contato pelo whatsapp (42)99953-3268

> Este repositório expõe **apenas** o README público do Oaxis. O código-fonte permanece privado até o MVP estável.
