# Empreendedores do Reino — Registro Mestre de Arquitetura e Decisões v0.1

**Data:** 02/10/2026

> “Empreender no Reino é o caminho. Empreendedores do Reino é quem nós somos.”

## 1. Finalidade
Este registro consolida decisões de produto, arquitetura, governança e operação para reduzir perda de contexto e retrabalho.

**Fluxo:** Preservar → Inspecionar → Comparar → Planejar → Validar → Implementar → Homologar.

## 2. Portabilidade
`LOVABLE = DEVELOPMENT ACCELERATOR, NOT PERMANENT INFRASTRUCTURE DEPENDENCY`

- SOURCE_CODE_PORTABILITY = YES
- DATABASE_PORTABILITY = YES
- AUTH_PORTABILITY = YES
- STORAGE_PORTABILITY = YES
- SECRETS_PORTABILITY = YES
- DOMAIN_PORTABILITY = YES
- INTEGRATION_PORTABILITY = YES
- CI_CD_PORTABILITY = YES
- BACKUP_PORTABILITY = YES
- EDGE_FUNCTION_PORTABILITY = YES
- OBSERVABILITY_PORTABILITY = YES
- DATA_EXPORT_PORTABILITY = YES

## 3. Estado real observado
- Commit-base homologado: `51a074889e59f625eafd2f2f440a43d8505ca0de`.
- Banco PostgreSQL via Supabase já está habilitado no stack atual da Lovable.
- Não contratar Supabase Pro externo agora apenas por causa do plugin.
- Site público ainda lê `src/data/profiles.json`.
- Papéis existentes: SUPER_ADMIN, GOVERNANCE_ADMIN e CHURCH_ADMIN.
- Banco de Talentos ainda não existe no banco.
- Liderança institucional por igreja ainda não foi modelada.

## 4. Governança
### Inicial
- 1 Super Admin.
- Até 2 auxiliares da Central.
- 1 Admin Local principal por igreja.
- Até 2 auxiliares locais.

### Futuro preparado
Super Admin → Admin Geral Adjunto → Admins por Macrorregião (Norte, Nordeste, Centro-Oeste, Sudeste, Sul) → auxiliares regionais → admins estaduais → auxiliares estaduais → Admin Local → auxiliares locais.

Papel e capacidades devem ser separados. Limites devem ser configuráveis, não hardcoded.

## 5. Liderança institucional
Por igreja: Pastor Presidente, Vice-Presidente e Líder do Projeto, com foto, mini-bio e página expandida. Liderança institucional ≠ permissão administrativa.

## 6. Prioridade Mesquita
- Corrigir footer global para “Empreendedores do Reino”.
- Convite individual para empreendedor preencher o próprio cadastro.
- Convite → preenchimento → validação local → declaração → ativação.
- Foto de perfil + até 9 adicionais.
- Administração Local refinada (6.2c).
- Página de liderança.
- Assistente do Reino no onboarding.

## 7. Empreendedor x Banco de Talentos
Diretório de empreendedores = oferta de produto/serviço.
Banco de Talentos = pessoa buscando emprego formal com empreendedores/empresas da rede.
Não misturar entidades nem fluxos.

## 8. Banco de Talentos — futuro
Matching estruturado. Contato liberado apenas após interesse mútuo.
Se contratado: registrar sucesso.
Se não contratado: feedback estruturado obrigatório do empreendedor; distinguir recusa do empreendedor, do candidato, incompatibilidade mútua e vaga cancelada.
Feedback serve para análise e melhoria, não punição automática.

## 9. Escalabilidade
Migrar/redistribuir só por gatilhos reais: latência, CPU/memória, storage, conexões, filas, matching, criticidade, redundância, compliance.

Níveis: Fundação → Crescimento → Alta Disponibilidade → Arquitetura Distribuída.

## 10. Backup
- Baseline: backup externo automático semanal, preferencialmente na madrugada de sábado, iniciando após 00:00 na transição de sexta-feira para sábado.
- Evoluir para diário e janelas menores conforme criticidade.
- Testar restore periodicamente.
- Cobrir banco, documentos, imagens/storage, configuração e código.

## 11. Próxima sequência
1. Manter este documento vivo e versionado.
2. Retomar 6.2c local.
3. Corrigir footer.
4. Implementar convite e self-onboarding.
5. Fechar validação, declaração e ativação.
6. Adicionar liderança institucional.
7. Preparar auxiliares/capabilities sem implementar hierarquia nacional inteira.
8. Só depois iniciar Banco de Talentos.
