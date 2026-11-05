# Jorge Mauro

Engenheiro de software no time do assistente virtual da **Prefeitura do Rio**, que atende o cidadão pelo WhatsApp.
Cuido do servidor MCP que entrega as ferramentas ao agente (Salesforce Agentforce) — consultas e emissão de guias
de IPTU e Dívida Ativa, busca web com Gemini — e da confiabilidade e observabilidade disso em produção.

## Na Prefeitura do Rio

**[app-mcp-server](https://github.com/prefeitura-rio/app-mcp-server)** · Python · FastMCP · GKE
Servidor MCP do agente da Prefeitura. Mais de 30 PRs mergeados, entre eles:

- Health checks, preflight de configuração e smoke test HTTP (Hurl) contra a imagem no gate do PR
- Busca web com Gemini: fallback automático entre modelos, bloqueio de temas eleitorais e redação de PII na consulta
- Dívida Ativa: endpoints v2 de emissão de guia com validação de entrada e débitos estruturados
- Logs no BigQuery sem perda no encerramento (batch + DLQ) e barreira global de redação de PII
- Observabilidade com OpenTelemetry e SigNoz: separação de ambientes e correlação de spans
- Migração do FastMCP 2 → 3 e tratamento de CVEs nas dependências

**[k6](https://github.com/prefeitura-rio/k6)** · TypeScript · k6 Operator no GKE
Teste de carga do canal de mensageria (MIAW) do Salesforce.

**[prefect_rj_iplanrio](https://github.com/prefeitura-rio/prefect_rj_iplanrio)** · Python · Prefect
Pipeline do relatório da whitelist do WhatsApp.

**Infraestrutura** (repositório privado) · Terraform · GKE
Restrição da exposição pública dos endpoints do MCP.

## Projetos

- **[desafio-tech-lead-cidadaos-vulneraveis](https://github.com/jmaurodev/desafio-tech-lead-cidadaos-vulneraveis)** —
  solução full-stack do desafio técnico de Tech Lead (Programa Pequenos Cariocas): API FastAPI com JWT e RBAC,
  dashboard em Next.js, testes e registro de decisões.
- **[fastapi-siasg-extractor](https://github.com/jmaurodev/fastapi-siasg-extractor)** —
  extrator de itens de pregão SRP do SIASGnet/comprasnet, com API FastAPI e interface web.

## Stack

Python · FastAPI · FastMCP · LLMs (Gemini) · Salesforce Agentforce · GCP (GKE, BigQuery, GCS) ·
Terraform · OpenTelemetry · SigNoz · k6 · Prefect · Next.js/TypeScript · GitHub Actions

## Contato

[LinkedIn](https://www.linkedin.com/in/maurowick)
