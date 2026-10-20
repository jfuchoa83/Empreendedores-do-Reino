# EMPREENDEDORES DO REINO — DOSSIÊ MESTRE INTEGRAL DE CONTINUIDADE

**Estado consolidado em 20/10/2026**  
**Finalidade:** anexar ou fornecer este arquivo em um novo chat e continuar o projeto sem reconstruir decisões, sem perder contexto e sem reabrir decisões já fechadas.

> Este documento NÃO é um resumo curto. Ele combina o estado vigente, o histórico técnico recuperado, decisões de produto, regras de operação, commits, documentos internos atuais e os dossiês históricos integrais. Quando houver conflito, use a hierarquia de autoridade definida abaixo.

---

# 0. COMANDO AO NOVO CHAT — LEIA ANTES DE QUALQUER AÇÃO

1. Leia este documento inteiro antes de propor mudança estrutural.
2. Para qualquer trabalho na plataforma, use primeiro o plugin/integrador da **Lovable** e inspecione o projeto real. Não reconstrua estado por suposição.
3. Projeto correto: workspace `3ad844cb1354ba0fac93`; projeto `5be37771-fee0-4f39-84c1-247dd649c87c`.
4. Marca pública: **Empreendedores do Reino**.
5. Administração: **Empreendedores do Reino — Central de Governança** / **Central de Governança**.
6. Domínio oficial, grafia EXATA: **https://empreendernoreino.com.br**.
7. Não usar **Rede Mãe** em nova UI, salvo legado técnico inevitável.
8. Não publicar produção sem autorização explícita. **“Execute” autoriza implementação; publicação exige “Publique”/autorização equivalente.**
9. **Implementado ≠ homologado.**
10. Consolidar correções relacionadas em uma rodada para economizar créditos.
11. Registrar problemas e corrigir em lote; interromper só quando algo bloquear o teste.
12. Não inventar perfis, serviços, contatos, sites, redes sociais, fotos, métricas ou resultados.
13. Fluxo permanente: **Preservar → Inspecionar → Comparar → Planejar → Validar → Implementar → Homologar.**

## PRÓXIMO PASSO IMEDIATO

O domínio e o `www` já estão **ATIVOS** na Lovable.

A configuração Auth, na última leitura confirmada, ainda estava assim:
- Site URL: `https://empreendedores-do-reino-mesquita.lovable.app`
- Redirect permitido: `https://empreendernoreino.com.br/**`
- Redirect permitido: `https://www.empreendernoreino.com.br/**`
- Redirects antigos `lovable.app`: preservados.

O agente não possui ferramenta para escrever a **Site URL**. O proprietário deve fazer manualmente na interface:

**More → Users → Auth settings → Advanced**  
(o suporte também descreveu **More → Cloud → Users → Auth settings → Advanced**)

Alterar **somente** Site URL para:

`https://empreendernoreino.com.br`

Salvar **sem mexer** na lista de Redirect URLs.

### Assim que o usuário disser “Site URL alterada”
O novo chat deve:
1. usar a Lovable para reler a configuração Auth;
2. confirmar Site URL no domínio novo;
3. confirmar os dois redirects `/**`;
4. confirmar redirects antigos preservados;
5. inspecionar SHA/diff atual;
6. pedir autorização explícita antes de publicar;
7. depois da publicação, homologar domínio/Home/igreja/busca/Sobre/origem;
8. executar um **Magic Link real** no novo domínio;
9. só então considerar a migração de domínio homologada.

---

# 1. IDENTIDADE, ORIGEM E VISÃO

**Empreendedores do Reino** é um ecossistema cristão de empreendedorismo, comunidade, desenvolvimento humano, conexão econômica e serviço. A primeira implantação real é a **Igreja do Nazareno de Mesquita**, mas o produto é multi-igrejas.

A origem conceitual é anterior à plataforma. O grupo **“Expandindo o Reino de Deus com o Empreendedorismo”** trabalha encontros quinzenais, desenvolvimento de empreendedores, rodadas de negócios, jantares trimestrais discutidos e temas como empreendedor aos olhos de Deus, prosperar sem se corromper e finanças bíblicas.

Marca pública: **Empreendedores do Reino**.  
Expressão/movimento: **Empreender no Reino**.  
Frase norteadora: **“Empreender no Reino é o caminho. Empreendedores do Reino é quem nós somos.”**  
Assinatura: **“Prosperar faz parte. Expandir o Reino é o propósito.”**  
Frase de compromisso: **“Minha prosperidade deverá aumentar minha capacidade de servir.”**

Mesquita é **laboratório/piloto**, não a identidade total do projeto.

---

# 2. PRINCÍPIOS DE LINGUAGEM, CULTURA E PROPÓSITO

Regra editorial aprovada: afirmar diretamente o que queremos construir. Não introduzir mentalmente um conflito para depois negá-lo.

Formulações aprovadas:
- **“Trabalho, empreendedorismo, geração de emprego, desenvolvimento profissional e prosperidade caminham juntos na construção de dignidade, desenvolvimento e capacidade de servir.”**
- **“Empreendedores e profissionais exercem vocações complementares, gerando oportunidades, fortalecendo famílias e contribuindo para o crescimento da comunidade.”**
- **“A prosperidade com propósito se expande do indivíduo para a comunidade, ampliando nossa capacidade de servir, desenvolver pessoas, gerar oportunidades e produzir impacto.”**
- **“Queremos ampliar a capacidade das pessoas e da comunidade de prosperar, gerar oportunidades, desenvolver talentos e servir cada vez melhor.”**

Liberalidade: o empreendedor deve entender desde a entrada que contribuir inclui **tempo, conhecimento, experiência, conexões, talentos e recursos**. No onboarding atual, **não mencionar mensalidade, cobrança ou valor financeiro**.

Ideia futura, não formalizada: **Instituto Empreender no Reino** como braço institucional/social para formação, empregabilidade, capacitação, desenvolvimento econômico local, pequenos negócios e projetos comunitários. Não constituir juridicamente sem fase própria com jurídico/contabilidade/estatuto/governança.

---

# 3. MÉTODO DE TRABALHO

Sequência: **Contexto → Exploração → Análise crítica → Validação → Priorização → Arquitetura → Execução → Homologação.**

Preferências do usuário:
- prompts Lovable longos, consolidados e objetivos;
- solução com passo a passo;
- parceria crítica, não concordância automática;
- separar brainstorming de decisão;
- registrar tudo e corrigir em lote;
- não publicar sem autorização;
- não afirmar prova visual/browser que não foi feita;
- não homologar só porque implementou;
- preservar histórico/auditoria;
- portabilidade futura.

---

# 4. NOMENCLATURA E UX

- Marca: **Empreendedores do Reino**
- Admin: **Central de Governança**
- Assistente: **Assistente do Reino**, nunca “IA” na interface.
- Busca local protagonista: **“O que você precisa hoje?”**
- Princípio: **HOME CONVIDA; PERFIL IMPRESSIONA**
- Visual: premium/editorial/private-club/executive/cinematic; navy + gold + ivory/white; evitar SaaS genérico.

---

# 5. ÂNCORAS TÉCNICAS

## Lovable
- Workspace ID: `3ad844cb1354ba0fac93`
- Owner: José Fernandes Uchôa
- Conta: `jf.uchoa.neto@gmail.com`
- Project ID: `5be37771-fee0-4f39-84c1-247dd649c87c`
- Nome interno: Reino Conecta
- Editor: https://lovable.dev/projects/5be37771-fee0-4f39-84c1-247dd649c87c
- Preview: https://id-preview--5be37771-fee0-4f39-84c1-247dd649c87c.lovable.app
- Produção Lovable histórica: https://empreendedores-do-reino-mesquita.lovable.app

## Domínio
- **https://empreendernoreino.com.br**
- www ativo/incluído.
- Cuidado absoluto com a grafia: **empreender**, não “empreendedor”.

## Supabase/Lovable Cloud
- Project ref: `nbhxhtuvtuhhbenumwym`
- PostgreSQL/Supabase gerenciado pela Lovable Cloud.
- Plugin Supabase do ChatGPT está instalado, mas a organização “Empreendedores do Reino” retorna zero projetos acessíveis e o project ref gerenciado rejeita ações diretas por permissão. Usar Lovable/Lovable Cloud para esse backend quando necessário.

## GitHub
- Repo: `jfuchoa83/Empreendedores-do-Reino`
- https://github.com/jfuchoa83/Empreendedores-do-Reino
- Registro histórico: `docs/REGISTRO_MESTRE_ARQUITETURA_DECISOES.md`

---

# 6. ESTADO DE VERSÃO E PRODUÇÃO

Último SHA observado do projeto:
`980af7584ff775a62fbe0231f01e0e2830acf6d5`

Implementação funcional da rodada Domínio/Home nacional:
`2224b334303f996a0739c8f81aa85cc815582295`

Última produção confirmada antes dessa rodada:
`acb85653e3600fe7014f79d46318a53e44f46d77`

Deployment confirmado anteriormente:
`e0543f50-b9d6-4d2d-b4aa-d6a850b9276a`

A versão com Home nacional/domínio/busca local/origem simples foi **implementada e testada, mas NÃO publicada**.

---

# 7. CRÉDITOS LOVABLE CONHECIDOS

- Comando 2: **3,6**
- Convite + Onboarding V1: **11,9**
- Onboarding 1.1: **8,9**
- Origem pública: **2,6**
- Magic Link: **2,2**
- Onboarding 1.2: **6,2**
- Pré-homologação 1.2.1: **5,1**
- Tela final 1.2.2: **3,7**
- Admin Local 1.3: **9,5**
- Rodada Domínio/Home nacional: custo integral não retornado — **não inventar**
- Investigação Auth/Site URL posterior: **2,7** (0,7 + 1 + 1)
- Não assumir saldo atual sem consulta.

---

# 8. DOMÍNIO, DNS, HOSTING E E-MAIL

Domínio comprado no Registro.br.

DNS concluído:
- A raiz → `185.158.133.1`
- CNAME `www` → `empreendernoreino.com.br`
- TXT `_lovable` → verificação
- TXT `_lovable.www` → verificação

Lovable mostra: **Ativo • www incluído**.

Não é necessário Hostinger para hospedar o site enquanto ele estiver na Lovable. Hostinger pode ser contratado depois apenas para e-mail profissional, usando MX/SPF/DKIM/DMARC, sem mover o site.

Migração futura da aplicação para outro hosting continua possível, mas exige migração técnica; o domínio pode permanecer o mesmo.

---

# 9. ARQUITETURA PÚBLICA MAIS RECENTE — IMPLEMENTADA, NÃO PUBLICADA

## Home nacional
`/` = apresentação nacional + **Encontre uma igreja**.
Não usar Mesquita como Home nacional.
Não usar foto da igreja como hero nacional.

## Igreja
`/igreja/nazareno-mesquita`
- Igreja do Nazareno de Mesquita
- foto real
- “O que você precisa hoje?”
- categorias
- perfis em destaque
- explorar todos
- texto local enxuto.

## Busca local
`/igreja/nazareno-mesquita/buscar?q=...`
Somente perfis PUBLISHED + ativos vinculados à igreja via `church_profiles`.

Perfil permanece canônico:
`/empreendedor/{slug}`

## Sobre
`/sobre?igreja=nazareno-mesquita` mostra retorno seguro:
**← Voltar para Igreja do Nazareno de Mesquita**

Whitelist; sem open redirect.

## Futuro
`/igreja/` permanece família válida.
Outras instituições poderiam futuramente ter `/comunidade/` ou `/instituicao/`, se aprovado.
Não criar `/loja/` agora.

---

# 10. MISSÃO, VISÃO, PROPÓSITO, HISTÓRIA E VALORES

**Missão:**  
“Fortalecer os empreendedores da comunidade por meio de conhecimento, visibilidade, conexões e ferramentas que aproximem produtos, serviços, talentos e necessidades, gerando desenvolvimento, oportunidades e maior capacidade de servir.”

**Visão:**  
“Construir uma rede de referência em desenvolvimento empreendedor e oportunidades dentro da comunidade, capaz de revelar talentos, fortalecer negócios, conectar necessidades e estimular uma cultura de prosperidade com propósito.”

**Propósito:**  
“Expandir o Reino por meio de pessoas e negócios fortalecidos, transformando prosperidade em capacidade de servir, gerar oportunidades e produzir impacto.”

História:
- 2016 — busca por conhecimento sobre empreendedorismo;
- 2018 — percepção de que o conhecimento precisava ser disseminado melhor;
- 2021 — ideia ganha forma na igreja a partir da desconexão entre necessidades e ofertas dos próprios irmãos.

Sete frentes:
Empreendedores; Conexões comerciais; Oportunidades profissionais; Necessidades da comunidade; Inteligência de demanda; Desenvolvimento econômico e social; Formação e desenvolvimento.

Valores:
Fé e propósito; Excelência; Integridade; Cooperação; Serviço; Prosperidade com propósito.

---

# 11. DIREÇÃO VISUAL E IMAGENS

Direção: Luxury / Premium / High-End / Editorial / Private Club / Executive / Cinematic.

Paleta histórica:
- #06254B Azul Principal
- #03162F Azul Escuro
- #E2C95C Ouro Claro
- #C8A93A Ouro Médio
- #9A7A1F Ouro Escuro
- #6B5312 Ouro Sombra
- #E2E6E9 fundo claro
- #8B99A6 azul acinzentado

Falta ainda uma camada visual fotográfica que faça a marca “Empreendedores do Reino” ser sentida: reuniões, networking, atendimento, planejamento, comunidade, liderança, marcas d’água discretas e overlays editoriais.

Não preencher com banco de imagens genérico só para “encher”.
Eventos/negócios reais devem usar fotos reais aprovadas.

Perfis: futuro canônico = **1 imagem principal premium + até 9 adicionais**, máximo 10. Legado logo/capa permanece até migração segura.

Assets aprovados:
- Sinergia: `/__l5e/assets-v1/7485b6c0-0882-4fd0-a1de-3d8774f38ca7/logo_sinergia.jpg`
- Reforço Escolar: `/__l5e/assets-v1/b1cf20c5-4eef-4b2c-a0f3-6d92aff2d18c/marca_reforco_escolar_henrique.jpg`
Não regenerar sem pedido.

---

# 12. IGREJA PILOTO E TERRITÓRIO

- **Igreja do Nazareno de Mesquita** — DB slug `igreja-do-nazareno-de-mesquita`; status ACTIVE; Avenida União, 1400, Santa Terezinha, Mesquita/RJ; território CONFIRMED.

Endereço canônico:
**Avenida União, 1400, Santa Terezinha, Mesquita/RJ**
Nunca usar “Centro” sem nova confirmação.

Hierarquia futura:
**Brasil → Macrorregião → Estado → Região → Cidade/Município → Bairro → Igreja → Endereço**

Cidade organiza; igreja identifica.
Slug público atual: `nazareno-mesquita`
DB slug: `igreja-do-nazareno-de-mesquita`

---

# 13. BUSCA — REGRAS VIGENTES

Fonte pública atual: banco de dados. `profiles.json` é rollback/test fixture.

Busca centralizada em `src/lib/profiles.ts`.
Fronteira de palavra: “casa” não casar dentro de “casamento”; “ar” não casar dentro de “Farias”.

Mapeamentos importantes:
- energia solar → Força Solar
- segurança / segurança privada / vigilante armado / vigilante desarmado / segurança pessoal privada / transporte executivo / transfer / traslado executivo → Força Tarefa
- portaria / vigia / auxiliar de serviços gerais / ASG / bombeiro civil / auxiliar administrativo / recepcionista → FT Portaria
- aula de reforço / aulas de reforço → Reforço Escolar
- engenharia / arquitetura → Sinergia
- maquininha de cartão → Ton
- material de higiene / limpeza → Higiene
- refrigeração / ar → Refrigera Tec
- casa → Xavier
- casamento → Cordas

Genéricos registrados:
- limpeza → Higiene primeiro, FT Portaria depois
- serviço de limpeza → FT Portaria primeiro, Higiene depois
- condomínio → Força Tarefa, depois FT Portaria
- projeto → Refrigera Tec, depois Sinergia
- obra/reforma/construção → Farias, depois Sinergia

Taxonomia Construção x Engenharia continua hipótese a validar, não alterar por suposição.

---

# 14. 12 PERFIS PÚBLICOS — SNAPSHOT REAL

| Nome | Slug | Categoria | Telefone | Instagram | Website |
|---|---|---|---|---|---|
| Consultor Ambiental | `consultor-ambiental` | Consultoria Ambiental | 21 97213-4461 | — | — |
| Cordas de Amor Cerimônias | `cordas-de-amor-cerimonias` | Cerimonial e Celebrações | 21 96876-8831 | — | — |
| Farias Construções | `farias-construcoes` | Material de Construção | 21 99080-5240 | farias.const | — |
| Força Solar do Brasil | `forca-solar` | Energia Solar | 21 96520-9171 | forcasolardobrasil | — |
| FT Portaria | `ft-portaria-terceirizacao` | Terceirização de Serviços | 21 96593-0473 | — | — |
| Força Tarefa Segurança Privada | `grupo-forca-tarefa-seguranca` | Segurança Privada | 21 96593-0473 | — | — |
| Higiene, Limpeza e Descartáveis | `higiene-limpeza-descartaveis` | Higiene, Limpeza e Descartáveis | 21 96593-0473 | — | — |
| Reforço Escolar | `reforco-escolar-henrique` | Reforço Escolar | 21 99682-1985 | — | — |
| Refrigera Tec | `refrigera-tec` | Refrigeração e Ar-Condicionado | 21 97968-6874 | — | — |
| Sinergia | `sinergia-engenharia-arquitetura` | Engenharia e Arquitetura | 21 3273-7362 | br.sinergia | — |
| Ton — Maquininha de Cartão | `ton-maquininha-cartao` | Maquininha de Cartão | 21 99682-1985 | — | — |
| Xavier Imóveis | `xavier-imoveis` | Corretor de Imóveis | 21 98431-4779 | xavierimoveisrj | — |

Regras:
- nenhum website cadastrado no snapshot;
- não inventar redes sociais;
- Força Tarefa: vigilante armado, vigilante desarmado, segurança pessoal privada, transporte executivo/transfer/traslado. Remover “portaria” e “aluguel de carro/van”.
- FT Portaria: portaria, vigia, ASG, bombeiro civil, auxiliar administrativo, recepcionista.
- Reforço: “aula de reforço/aulas de reforço” como intenção; matérias/níveis oficiais precisam confirmação antes de ampliar.
- Cordas: o banco atual registra telefone **21 96876-8831** e Instagram vazio. Documentos históricos tiveram outro contato; não restaurar automaticamente.

---

# 15. CENTRAL DE GOVERNANÇA

SUPER_ADMIN — regra canônica:
> SUPER_ADMIN tem autoridade total sobre a rede e pode executar, a partir da Central, toda ação local em qualquer igreja, sem precisar trocar de papel para ganhar permissão.

Seleção de igreja = alvo/auditoria, não redução de autoridade.

GOVERNANCE_ADMIN não recebe automaticamente autoridade local de publicação.

Autorização:
- memberships + role_definitions + escopo NETWORK/CHURCH;
- contexto visual não concede permissão;
- RPCs SECURITY DEFINER revalidam escopo;
- MFA para roles que exigem;
- audit_log protegido;
- soft delete/arquivo;
- liderança institucional ≠ papel administrativo.

---

# 16. LIDERANÇA INSTITUCIONAL

Por igreja:
- Pastor Presidente
- Vice-Presidente
- Líder do Projeto

Foto + mini-bio + expansão.
Pastor Presidente e Líder do Projeto influenciam readiness; Vice não bloqueia.

Pr. Amadeu Aparecido Teixeira é referência histórica da Igreja do Nazareno de Mesquita; usar somente dados institucionalmente confirmados.

UI de liderança já foi implementada, mas homologação visual é separada.

---

# 17. CONVITE DO EMPREENDEDOR — SEGURANÇA

- `entrepreneur_invitations` separado de convite admin.
- 32 bytes / 256 bits.
- SHA-256 persistido; plaintext só na criação.
- 24h.
- claim atômico e uso único.
- e-mail confirmado deve corresponder.
- cria DRAFT + revisão + vínculo.
- owner não ganha admin membership.
- igreja imutável.
- SMS/telefone auth desabilitado.
- WhatsApp apenas para envio manual.
- V1 exige e-mail.

Retomada:
- `/acesso-cadastro`
- Magic Link para conta existente
- `shouldCreateUser:false`
- sem duplicação
- cooldown/auditoria
- token consumido não reutilizado.

---

# 18. ONBOARDING V1.2

Princípio:
**“O empreendedor declara a atividade e a oferta. O sistema organiza a taxonomia.”**

Etapa 1: negócio/tipo, responsável, papel; igreja read-only.  
Etapa 2: WhatsApp obrigatório, e-mail read-only, IG/site opcionais.  
Etapa 3: `primary_activity` livre 3–200 + `catalog_gap`; sem escolha de categoria oficial; “Catálogo em análise”.  
Etapa 4: até 10 itens de oferta; nome obrigatório; descrição opcional.  
Imagens: logo/capa legado opcional; 1+9 depois.  
Apresentação: tagline/curta/completa; Assistente ainda não integrado.  
Revisão: amigável; confirmação humana.  
DRAFT/CHANGES_REQUESTED editável; IN_REVIEW somente status; COMPLETED separado.

Tela final 1.2.2 foi corrigida para mobile/tablet/desktop e diferencia “Aguardando validação” de “Cadastro aprovado e publicado”.

---

# 19. BOAS-VINDAS, ASSIDUIDADE E LIBERALIDADE — APROVADO CONCEITUALMENTE, PENDENTE

Antes da etapa 1, criar boas-vindas/ciência:
- participação é desenvolvimento, relacionamento, cooperação e serviço;
- encontros quinzenais fazem parte do compromisso;
- imprevistos legítimos podem ser justificados;
- duas faltas consecutivas não justificadas ou ausências recorrentes não justificadas podem gerar conversa com liderança e reavaliação da participação;
- redação pastoral/elegante, não punitiva;
- checkbox de ciência.

Liberalidade:
contribuir, dentro das possibilidades, com tempo, conhecimento, experiência, conexões, talentos e recursos.

**Não falar de mensalidade/dinheiro no onboarding atual.**

---

# 20. ADMIN LOCAL 1.3 — IMPLEMENTADO

Visão Geral sem criação redundante; panorama.
Menu implementado:
- Visão geral
- Empreendedores
- Validação local

Ações por status, acompanhamento read-only, 7 etapas, contato autorizado, reenviar acesso por e-mail/WhatsApp, sem duplicar cadastro.

Resíduos sinalizados:
- “Pedidos de necessidade em aberto” na visão geral;
- “Verificar convites” refere-se a convites administrativos e pode confundir;
- itens “Em preparação” podem atrapalhar apresentação;
- PENDING WhatsApp genérico não leva token e pode parecer reenvio;
- arquivamento local de onboarding não foi ampliado; SUPER_ADMIN mantém autoridade.

---

# 21. NOVA ORGANIZAÇÃO DO ADMIN LOCAL — DECIDIDA, AINDA PENDENTE

Menu desejado:
**Visão Geral → Empreendedores → Convites enviados → Validação local**

Visão Geral:
somente indicadores.

Empreendedores:
somente cadastros/perfis da igreja.
Tabela:
**Empreendimento | Responsável | Categoria | Status | Atualizado | ⋮**
Ações por status.

Convites enviados:
- Convidar empreendedor
- Adicionar manualmente
- acompanhar porta de entrada

Validação Local:
somente `IN_REVIEW`.
Aprovar/publicar ou devolver para ajustes.
Motivo obrigatório na devolução.

Pendência funcional:
ao devolver, enviar **e-mail automático** ao empreendedor com motivo e orientação para retomar. Isso ainda não está implementado.

---

# 22. MAGIC LINK E E-MAIL

Problemas históricos:
- auth-bridge “Acesso negado”;
- branding “Reino-Conecta”;
- inglês “Confirm your signup / Verify Email”.

Correções:
- origem pública fixa;
- Magic Link only;
- sessão verificada/claim;
- `/acesso-cadastro`.

Teste real anterior chegou a entregar e-mail e criar/claimar cadastro.

Pendências:
- branding/template em PT-BR ainda não homologado;
- Site URL atual precisa ser alterada manualmente para o domínio novo;
- manter redirects antigos durante transição.

---

# 23. EXPERIÊNCIA DO VISITANTE

Jornada:
**Necessidade → Busca → Resultado → Perfil → Contato → Negócio → Avaliação → Apoio**

Home nacional explica o movimento.
Página da igreja resolve a necessidade local.
Perfil apresenta o empreendedor.
Pós-compra: **Ponto de Apoio** primeiro, **Avaliações** depois.

---

# 24. PONTO DE APOIO

Nome oficial já definido.
Canal privado para problema, dúvida ou necessidade de apoio envolvendo produto/serviço de empreendedor.
Sem exposição pública.
Entrada futura contextual em perfil/contato/pós-compra.
Ainda não implementado.

---

# 25. AVALIAÇÕES

Pós-serviço/produto real.
Governança/antiabuso.
Pode medir atendimento, qualidade, combinado, comunicação, resolução, nota e comentário.
Sem ranking humilhante.
Moderação de comentários.
Ainda não implementado.

---

# 26. TELEMETRIA — ATUAL

Eventos e contagens no snapshot de 20/10/2026:
- profile_view: **117**
- search_submitted: **41**
- whatsapp_click: **26**
- instagram_click: **22**
- search_zero_results: **7**

Origem simples implementada no código, não publicada:
- `?origem=whatsapp`
- `?origem=instagram`
- `?origem=telao`

Whitelist, sessionStorage, gravação em `event_properties`, sem novo PII.
Não ampliar agora para sistema pesado de campanhas/UTM.

---

# 27. TELEMETRIA FUTURA E INTELIGÊNCIA

Funil futuro:
visitante → pesquisa → resultado → perfil → contato → avaliação/apoio.

Dashboards central/local/empreendedor.
Inteligência de Demanda distingue:
1. falha da busca;
2. ausência de fornecedor;
3. oportunidade nova.

Saúde e Capacidade é painel separado, por recurso, sem média inventada.

---

# 28. CAPACIDADE / SIMULTANEIDADE

Snapshot observado:
- banco ~15 MB;
- max_connections 60;
- 11 conexões presentes em um momento.

Isso NÃO significa 60 visitantes máximos.

Busca é leve porque o ranking é feito no navegador sobre poucos perfis.
Para 30–60 acessos concentrados não foi identificado bloqueio arquitetural imediato, mas capacidade exata não foi homologada.

Teste futuro:
**10 → 25 → 50 → 100 simultâneos**, medindo latência, erros, banco e perda de eventos.

---

# 29. DIVULGAÇÃO

Para o lançamento inicial:
- WhatsApp
- Instagram
- QR do telão

Links simples:
`/igreja/nazareno-mesquita?origem=whatsapp`
`...?origem=instagram`
`...?origem=telao`

Ideia futura no Admin: seção **Divulgação** em “Crescimento”. Não implementar dashboard complexo agora.

---

# 30. BANCO DE TALENTOS / EMPREGABILIDADE

Separado do diretório de empreendedores.

Visão futura:
matching, oportunidades, contratação, feedback estruturado e melhoria.

Ideia recente: se alguém ficar desempregado por período prolongado (exemplo discutido: 45 dias), a rede pode investigar causas e mobilizar currículo, qualificação, capacitação e oportunidades. Ainda não é regra implementada.

---

# 31. ASSISTENTE DO REINO

Frase canônica:
> “O empreendedor fala do jeito dele. O Assistente do Reino entende, organiza, pergunta o que faltar e transforma a conversa em Categoria → Necessidades → Oferta → Apresentação.”

Nunca inventa.
Confirma antes de preencher/publicar.
Não cria taxonomia global sozinho.
Ainda não implementado.

---

# 32. DECLARAÇÃO SOLENE

**Declaração Solene de Compromisso do Empreendedor do Reino**

Frases registradas:
- “O Empreendedor do Reino não existe apenas para gerar negócios. Existe para gerar impacto, desenvolvimento e expansão do Reino.”
- “A função do empreendedor do Reino não é ganhar dinheiro. Ganhar dinheiro é resultado.”
- “Prosperar faz parte. Expandir o Reino é o propósito.”
- “Minha prosperidade deverá aumentar minha capacidade de servir.”
- “Minha prosperidade não será minha mensagem. Minha vida será a mensagem. E os frutos confirmarão aquilo que estou vivendo.”

Fluxo futuro:
submit → validar → declaração → imprimir → assinar → upload → confirmar → ativar.

---

# 33. REVISTA

Rota dormente/legado.
Fora do menu/Home/footer na versão recente.
PDF V0 antigo foi rejeitado como autoridade editorial.
Não reabrir até existir fonte editorial canônica.

---

# 34. BACKUP E PORTABILIDADE

> “A Lovable é nosso acelerador de desenvolvimento, não uma dependência arquitetural irreversível.”

> “Não queremos abandonar a Lovable. Queremos preservar o direito técnico de abandoná-la.”

Portabilidade de código, banco, auth, storage, secrets, integrações, CI/CD, backup, edge, observabilidade e dados.

Backup baseline: semanal; evoluir conforme criticidade; testar restore.

---

# 35. ROADMAP CANÔNICO

**A — Empreendedor redondo**
ciclo real + Admin Local + convite + onboarding + e-mail + imagens + Assistente + Declaração.

**B — Comprador**
Ponto de Apoio → Avaliações.

**C — Inteligência**
telemetria completa → dashboards → Inteligência de Demanda → Saúde/Capacidade.

**D — Território/Governança**
Território v2 → URLs/slug → governança/auditoria → backup/restore.

**E — Expansões**
Banco de Talentos → Central de Conhecimento → mensuração social/econômica → demais módulos.

Atalho:
**Empreendedor redondo → Ponto de Apoio → Avaliações → Telemetria/Inteligência → Território/Governança → expansões.**

---

# 36. ESTADO REAL DO BANCO — SNAPSHOT 20/10/2026

- published_active: **12**
- revisions_in_review: **1**
- revisions_draft: **1**
- revisions_changes_requested: **1**
- invitations_claimed: **3**

Esses valores são snapshot; reler antes de chamar de “atuais” em data futura.

---

# 37. SEGURANÇA

- RLS por escopo.
- memberships + role_definitions.
- MFA AAL2 quando exigido.
- convites não escalam papel.
- audit_log protegido/append-only para app.
- service role nunca frontend.
- uploads pendentes privados.
- analytics pseudônimo.
- sem fingerprinting.
- soft delete/histórico.
- mudanças sensíveis com motivos/auditoria.

---

# 38. PONTOS QUE NÃO PODEM SER ESQUECIDOS

1. Site URL Auth ainda antiga — próximo passo.
2. Template Magic Link/branding ainda pendente.
3. Domínio novo ativo; Home nacional ainda não publicada.
4. Separação “Convites enviados” ainda não implementada.
5. E-mail automático ao devolver ajustes ainda não implementado.
6. Imagens 1+9 ainda não migradas.
7. Galerias reais ainda não abastecidas.
8. Ponto de Apoio/Avaliações não implementados.
9. Campanha/telemetria deliberadamente mínima.
10. Teste formal de carga não executado.
11. Território v2 não iniciado.
12. Comando 2 tem teste técnico forte, mas homologação visual separada.
13. Arquivamento local do onboarding não autorizado.
14. Não restaurar dados históricos conflitantes sem consultar banco atual.
15. Não dizer que vídeo foi analisado quando a ferramenta falhou.

---

# 39. PRÓXIMA SEQUÊNCIA EXATA

### 1 — Manual
Lovable → More → Users → Auth settings → Advanced  
Site URL → `https://empreendernoreino.com.br`  
Não mexer nos redirects.

### 2 — Verificação
Novo chat relê Auth e confirma tudo.

### 3 — Pré-publicação
Confere SHA/diff e rotas.

### 4 — Publicação
Somente com autorização explícita do usuário.

### 5 — Homologação pública
Raiz, www, Home nacional, Mesquita, busca local, perfis, Sobre/retorno, responsividade, origem.

### 6 — Magic Link real
Convite/retomada/e-mail/retorno/sessão/claim.

### 7 — Fechamento
Só depois homologar domínio e retomar Admin Local: **Convites enviados + Validação Local + e-mail de devolução**.

---

# 40. HIERARQUIA DE AUTORIDADE

1. última instrução explícita do usuário;
2. estado técnico real atual via Lovable/banco;
3. seções vigentes deste dossiê;
4. roadmap/AGENTS atuais;
5. conteúdo canônico aprovado;
6. dossiês históricos;
7. prompts/materiais antigos.

---

# ANEXO A — LEDGER DE COMMITS/EDIÇÕES LOVABLE

| Data | SHA | Mensagem | Status |
|---|---|---|---|
| 2026-09-29 | `48f0f75195ec20fe38f922b99c8702155f1230ee` | Criou estrutura V0 completa | completed |
| 2026-09-29 | `c350ae527ee7009c398633828e3d51b249cb27e3` | Applied Institutional Editorial | completed |
| 2026-09-29 | `a162d55f458984ce780918dff3bb391cd82832b7` | Aplicou assets reais da V02 | completed |
| 2026-09-29 | `fad5f984e8301d3a4836c7ac32d8047523b6ce38` | Ajustou identidade e logos R1.2 | completed |
| 2026-09-29 | `fc3774f6cf0f66f0e20fe85ff2f8a64f9ec06147` | Aplicou V0 R1.2 assets reais | completed |
| 2026-09-30 | `8f88c9847a64b921eaf51d7ba049556e02255405` | Validou e corrigiu perfis | completed |
| 2026-10-01 | `e3395cd17ad8fcd56cae730799c6023ab8e41093` | Fixou galeria e limites ingestão | completed |
| 2026-10-01 | `f917b7ed39309de1afcf4c7013652940e2e7af95` | Executa Etapa 0 e corrige type | completed |
| 2026-10-01 | `505ccbbaf43e2170ef4cb0fba6e3230f8f884629` | Adicionou termos de busca | completed |
| 2026-10-01 | `6d7b5bca92002707e2bbc15f4e65fd1defec0519` | Corrigiu busca por palavras inteiras | completed |
| 2026-10-01 | `ff2478ef4ede66a5fcd2c5c4fc7311e41e60fb91` | Atualizou perfis de busca | completed |
| 2026-10-01 | `101331c83061208deda8eec0f3563853c648bfcc` | Criou tabelas e migração | completed |
| 2026-10-01 | `cd643778366a439686211fcf1e773317476af7d3` | Concluída reconciliação Etapa 4 | completed |
| 2026-10-01 | `397d8a4440c5529de8020274b34bb3c215ac0bf2` | Instalou arquitetura multi-tenant | completed |
| 2026-10-01 | `2291d102943b63ad816cadcd752eb3aa341b07f5` | Implementou gate de segurança | completed |
| 2026-10-01 | `d0439ced2e12bdd7d715c62e9015c8db1f45e4d6` | Revisou plano Etapa 6.2 | completed |
| 2026-10-01 | `f15cf6794467fca71b6b5b43317721dab27635f2` | Implementou estrutura 6.2a DB | completed |
| 2026-10-01 | `fecbde2738e43e19930574047f6c70f81b1ca257` | Concluiu a etapa 6.2a admin | completed |
| 2026-10-01 | `6961965eaa8db1d97a9fef0c1e3837b5dc511a1b` | Forçou nova versão da prévia | completed |
| 2026-10-01 | `928f5035ad1d982a43789bcd139ca8e2bb5dc7e4` | Update plan | completed |
| 2026-10-01 | `3cd02525fbad5b72aca45dcb2d4f1be96901ed01` | Update plan | completed |
| 2026-10-01 | `20559ef3d5483ea6ac0b5113a76d105e1b4d6caa` | Implementou etapa 6.2b completa | completed |
| 2026-10-01 | `fa3d412ec0a9d5375b1486fa740aadaeab72e926` | Update plan | completed |
| 2026-10-01 | `6dc7fc1a36039c2d029ee9265185b8388c5acb39` | Update plan | completed |
| 2026-10-01 | `56d70adcff5f7f3b3c1d91aecd696221c038830e` | Ajustou estimativa de custo | completed |
| 2026-10-02 | `51a074889e59f625eafd2f2f440a43d8505ca0de` | Homologou etapa 6.2b da CEV | completed |
| 2026-10-03 | `a11c148e73a0447fb7f03681bf00926c429d05d0` | Update plan | completed |
| 2026-10-03 | `11a057042deecc3af9ef0e1c664aacf2b3e4f460` | Update plan | completed |
| 2026-10-03 | `8dee62e85151935ec4533fbebaf15b445d7ca761` | Corrigiu logos no banco | completed |
| 2026-10-04 | `7fab663b1923a2eabe778f71c168b060844fe57a` | Migrou perfis do banco p/ site | completed |
| 2026-10-05 | `a3b7c888abf2da9253f803995972e1d61cc9e041` | Corrigiu 3 textos admin | completed |
| 2026-10-05 | `2fa858b217a1f62b662441481bb4c65d97eb12dd` | Update plan | completed |
| 2026-10-05 | `8e5881c31cdad4943328cc7ee7402e73b2cb7702` | Update plan | completed |
| 2026-10-06 | `8145fe751f2626c0f84e5779b96270216b83e985` | Update plan | completed |
| 2026-10-06 | `b699ecbf9b650da36318e8bc302b6d2af246e6c5` | Aplicou checklist e admin v2 | completed |
| 2026-10-07 | `b602ace4c30c21ea7a064ddd6c271e2a175da925` | Adicionou Saúde da Plataforma | completed |
| 2026-10-08 | `020dfa66cd05a3905155923e22e4d7c03d77cf76` | Adicionou verificação ao checklist | completed |
| 2026-10-13 | `686573d82ecab5110ee1626265806cdfc23d9293` | Fechou Liderança Igreja | completed |
| 2026-10-15 | `8c0b71c1a011bfeaf6bb7cef1a56ab475fc10411` | Compactou orientações do projeto | completed |
| 2026-10-17 | `47863dbab3647ce8f6767575c11a05224e512f70` | Atualizou visual da vitrine | completed |
| 2026-10-17 | `8664e188d7650ef01be456131aa4ef32ad16a1f7` | Lançou Vitrine Pública 1.1 | completed |
| 2026-10-17 | `00c18d188e6f92ab50abb0c09f8806825b18e7c1` | Adicionou seção história Sobre | completed |
| 2026-10-17 | `936ef226411051c38aab2320a1322eae9fb9924b` | Adicionou seção Sobre 2.2 | completed |
| 2026-10-17 | `95053e47e765bf1eefd43c9bfc708566ce16a16d` | Vitrine 1.2 implementada | completed |
| 2026-10-17 | `5683965554667a67f7188f867fafd70aafed2baf` | Publicou perfis públicos v1.0 | completed |
| 2026-10-17 | `d06fd07ee65be00eb6294d696ae91a112b146f92` | Corrigiu vitrine pública | completed |
| 2026-10-17 | `6176ace997f6396d660fae7d011dfeaae9549073` | Corrigiu microcopy na vitrine | completed |
| 2026-10-17 | `adb3f3211112ead2b4e22c5c2b7921ecc64c3660` | Fechei o Comando 2 | completed |
| 2026-10-17 | `d9a5231cb98e7179239334f4c3611e49ab97f4d2` | Compactou reforços das regras | completed |
| 2026-10-18 | `ec9f18ee52195eb146412f491a6861ca8f0707dd` | Otimizou a entrega do onboarding | completed |
| 2026-10-18 | `f23d9aa11b711f6e26b14a306333564bf9bcea56` | Centralizou origem pública | completed |
| 2026-10-18 | `b01b1f44d52d5c4eb922ee013ee3935d79540d2b` | Isolou origem da prévia | completed |
| 2026-10-18 | `8329cf16f8e31407387b7377702dd8aa833f8bb5` | Implementado onboarding v1.2 | completed |
| 2026-10-18 | `dedc09386560d9268c11b8c6e9363ccdf28456f0` | Preservou snapshot admin | completed |
| 2026-10-19 | `8fc81beeaa6cc5ce31df60993279ebf3252ae5a3` | Corrigiu tela final responsiva | completed |
| 2026-10-19 | `acb85653e3600fe7014f79d46318a53e44f46d77` | Adicionou ações para admin local | completed |
| 2026-10-19 | `2224b334303f996a0739c8f81aa85cc815582295` | Raccourci les règles du projet | completed |
| 2026-10-20 | `46f1a38f1e9bc5d29c8e79b1afa248da2e4b15b6` | Update plan | completed |
| 2026-10-20 | `980af7584ff775a62fbe0231f01e0e2830acf6d5` | Update plan | completed |

---

# ANEXO B — ROADMAP.MD VIGENTE NO SHA 980af...

```markdown
# V0 — Empreendedores do Reino

## Roadmap mestre — prioridades atuais (histórico preservado abaixo)

### PRIORIDADE A — Fechar ciclo do empreendedor / apresentação
- [ ] Homologação real convite → cadastro → retomada → envio → validação → devolução → reenvio → publicação; depende de entrega real e sessões do empreendedor/admin com MFA quando exigido.
- [x] Admin Local 1.3: Visão Geral sem criação, menu sem atalho redundante, acompanhamento somente leitura com contato autorizado, 7 etapas/regras reais, retomada por e-mail/WhatsApp e ações por status. Implementado; homologação operacional real pendente.
- [ ] Encerrar/arquivar onboarding em andamento pelo Administrador Local — autorização atual é exclusiva do Superadministrador; não ampliada nesta rodada. Convites de perfis já arquivados saem da operação.
- [ ] Template/branding Magic Link em português “Empreendedores do Reino” — permanece pendente sem domínio de envio/configuração operacional confirmada.
- [ ] Imagens canônicas: exatamente 1 imagem principal premium + até 9 adicionais, sem capa separada; preservar legado até migração segura.
- [ ] Conferência visual final Admin Local e Validação Local em sessão real autorizada.
- [ ] Assistente do Reino no onboarding: conversa → Categoria → Necessidades → Oferta → Apresentação; nunca inventar dados, confirmação humana antes de publicar.
- [ ] Declaração Solene de Compromisso após cadastro/validação e antes da ativação definitiva; assinatura física, upload, versão/data/conferente.

### PRIORIDADE B — Experiência do comprador / comunidade
- [ ] **Ponto de Apoio** — nome oficial já definido do canal central para registrar problema, dúvida ou necessidade de apoio envolvendo produto/serviço de empreendedor; acompanhamento e resolução privados, sem exposição pública.
- [ ] Definir entrada contextual no perfil/contato/pós-compra.
- [ ] Avaliações pós-atendimento/compra do produto/serviço entregue: governança e prevenção de abuso.
- Nenhum desses módulos implementado nesta rodada.

### PRIORIDADE C — Inteligência / telemetria / demanda
- [ ] Instrumentar funil completo: visitantes, pesquisas/termos/zero-result, perfis, cliques WhatsApp/Instagram/site, convites, etapas/abandono do onboarding, validações, avaliações e Ponto de Apoio.
- [ ] Dashboards agregados com filtros por período, igreja, território, empreendedor, termo/necessidade; ranking de pesquisas/cliques e funil com contagens reais.
- [ ] Inteligência de Demanda: distinguir falha de busca × ausência de fornecedor × oportunidade nova.
- [ ] Saúde e Capacidade por recurso, gargalo relevante, histórico/intervenções e dados desatualizados sinalizados; sem média inventada.

### PRIORIDADE D — Território / governança
- [ ] Território v2 com mapa: Brasil → Macrorregião → Estado → Região → Cidade → Bairro → Igreja → Endereço.
- [ ] Página/URL única por igreja, slug global; cidade/bairro são território, não identidade.
- [ ] Comando 2 só homologar após validação visual final; Comando 3/Território depois.
- [ ] Refinar aprovações pendentes/histórico, auditoria legível e arquivo histórico.
- [ ] Backup/portabilidade e teste de restauração antes de escala relevante.

### PRIORIDADE E — Expansão posterior
- [ ] Banco de Talentos; Central de Conhecimento; resultados/mensuração social/econômica; Codex de Governança e demais módulos futuros registrados abaixo.

### Verificação da rodada Admin Local 1.3
- [x] A–C conferidos no código; D–G matriz de ações e componente de acompanhamento testados; J regra de WhatsApp PASS; H/I/K autorização, retomada sem duplicação, cooldown 60s, limite 5/h e auditoria PASS em transação com claims simuladas e rollback. Zero igrejas/vínculos de teste e 12 perfis públicos preservados.
- [x] M: 21 testes unitários PASS e compilação/typecheck automáticos OK. N: vitrine/busca/perfis sem diff funcional e smoke 200. Acompanhamento isolado em 390/768/1280 sem overflow, 7 etapas e sem erros; nenhuma rota/fixture na aplicação.
- [ ] Homologação real A–I: sessão do responsável autenticada, mas sem membership administrativo; não concedido papel nem contornado MFA. Reenvio real/recebimento do e-mail e navegação administrativa real não verificados. L não se aplica: nenhuma autorização nova de arquivo; encerramento local segue pendente.
- Nada publicado; Ponto de Apoio/Avaliações/Telemetria/Território/Assistente apenas registrados. Créditos observados entre consultas: 5,80 (não custo integral da rodada).

- [x] Estruturar dados locais, busca e componentes compartilhados
- [x] Construir Home, busca, perfil, Sobre, Revista e painel demonstrativo
- [x] Aplicar identidade editorial responsiva e acessível
- [x] Validar buscas, links, rotas e layouts em 390 px, tablet e 1440 px

## R1.2 — Identidade e acabamento

- [x] Aplicar a paleta oficial e a direção Institutional Editorial
- [x] Incorporar o pacote R1.2 com hero da igreja, logos reais e mapeamento de mensagens
- [x] Refinar header, hero, busca, cards, perfis, Sobre, Revista, painel e footer
- [x] Exibir apenas mensagens reais da base e manter monogramas onde não há logo fornecida
- [x] Corrigir a Revista para apresentar a imagem disponível como prévia, sem tratá-la como capa oficial
- [x] Revalidar busca, perfis, WhatsApp, Instagram, acessibilidade e responsividade

## Fase 1 — Fundação de dados e persistência

- [x] Ativar Lovable Cloud e criar o esquema persistente com RLS
- [x] Separar assets publicados na CDN e uploads pendentes privados
- [x] Migrar e validar os 12 perfis, textos editoriais e manifesto de assets
- [x] Instrumentar eventos essenciais sem identificação invasiva
- [x] Executar os 12 testes de aceitação e a auditoria final de segurança

## Fase 1 — Delta corretivo final

- [x] Permitir várias imagens destacadas no hero, ordenadas por posição
- [x] Preservar o limite de dez imagens e a posição única por perfil
- [x] Reforçar a ingestão pública de analytics e documentar a retenção do visitante
- [x] Revalidar dados, privacidade, galeria e ausência de regressão visual

## Etapa 5 — Fundação multi-tenant

- [x] Rede Mãe, igreja Mesquita, 12 perfis vinculados, papéis por membership com RLS
- [x] Auditoria central, troca segura de e-mail do admin geral, convite do admin inicial
- [x] Estrutura da administração central separada do público
- [ ] Envio de e-mails de segurança — aguarda provedor de e-mail
- [ ] MFA obrigatório do admin geral — aguarda ativação de MFA na autenticação
- [ ] Primeiro admin da igreja — aguarda e-mail definido

## Etapa 6.2a — Administração operacional (base)

- [x] Estados de publicação, revisões, status da igreja, pedidos de necessidade (aditivo, RLS, auditoria)
- [x] Seletor de contexto (Rede Mãe / Mesquita), só visual + auditoria
- [x] Painel base: igrejas, empreendedores, fila de revisão, pedidos, auditoria
- [x] Assistente "Adicionar empreendedor" em 7 etapas (IA visível e desativada)
- [x] Testes transacionais do banco
- [ ] Teste logado das telas no navegador — aguarda primeiro login real + segundo fator de jf.uchoa.neto@gmail.com

## Etapa 6.2b — Central de Governança
- [x] Shell próprio do admin, contextos NETWORK/OBSERVE/CHURCH, menus e painéis por contexto
- [x] Validação local (sem revisão central obrigatória); auditoria invisível ao CHURCH_ADMIN
- [x] GOVERNANCE_ADMIN + solicitações com justificativa e aprovação do SUPER_ADMIN
- [x] Arquivo Histórico (sem exclusão física) e estrutura territorial com Região curada pela Central
- [x] Testes do banco e regressão; não publicado
- [ ] Teste logado das telas — exige sessão real com segundo fator do usuário
- [ ] Endereço/região reais de Mesquita — aguarda confirmação da Central

## Futuro (só registrado)
- Banco de Talentos, Ponto de Apoio, Central de Conhecimento, Codex de Governança, Avaliações/Inteligência de Conteúdo, Resultados/Mensuração, Declaração de Compromisso, Assiduidade/presença, Assistente do Reino (Assistente de Gestão; nunca exibir "IA")

## ETAPA 6.2c
- [x] Pré-homologação 1.2.1: tabela local Empreendimento | Responsável | Categoria | Status | Atualizado | ⋮; igreja só no contexto local. Payload admin aceita metadados e RPC mescla snapshot para preservar campos omitidos. Complemento SQL v1_2 PASS com rollback: atividade livre sem categoria, categoria canônica obrigatória na publicação, devolução/reenvio e preservação de atividade/contexto/identidade/needs/brands/segments. Zero fixtures; 12 perfis públicos preservados; 15 unitários PASS; compilação automática OK; AGENTS 5.111 bytes. Nada publicado.
- [ ] Conferência visual da tabela 1.2.1 com Administrador Local — sessão real disponível não possui papel administrativo; nenhum papel concedido para teste. Homologação operacional permanece pendente.
- [x] Onboarding 1.2.2 — tela final responsiva + acompanhamento: card 100% na viewport (390/768/1280 sem overflow), CTA principal com quebra de linha e largura total no mobile (override local, sem tocar no Button global), nova mensagem de validação pela liderança, "Sair" com ênfase reduzida, acompanhamento IN_REVIEW com orientação, estado publicado com CTA ao perfil (slug = profiles.id, já correto). Inspeção visual via rota temporária removida após o teste. Nada publicado.
- [x] Bloqueador Magic Link/retorno do onboarding — corrigido em código: domínio público fixo, sem campos de código, retorno com sessão verificada e claim automático. Configuração Auth (Site URL/allow list) não acessível nas ferramentas disponíveis; template pendente (sem domínio de envio configurado). Aguardando novo teste real após publicação autorizada; não homologado nem publicado.
- [x] Onboarding do Empreendedor 1.1 — UX Premium + Convites + Cadastro Próprio + Validação Local — implementado, aguardando validação visual e operacional. Testes transacionais A–E/G/K/L/M/P/R/S PASS e escrita F PASS, 12 unitários PASS, compilação automática OK. Telas logadas H–J/N/O/Q/V pendentes por MFA; sem homologação operacional.
- [ ] Imagens 1+9 adiado: snapshot/RPCs privados suportam somente logo/cover; preservar aprovação, storage e perfis públicos exige migração completa posterior. UI temporária opcional com escolher/arrastar, preview e remover do cadastro; nenhum arquivo legado apagado.
- [ ] Homologar ciclo real com e-mail recebido, sessão do empreendedor e segundo fator administrativo; depois, Assistente do Reino completo.
- [x] Convite do Empreendedor + Onboarding Próprio 1.0 — implementado, aguardando validação visual e operacional do responsável; testes transacionais A–J/M/N/O e escrita própria PASS com rollback; 8 testes unitários PASS; compilação automática OK. SMS desabilitado: WhatsApp somente para envio do link; V1 funcional exige e-mail confirmado. Comando 2 e Vitrine Pública preservados.
- [ ] Convites V1: conferir entrega/retorno de e-mail real e fluxo completo logado (lista/modal/claim/cadastro/validação); sessão administrativa disponível exige segundo fator, não contornado. Testes de leitura RLS com identidade não administrativa ainda pendentes; não homologado.
- [x] Bloqueador do convite — origem pública canônica: links e redirects de e-mail usam helper central (`getPublicAppOrigin`) que rejeita lovable.dev/auth-bridge e cai no domínio publicado; link completo montado no servidor. Resolvido em código; homologação externa pendente — preview hospedado responde 401 fora do workspace (política da plataforma), exige publicação para prova externa. Não publicado.
- [ ] Onboarding imagens: migrar logo/capa privados legados para exatamente 1 foto premium + até 9 adicionais; nesta V1 uploads continuam opcionais, sem publicação automática. Assistente/Catálogo automático e Declaração fora desta rodada.
- [x] Subetapa A: rodapé global "Empreendedores do Reino"

- [x] Subetapa B (6.2c): logo_url de Sinergia e Reforço Escolar Henrique preenchidos no banco com assets aprovados existentes; demais divergências de arquivo de logo (código .jpg vs banco premium .png) apenas relatadas.

- [x] Subetapa A (6.2c): testes teste-01-dd7d32 e teste2-1aabb7 arquivados e auditados.
- [x] Site público (Início, Busca, Perfil) lendo do banco só perfis PUBLICADO+ativos — homologado: tipos OK, 26 rotas OK, 381 buscas (3 diferenças aprovadas); profiles.json só como cópia de segurança.
- [ ] Prova automatizada do 13º perfil — não executada (exige caminho de teste sem dado residual).
- [x] Microajustes: "Igrejas na rede", "Segurança da conta"/Superadministrador, rótulos curtos na auditoria.

- [x] Comando 1 (6.2c): Visão Geral sem blocos vazios, bloco Implantação (checklist a definir), Aprovações pendentes para o Superadministrador, Pedidos de necessidade fora dos menus — falta conferência visual com segundo fator.
- [ ] Comando 2 — implementação concluída e testes técnicos de autorização/segurança PASS; aguardando validação visual final do responsável para homologação. (Roteiro supabase/tests/etapa_6_2c_cmd2_close.sql, rollback, zero resíduo.)
- [ ] Comando 3 (6.2c): Território v2 com mapa e lista — aguarda Comando 2.

- [x] Comando 2.1 (fechamento do Comando 2): checklist verificável — cada requisito com ação contextual e fonte; Pastor Presidente e Líder do Projeto não confirmáveis até existir cadastro de liderança — aguarda validação visual.
- [x] UI de Liderança (Pastor Presidente, Vice-Presidente, Líder do Projeto): leitura, cadastro/edição via RPC existente e checklist automático — implementada, aguardando validação visual. Comando 2 NÃO homologado; testes extensos de autorização ficam para o próximo fechamento.

## Vitrine Pública 1.1 — Narrativa, busca e hierarquia
- [x] Vitrine Pública 1.2 — Hero limpo + Sobre Premium: implementada, aguardando validação visual do responsável; Home/Sobre verificados em 1280 e 390 px, busca ASG preservada, compilação automática OK.
- [ ] Acervo fotográfico real para páginas institucionais — só há fachada institucional adequada nesta rodada; faltam fotos reais aprovadas de trabalho, negócios e comunidade.
- [x] Vitrine Pública 1.1 implementada — Home e Sobre com narrativa empreendedor-first e busca compartilhada refinada; aguardando validação visual do responsável. Dados, ranking e administração preservados.
- [x] Sobre 2.1 — História e evolução (2016 conhecimento → 2018 difusão → 2021 igreja) implementada na página Sobre, com bloco "Da ideia impressa à experiência digital" e transição para "O que estamos construindo"; Revista permanece fora da navegação e /revista dormente; aguardando validação visual.
- [x] Sobre 2.2 — Missão, Visão, Propósito e 6 Valores (V1) implementados no /sobre com seção "Identidade institucional" e valores em composição editorial; aguardando validação editorial do responsável — não homologada até validação.
- [ ] Apresentação institucional para reunião de homens — PRÓXIMA PRIORIDADE após estabilização dos textos públicos; sem PPT nesta rodada.
- [x] Perfis Públicos Premium 1.0 — implementado, aguardando validação visual do responsável; compilação/typecheck automáticos OK, 4 testes de regras PASS, 12 resultados e buscas energia solar/ASG/casamento preservadas; perfis com/sem capa verificados em 1280/768/390 px. Galeria não exposta: is_published não distingue aprovação de imagem; nenhuma imagem cadastrada. Administração/Comando 2 e publicação intocados.
- [ ] Acervo real por perfil — 1 capa (Força Solar), 0 galerias; faltam fotos reais aprovadas para os outros 11 perfis. Onboarding futuro: exatamente 1 foto premium + até 9 adicionais (máximo 10), sem capa separada obrigatória.
- [x] Vitrine Pública — pré-homologação técnica concluída (varredura Home/Buscar/6 perfis/Sobre/404 em 390/768/1280 px, 5 buscas obrigatórias, sem overflow/erros; microcopy do rodapé e og:description do Sobre alinhados à narrativa empreendedor-first) — aguardando validação final do responsável; NÃO marcar homologada sem essa validação.
- [ ] Taxonomia Construção x Engenharia — hipótese a validar; não alterar busca ou mapeamento atual.

## Futuro — IMPORTANTE — implementar antes de escala relevante
- [ ] Saúde e Capacidade da Plataforma (Observabilidade e Capacidade)
  - Nunca uma média única: cada recurso é monitorado à parte (banco/conexões, processamento, memória quando disponível, armazenamento, volume/concorrência de buscas, tempo de resposta, taxa de erros, disponibilidade).
  - Cada recurso: valor real, limite seguro próprio, índice de pressão, estado, tendência, projeção, histórico, última medição e explicação curta.
  - Estados: Normal → Atenção → Planejamento → Ação necessária → Crítico; limiares por recurso, definidos após inspecionar a infraestrutura real.
  - Indicador da Central = resumo que reflete o gargalo mais relevante (ex.: "Saúde da Plataforma — Atenção: Banco de dados"), abrindo tela detalhada.
  - Histórico preserva intervenções/expansões (data, motivo, capacidade antes/depois), sem zerar o gráfico.
  - Coleta falha/atrasada: "Dados indisponíveis" / "Medição desatualizada"; nunca reaproveitar dado antigo como atual.
  - Assistente do Reino só interpreta dados consolidados e recomenda; não cria métricas nem executa migrações.

- Onboarding do Empreendedor 1.2 — atividade livre, oferta simplificada, catálogo em análise e tela final — implementado, aguardando homologação operacional. Assistente do Reino permanece etapa posterior.

## Rodada Domínio + Home Nacional (pendente de homologação, não publicada)
- [x] Origem canônica `https://empreendernoreino.com.br`; Home nacional; `/igreja/nazareno-mesquita` + busca local escopada; `/sobre?igreja=` com retorno whitelist; `?origem=whatsapp|instagram|telao`.
- [ ] EXTERNO: conectar domínio (DNS) e configurar Site URL/Redirect URLs de autenticação para o novo domínio antes de publicar.
```

---

# ANEXO C — AGENTS.MD VIGENTE

```markdown
<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Public profiles read published active database rows through the anonymous server whitelist; JSON is only a rollback/test fixture.
- Centralize search normalization/ranking in `src/lib/profiles.ts` so all search surfaces return the same order.
- Centralize approved assets/slogans in `profile-assets.ts`; preserve source data.
- Load premium paragraphs and service descriptions by slug only; keep listing/search payloads unchanged.
- Hide public galleries until image approval is unambiguous; never widen RLS to supply images.
- Anonymous analytics: validated server functions, random visitor/session IDs, configured retention, no fingerprinting; reset deletes browser ID and expired/withdrawn record. Launch origin is a session-only whitelisted `?origem=` in `event_properties`.
- Gallery hero is multi-image ordered by `display_order`, falling back to `cover_url`.
- Search uses needs → need_terms → profile_needs (N:N); services, offers, brands and segments stay separate to avoid taxonomic confusion.
- `needs-search.ts` stays comparison-only, reusing public matching until equivalence approval prevents ranking drift.
- Tenancy: primary network → churches → reversible church_profiles; one active church per profile, IDs/slugs preserved.
- Authorize admins only through `memberships` (user + `role_definitions` code + NETWORK/CHURCH scope) checked by `app_private` helpers in RLS; this avoids a church_id on users and lets new roles be added as data.
- Grant admin roles only by claiming an invitation for the caller's confirmed email, server-side; an open session alone must never yield a role.
- Write `audit_log` only from SECURITY DEFINER triggers/server code and block UPDATE/DELETE/TRUNCATE by trigger; append-only for app actors only (DB owners can bypass).
- Change a SUPER_ADMIN email only via step-up (password + AAL2), dual confirmation with hashed single-use expiring tokens consumed atomically, and audit of every outcome; critical admin actions should reuse this pattern.
- Roles flagged `role_definitions.requires_mfa` only count in RLS at AAL2 (`app_private.session_meets_mfa`); enable MFA for a role by data, not code.
- Pending admin invitations can only be revoked; triggers freeze identity and enforce membership/invitation NETWORK vs CHURCH scope.
- Require a reason (unlink/revoke) instead of deleting tenant/admin rows; app roles have no DELETE grant on them, preserving audit history.

- Write operational admin changes only through `public.admin_*` SECURITY DEFINER RPCs that re-check scope and audit with UI context; the context string is never an authorization input.
- Profiles carry `publication_status` (DRAFT/IN_REVIEW/PUBLISHED/CHANGES_REQUESTED/ARCHIVED) alongside `is_active`; only SUPER_ADMIN approves/archives, and the public DB rule requires active AND published.
- Admin/leadership use authenticated server functions and scoped RPCs. Context labels UI/audit only; memberships and MFA authorize Central/local actions.
- Profile publication is local: DRAFT → IN_REVIEW (shown as "validação local") → PUBLISHED via `admin_local_validate_profile`; `admin_review_profile` is legacy and unused by the UI.
- Sensitive central changes by GOVERNANCE_ADMIN go through `governance_requests` (justification, before/proposed, SUPER_ADMIN decision); only SUPER_ADMIN executes `gov_*` writes.
- `audit_log` is readable only by SUPER_ADMIN; archived profiles/churches are hidden by RESTRICTIVE policies except to SUPER_ADMIN or a valid `archive_access_grants` row. No physical deletes.
- Territory: fixed macroregions/states; curated regions/municipalities; a church's address + municipality is the classification origin and only SUPER_ADMIN changes it (trigger-enforced).
- The public Header/Footer are hidden under /admin; the admin has its own shell.

- Entrepreneur invitations have hash-only credentials and atomic verified-email claims; owner RPCs protect own drafts, never grant admin roles.
- Share ProfileWizard and onboarding-rules across admin/owners; separate writes and styles avoid duplication.
- Entrepreneur auth uses a fixed public origin and verified-session callbacks; never derive redirects from editor/request origins.

- Catalog gaps may submit without a category but retain the unresolved snapshot; publication still requires canonical validation. Legacy private images remain until an atomic 1+9 approval model exists.
- Keep free-text activity and onboarding metadata on admin saves via snapshot merge; taxonomy stays admin-side to prevent data loss.
- Admin invitation lists/details/resume preparation use scoped admin RPCs; ownStepErrors is shared with read-only progress to prevent rule drift. Resume consumes a per-invitation cooldown and audited hourly quota, never creates profiles or invitations.
- Church pages `/igreja/$church` (+`/buscar`) resolve via the `churches.ts` whitelist and scope server-side with `public_church_profile_ids`; profiles keep one `/empreendedor/$slug` URL.
```

---

# ANEXO D — ENTREPRENEUR-ONBOARDING-V1.MD VIGENTE

```markdown
# Convite do Empreendedor + Onboarding Próprio 1.0

Status: implementado, não homologado; aguarda validação visual e operacional.

## Arquitetura
- Tabela específica `entrepreneur_invitations`; não reutiliza convites administrativos.
- Segredo aleatório Web Crypto de 32 bytes (256 bits); SHA-256 armazenado; link retornado apenas na criação. Nunca registrado na auditoria.
- Prazo exato de 24h imposto pela RPC; vencimento verificado no claim, sem cron.
- Claim bloqueia a linha, exige PENDING, prazo futuro e e-mail confirmado em auth.users igual ao destinatário. Cria perfil privado DRAFT, revisão e vínculo de igreja na mesma transação.
- Continuar usa sessão autenticada, não o link consumido. RPCs do empreendedor verificam claimed_by/profile_id; não concedem memberships.
- Grants explícitos foram endurecidos após detectar privilégios padrão amplos: anon sem leitura, authenticated sem hash/contatos brutos e sem escrita direta. Funções de envio são service_role-only.
- RLS owner SELECT aditivo em perfis/revisões; nenhuma alteração nas regras públicas ou administrativas anteriores.
- Wizard único compartilhado, com funções separadas de gravação administrativa e própria. Salvar e continuar persiste de verdade; não há aviso fictício de autosave.

## Confirmação e retomada
- Consulta real a `/auth/v1/settings`: email habilitado, confirmação obrigatória, telefone desabilitado.
- Envio utiliza signInWithOtp somente para e-mail ligado ao convite, após validação/rate limit persistido: máximo 5 solicitações por convite, intervalo mínimo 60 segundos.
- Magic link retorna à página pública do convite; usuário confirma e inicia. Código opcional funciona quando presente no template hospedado.
- Retomada por `/acesso-cadastro`: envio somente para conta já vinculada e confirmada, sem criar nova conta. Usuário conectado abre `/meu-cadastro`.
- WhatsApp abre wa.me com mensagem e link para envio manual; não há SMS/WhatsApp OTP. Convite apenas telefônico pode existir, mas não permite iniciar o cadastro nesta V1: exige novo convite com e-mail.
- Entrega real de e-mail e retorno de autenticação não foram comprovados nesta rodada. Configuração habilitada não prova entrega.

## Operação
- Empreendedores contém área Convites, diálogo, link copiável exibido uma vez, cancelar e gerar novo convite (invalida anterior em transação).
- Igreja local fixa; Superadministrador seleciona alvo e RPC revalida MFA/escopo. GOVERNANCE_ADMIN não cria/cancela.
- Responsável interno separado do nome público do empreendimento; função e tipo registrados na revisão privada.
- Lacuna de necessidade pode ser descrita sem interromper envio; categorias ainda seguem catálogo existente. Assistente/catálogo automático não implementados.
- Upload privado opcional logo/capa legado: own uploader verifica proprietário, revisão editável, tamanho e assinatura de arquivo. Modelo 1+9 fica pendente.
- Submit vai a IN_REVIEW da igreja; devolução mostra motivo e permite reenvio. Publicação pela RPC local existente marca convite COMPLETED por trigger.

## Testes A–S
| Item | Resultado |
|---|---|
| A Local própria igreja | PASS transacional |
| B Local outra igreja | PASS negado |
| C Governança cria | PASS negado |
| D Superadministrador + MFA | PASS; sem MFA negado |
| E Hash sem plaintext no banco | PASS estrutura/grants e teste SHA-256 |
| F 24h | PASS valor real expires_at-created_at |
| G Expirado | PASS negado |
| H Cancelado | PASS negado |
| I Claim válido | PASS |
| J Claim repetido | PASS negado |
| K Sem acesso administrativo | Nenhuma membership concedida; navegador com empreendedor não administrativo PENDENTE |
| L Próprio rascunho | PASS RPC escrita própria e rejeição não-owner; leitura RLS com identidade não administrativa PENDENTE |
| M Igreja imutável | PASS tentativa rejeitada |
| N Fila igreja correta | PASS IN_REVIEW e church_id |
| O Devolve/corrige/reenvia | PASS transacional |
| P Zero resíduo | PASS: 0 convites, 0 igreja fixture, 12 públicos após rollback |
| Q Typecheck/compilação | PASS automática; 8 testes unitários PASS |
| R Desktop/mobile | PASS convite inválido/retomada em 1280/390, sem overflow; lista/modal/convite válido/wizard/validação logados PENDENTES por MFA |
| S Vitrine intacta | PASS diff vazio nas páginas públicas/ranking e 12 resultados na Busca |

Roteiro conservado em `supabase/tests/entrepreneur_onboarding_v1.sql`. Execução com claims sintéticos e exceção final ROLLBACK_SUCCESS, que desfez fixtures e auditorias. Não equivale a teste de e-mail real ou fluxo autenticado no navegador.

## Limites
- Nenhuma homologação operacional sem o fluxo completo real.
- Nenhum envio externo fictício, autoinscrição nova, Assistente, Declaração, Território v2 ou Banco de Talentos.
- Comando 2 não reaberto. Nada publicado.
```

---

# ANEXO E — SECURITY.MD VIGENTE

```markdown
# Segurança administrativa — estado após ETAPA 6.1

## Comprovado (suite `supabase/tests/etapa_6_1_security_attack.sql`, executada em transação desfeita)
- SUPER_ADMIN (AAL2) vê as 2 igrejas do teste e os 12 vínculos de Mesquita; em AAL1 não vê nada.
- CHURCH_ADMIN vê só a própria igreja; não edita outra, não vincula/move perfil para outra, não se promove, não cria convite SUPER_ADMIN.
- Usuário comum não cria/altera memberships, não lê/altera/apaga/trunca `audit_log`, não lê nem cria pedidos de troca de e-mail.
- Unlink sem justificativa é bloqueado (constraint); com justificativa gera 1 evento `UNLINK` com ator e motivo.
- `audit_log`: UPDATE/DELETE bloqueados por trigger inclusive no caminho do servidor.
- Códigos de troca de e-mail: só hash SHA-256 armazenado; consumo atômico de uso único; expirados rejeitados.

## Corrigido na 6.1
1. **Escalada via convite**: um CHURCH_ADMIN podia editar um convite da própria igreja e trocar `role_code` para SUPER_ADMIN (ou o e-mail). Agora campos de identidade do convite são congelados por trigger; ator do app só pode PENDING → REVOKED; política de UPDATE restringe CHURCH_ADMIN a convites CHURCH_ADMIN não-bootstrap.
2. **Coerência de escopo**: SUPER_ADMIN sempre sem igreja; papéis CHURCH sempre com igreja da mesma rede (trigger em memberships e convites).
3. **Mudança de rede**: só SUPER_ADMIN altera `churches.network_id`.
4. **MFA obrigatório para SUPER_ADMIN**: papéis com `requires_mfa` só valem no RLS em AAL2; a troca de e-mail exige AAL2 sempre; a área `/admin` força cadastro/confirmação TOTP.
5. **Corrida na confirmação**: confirmação agora é update condicional atômico (lado ainda não confirmado, pedido aberto, não expirado).

## Pendente externo
- **E-mail transacional**: nenhum domínio de envio configurado. Códigos de troca de e-mail nunca saem do servidor (não são retornados nem logados); o envio fica registrado como `PENDING` na auditoria. Falta: configurar domínio de e-mail e ligar `sendSecurityNotice` ao envio real.
- **MFA ponta a ponta**: TOTP é o mecanismo nativo do auth; não há usuários cadastrados ainda, então o cadastro real do autenticador só será validado no primeiro login do admin geral.
- **Primeiro CHURCH_ADMIN** de Mesquita: sem e-mail fornecido.
- Eventos de cadastro de MFA ocorrem no serviço de auth e não são copiados para `audit_log`.

## Limitação
`audit_log` é append-only para atores da aplicação e para o código do servidor. O dono do banco/superusuário pode desativar triggers e alterar dados; não é imutabilidade criptográfica.

## Requisitos para produção
Domínio de e-mail verificado; admin geral com MFA cadastrado; verificação de senha vazada ativada; revisão periódica da auditoria; exportação externa da auditoria se for necessária prova independente.

## Etapa 6.2a (parcial)
- Escrita administrativa só por funções `admin_*` no banco, que conferem escopo e auditam com o contexto. O contexto enviado pela interface não concede acesso (testado).
- Estas 7 funções aparecem como aviso no verificador de segurança ("usuário logado executa função privilegiada"). É intencional: cada uma confere papel e igreja internamente.
- 24 testes transacionais passaram (criação/edição restrita à igreja, envio com confirmação humana, revisão e arquivamento só pela Rede Mãe com motivo, convite só com igreja pronta/ativa, rascunhos invisíveis ao público, 12 perfis intactos).
```

---

# ANEXO F — REGISTRO MESTRE DE ARQUITETURA E DECISÕES V0.1 (02/10/2026) — TEXTO INTEGRAL RECUPERADO

> Histórico. Quando conflitar com estado atual, prevalece a hierarquia acima.

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
- Baseline: backup externo automático semanal, preferencialmente madrugada de sexta-feira.
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


---

# ANEXO G — DOSSIÊ MESTRE DE CONTINUIDADE DE 01/10/2026 — TEXTO INTEGRAL RECUPERADO

> Histórico integral incorporado para evitar perda de contexto. Quando conflitar com estado atual, prevalece a hierarquia acima.

<PARSED TEXT FOR PAGE: 1 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
EMPREENDEDORES DO REINO
Dossiê Mestre de Continuidade, Produto, Arquitetura e
Implementação
Estado consolidado em 01 de outubro de 2026
Hero institucional atual — Igreja do Nazareno de Mesquita
FINALIDADE DESTE ARQUIVO
Este documento é o handoff mestre do projeto. Ao ser anexado em outro chat, deve fornecer contexto 
suficiente para continuar o trabalho sem reconstruir decisões anteriores. O conteúdo abaixo apresenta o 
estado ATUAL: regras substituídas não devem voltar a ser usadas.
ORDEM OPERACIONAL PERMANENTE — LOVABLE
Antes de qualquer procedimento que envolva o site/plataforma, o próximo chat deve usar PRIMEIRO o 
plugin do Lovable para inspecionar o projeto real, o workspace, as alterações já existentes e o modo 
adequado de execução. O objetivo é filtrar e consolidar a instrução antes de gastar créditos no Lovable. 
Nunca mandar prompt manual ao Lovable sem antes fazer essa inspeção, salvo indisponibilidade 
comprovada do plugin.
<PARSED TEXT FOR PAGE: 2 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
1. Protocolo obrigatório ao abrir este documento em outro chat
1. Acionar imediatamente o plugin do Lovable e listar workspaces/projetos disponíveis.
2. Localizar o projeto Empreendedores do Reino / Reino Conecta. Se não aparecer, NÃO executar Build e NÃO 
improvisar prompts: orientar a reconexão do plugin à conta/workspace correto.
3. Ler o estado real do projeto pelo plugin antes de definir qualquer alteração.
4. Escolher conscientemente o modo do Lovable para cada ato: CHAT para análise curta, PLAN para 
arquitetura/escopo, BUILD somente quando a implementação estiver consolidada e autorizada.
5. Agrupar alterações relacionadas em uma única execução sempre que isso reduzir retrabalho e créditos, 
sem misturar fases incompatíveis.
6. Após cada execução relevante, usar novamente o plugin para verificar o resultado e só então decidir se 
existe correção real.
STATUS ATUAL DA CONEXÃO
Na última verificação feita antes da emissão deste documento, o plugin conectado enxergava apenas o 
workspace “Business's Lovable”, plano Free, com 1 projeto, e NÃO apresentava o projeto Reino Conecta. 
Portanto, o primeiro gate no próximo chat é confirmar/reconectar o plugin.
REGRA DE ECONOMIA DE CRÉDITOS
Pensar e auditar aqui; usar o plugin para ler o projeto; mandar ao Lovable apenas a instrução consolidada 
necessária. Evitar o ciclo: pensar aqui colar manualmente Lovable repensar voltar para nova → → →
correção, quando o plugin puder resolver a inspeção antes.
2. Visão executiva do projeto
Empreendedores do Reino é um ecossistema cristão de empreendedorismo, comunidade, desenvolvimento e 
conexão econômica. Nasceu no contexto da Igreja do Nazareno de Mesquita e evoluiu de revista/diretório para 
uma plataforma digital pesquisável, mensurável e preparada para expansão a outras igrejas evangélicas.
 Objetivo local: permitir que membros encontrem primeiro, dentro da própria comunidade, profissionais, 
serviços, produtos e empresas de confiança.
 Objetivo de desenvolvimento: fortalecer empreendedores com propósito, excelência, integridade, 
cooperação, liderança e capacitação.
 Objetivo de rede: evoluir para uma plataforma-mãe multi-igrejas, com ambientes próprios por igreja e 
inteligência central consolidada.
 Objetivo de gestão: medir alcance, adoção, buscas, perfis, contatos, satisfação, qualidade, campanhas, 
lacunas de oferta e comportamento administrativo.
 Princípio de comunicação: aparência premium, humana e editorial, com mínima “cara de IA”.
<PARSED TEXT FOR PAGE: 3 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
3. Fundamentos de propósito extraídos dos arquivos
O arquivo “Empreendedores do Reino de Deus - Empreendendo com Proposito.pdf” consolida a base conceitual
do projeto. Ele deve alimentar principalmente a página Sobre, apresentações institucionais e a narrativa do 
ecossistema. Os pilares atuais são:
 Vocação divina: empreender não apenas como negócio, mas como uso responsável de dons e habilidades.
 Mordomia fiel: gestão com sabedoria, integridade, generosidade e foco no bem comum.
 Missão no mercado de trabalho: empresas e profissões como espaços de testemunho, serviço e impacto 
positivo.
 Trabalho como ministério: fé, excelência e integridade aplicadas ao cotidiano profissional.
 Integridade nos negócios e busca constante por excelência.
 Provisão com propósito: recursos, influência e resultados também como instrumentos de apoio à obra, 
missões e comunidade.
 Cooperação em vez de concorrência destrutiva: membros se fortalecem mutuamente.
 Impacto social e comunitário: negócios que servem pessoas, famílias, igreja e sociedade.
ASSINATURA INSTITUCIONAL
“Consumir no Reino é plantar no Reino” deve continuar como uma assinatura forte do projeto, usada com 
sobriedade em blocos institucionais e materiais de comunicação.
4. Estado técnico atual da plataforma
4.1 Fase 1 — fundação de dados e persistência
A Fase 1 foi reportada como concluída e homologada, incluindo o delta corretivo da galeria. Antes de qualquer 
nova implementação, o próximo chat deve confirmar esse estado no projeto real via plugin do Lovable.
 Backend: Lovable Cloud / Supabase integrado, PostgreSQL, Auth, Storage e server functions.
 Tabelas reportadas: profiles, profile_services, profile_gallery, profile_brand_settings, app_users, user_roles, 
user_sessions, analytics_events, unmet_demands, reviews, review_moderation_logs.
 RLS ativo: perfis ativos/galeria publicada/avaliações aprovadas podem ser públicas; analytics, dados 
pessoais e moderação ficam protegidos.
 Storage: published-assets (público/CDN) e pending-uploads (privado).
 12 perfis migrados com textos editoriais completos.
 Identidade de navegação: visitor_id pseudônimo persistente; session_id por sessão; user_id somente 
quando houver identificação/autenticação consentida.
 Analytics via função controlada; leitura pública bloqueada.
 Galeria: até 10 imagens por perfil, UNIQUE(profile_id, display_order), várias imagens podem ser 
is_hero_featured=true; fallback para cover e depois fallback institucional.
 Proteções reportadas: whitelist de eventos, sanitização, limites de tamanho, integridade de profile_id e rate 
limit de 60 eventos/minuto por sessão.
 Retenção documentada do visitor_id: 365 dias, sem fingerprinting.
<PARSED TEXT FOR PAGE: 4 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
FASE 1
Status documental neste handoff: PASS DEFINITIVO, sujeito à verificação física no projeto via plugin 
Lovable antes de prosseguir.
5. Direção visual global
A linguagem visual deve ser Luxury / Premium / High-End / Editorial / Private Club / Executive / Cinematic. O 
site não deve parecer marketplace genérico, catálogo de cards repetidos ou template produzido 
automaticamente.
5.1 Paleta oficial
Token Cor
Azul Principal #06254B
Azul Escuro #03162F
Ouro Claro #E2C95C
Ouro Médio #C8A93A
Ouro Escuro #9A7A1F
Ouro Sombra #6B5312
Cinza Claro/Fundo #E2E6E9
Azul Acinzentado #8B99A6
Azul/Cinza Escuro #4C574A
5.2 Tipografia
A tipografia atual precisa deixar de parecer puramente funcional. Direção recomendada para a Fase 2: 
Cormorant Garamond (ou Bodoni Moda, se o teste visual ficar superior) para títulos/editorial + Manrope para 
interface, busca, corpo e botões. A escolha final deve ser validada no Plan do Lovable antes do Build.
5.3 Regra de imagens e marca d’água
 Usar imagens, texturas ou marcas d’água nas principais seções azuis e brancas para evitar faixas chapadas 
e excesso de “sessão/caixa/sessão”.
 Imagens institucionais devem ser fotográficas, realistas e discretas; texto, logo, dashboard, ícones e 
números NÃO devem vir “impressos” na própria imagem.
 O conteúdo textual do site entra por HTML/CSS sobre a imagem, permitindo reuso, crop, overlay e 
responsividade.
 Fotos dos perfis de empresas serão REAIS, fornecidas pelos próprios empreendedores; não gerar 10 
imagens artificiais por empresa.
 Cada perfil deve aceitar até 10 fotos reais e permitir escolher várias para o carrossel/hero.
6. Navegação e páginas
 Menu proposto: Início | Empreendedores | Liderança | Revista | Sobre.
 Rotas existentes a preservar/evoluir: /, /buscar, /empreendedor/:slug, /sobre, /revista, /admin-demo 
(evoluirá para portal administrativo real).
 Nova rota: /lideranca.
<PARSED TEXT FOR PAGE: 5 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
 Rodapé/créditos: não afirmar que o projeto foi criado pela igreja. O projeto tem idealização própria (JF 
Uchôa; confirmar grafia completa antes da publicação). A igreja é a comunidade/unidade inicial, não a 
autora automática do projeto.
6.1 Home
 Hero com foto da Igreja do Nazareno de Mesquita; overlay azul apenas via CSS, preservando a fachada e a 
bandeira brasileira.
 Busca como protagonista: “Encontre quem pode servir você dentro da nossa comunidade.”
 Composição editorial/cinematográfica, menos cards uniformes, mais respiro e assimetria controlada.
 Bloco forte “Consumir no Reino é plantar no Reino”.
 Categorias, curadoria editorial de empreendedores e seções com imagens institucionais discretas.
6.2 Página Sobre
A página Sobre não pode permanecer vazia. Ela deve contar: origem, propósito, fé aplicada ao trabalho, 
cooperação, desenvolvimento de empreendedores, fortalecimento da comunidade, como funciona e visão de 
expansão. As imagens institucionais do Pacote 01 devem ambientar os blocos.
6.3 Página Liderança
 Pr. Amadeu Aparecido Teixeira: utilizar a foto real existente na revista e o conteúdo institucional já 
extraído do arquivo.
 O arquivo “Empreendedores do Reino de Deus.pdf” apresenta o Pr. Amadeu como liderança histórica da 
Igreja do Nazareno de Mesquita, com atuação desde 1974; usar como fonte histórica/institucional.
 Pastor auxiliar identificado em pesquisa pública anterior: Pr. Alexandre Nunes Loyola. Antes de publicar 
cargo, foto ou biografia, confirmar oficialmente com a igreja.
 A página deve ser extensível a futuras lideranças sem redesenho.
6.4 Revista
STATUS DA REVISTA
A página Revista permanece CONGELADA neste momento. O PDF V0 gerado durante a conversa não foi 
aprovado pelo usuário e não deve virar autoridade editorial. O requisito funcional futuro continua: rota 
própria /revista, leitura digital responsiva, navegação/folheamento e opção de download — mas somente 
após definir a revista canônica.
7. Motor de busca — regras atuais
 Busca por profissão, serviço, produto, empresa, empreendedor, categoria, palavras-chave, aliases e 
sinônimos.
 Quanto mais específica a consulta, mais específico deve ser o resultado.
 Exemplo obrigatório: busca “material de construção” deve priorizar Farias/material de construção e NÃO 
trazer Sinergia só por conter associação ampla com “construção”.
 Busca genérica “construção” pode expandir para material de construção, empreiteira, engenharia, reforma
e arquitetura quando a relevância fizer sentido.
<PARSED TEXT FOR PAGE: 6 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
 Ordem de relevância recomendada: correspondência exata de serviço/produto/categoria frase/tag exata →
→ → parcial relevante expansão semântica apenas para consultas genéricas.
 Tags derivadas podem existir internamente, mas não devem aparecer como alegações públicas do negócio.
 Na página de resultados, após executar a busca, o input deve voltar vazio com placeholder “O que você 
precisa hoje?”, enquanto o contexto da consulta pode aparecer fora do campo como “Resultados para...”.
7.1 Busca sem resultado / Demanda Não Atendida
Mensagem-base
Ainda não encontramos esse serviço em nossa rede. Irmão, fique tranquilo. Esse serviço ainda não está 
disponível em nosso diretório, mas vamos verificar junto à nossa comunidade quem pode atender essa 
necessidade e convidar esse profissional para fazer parte do projeto. Assim, buscamos ajudar você a 
encontrar um bom serviço e, ao mesmo tempo, fortalecer e abençoar alguém da nossa comunidade.
 Botão: “Quero ser avisado quando encontrarem”.
 Internamente: registrar Demanda Não Atendida, termo buscado, igreja, sessão e contato somente se 
fornecido voluntariamente.
8. Arquitetura dos perfis
 Perfil não deve parecer ficha cadastral; deve ser editorial/premium.
 Hero institucional azul com logo maior, tagline, cover/galeria em rotação e CTA elegante.
 Logo, cover e gallery são entidades distintas.
 Até 10 fotos reais por perfil; ordenação; alt text; remoção/substituição; várias fotos podem alimentar o 
hero.
 Textos integrais da revista devem ser preservados, não trocados por resumos genéricos.
 CTA WhatsApp, Instagram, telefone/site quando existir, e futuro botão “Quero receber novidades deste 
empreendedor”.
 As imagens reais de serviços serão anexadas futuramente por empreendedor e colocadas nos locais 
corretos; não gerar banco artificial por empresa.
9. Base atual de 12 perfis — dados editoriais vigentes
ATENÇÃO
Os textos abaixo vêm das fontes comerciais existentes. Alegações numéricas, percentuais, taxas, condições e
promessas comerciais devem ser revalidadas antes da publicação definitiva quando puderem ter mudado. 
A regra é preservar o texto editorial sem transformar informação histórica em condição comercial vigente.
Força Solar do Brasil
Categoria Energia Solar
Tagline Reduza sua conta de luz em até 95% e valorize seu 
<PARSED TEXT FOR PAGE: 7 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
imóvel investindo em energia limpa e renovável!
WhatsApp/Telefone 21 96520-9171
Instagram forcasolardobrasil
Nossa empresa de energia solar oferece projetos personalizados, equipamentos de alta performance e 
instalação profissional para garantir o máximo rendimento. Além de economizar todos os meses, você 
contribui para um futuro mais sustentável e livre da instabilidade das tarifas de energia.
Com garantia, suporte técnico e financiamento facilitado, o retorno do investimento é rápido e seguro. Não 
perca tempo pagando mais caro pela eletricidade.
Transforme o sol em economia e liberdade. Fale com nossos especialistas e comece hoje mesmo a gerar sua 
própria energia!
Xavier Imóveis
Categoria Corretor de Imóveis
Tagline O imóvel dos seus sonhos já existe... e ele pode ser seu
antes que alguém leve!
WhatsApp/Telefone 21 98431-4779
Instagram xavierimoveisrj
Imagine abrir a porta e sentir: "Eu consegui!". Imagine investir hoje e ver seu patrimônio crescer todos os dias.
Comigo, você não procura às cegas — você tem acesso VIP às melhores oportunidades, negociações que 
favorecem você e segurança total em cada etapa.
Nada de riscos, nada de perder tempo... apenas resultados rápidos e certeiros.
Comprar, vender ou investir? Eu vou caçar a opção perfeita para o seu perfil e garantir que você saia no lucro.
Mas atenção: o imóvel certo não espera. Outro comprador pode estar a um telefonema de distância.
Me chame agora e vamos transformar seu sonho ou investimento em realidade antes que seja tarde.
Consultor Ambiental
Categoria Consultoria Ambiental
Tagline Proteger o solo é proteger o futuro do seu negócio.
WhatsApp/Telefone 21 97213-4461
Instagram —
<PARSED TEXT FOR PAGE: 8 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Nota atualizada
O serviço é voltado especialmente a postos de gasolina e empresas de ônibus. A apresentação pública deve 
refletir esses dois contextos, sem inventar serviços técnicos específicos ainda não confirmados.
Como consultor ambiental especializado, eu ajudo você a prevenir riscos, manter seu posto em conformidade 
legal e operar de forma sustentável, preservando o solo e a imagem da sua empresa.
Minhas soluções não são genéricas — são estratégias personalizadas para garantir que sua operação seja 
segura, limpa e lucrativa, evitando passivos ambientais que podem custar o seu negócio.
No setor de postos de combustíveis, cada detalhe conta: um vazamento ou manejo inadequado pode gerar 
multas altíssimas, danos irreversíveis ao meio ambiente e perda de credibilidade.
Cuidar do solo é agir agora. Entre em contato e descubra como blindar seu posto contra problemas ambientais 
antes que eles aconteçam.
Escopo atualizado
Escopo vigente: consultoria ambiental voltada a postos de gasolina e empresas de ônibus. Preservar o texto 
histórico sobre postos e ampliar a contextualização para empresas de ônibus sem criar alegações não 
fornecidas.
Força Tarefa Segurança Privada
Categoria Segurança Privada
Tagline Proteja o que mais importa com quem entende do 
assunto.
WhatsApp/Telefone 21 96593-0473
Instagram —
Segurança não é custo — é o escudo que protege tudo o que você ama.
Quando o perigo bate à porta, segundos decidem entre a tranquilidade e o caos. Ter um profissional altamente 
treinado no seu condomínio é ter resposta imediata, prevenção de riscos e proteção 24h para famílias, clientes 
e patrimônio.
Seja em condomínios residenciais ou comerciais, nossa equipe combina tecnologia avançada com presença 
humana estratégica, garantindo um ambiente seguro, controlado e livre de ameaças.
Cada profissional é preparado para agir com precisão, postura impecável e atenção constante — porque 
segurança não se improvisa.
<PARSED TEXT FOR PAGE: 9 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Não espere que o perigo seja notícia. Entre em contato agora e descubra como blindar seu condomínio antes 
que o risco chegue ao portão.
Farias Construções
Categoria Material de Construção
Tagline Sua obra começa aqui!
WhatsApp/Telefone 21 99080-5240
Instagram farias.const
Chamada secundária Qualidade, variedade e melhor atendimento!
Construir ou reformar exige mais do que força de vontade — exige materiais de confiança, bons preços e um 
atendimento de qualidade. É exatamente isso que você encontra na nossa loja de material de construção!
Dos alicerces ao acabamento, oferecemos tudo em um só lugar: cimento, areia, tijolos, pisos, tintas, 
ferramentas, hidráulica, elétrica e muito mais. Trabalhamos com as melhores marcas do mercado, garantindo 
durabilidade, economia e segurança em cada etapa da sua obra.
Seja você um pedreiro experiente, arquiteto ou dono de casa reformando aos poucos, nossa equipe está pronta 
para te ajudar a fazer a melhor escolha dos materiais para a sua obra — com orientação técnica, entrega 
rápida e condições especiais.
FT Portaria
Categoria Terceirização de Serviços
Tagline Seu condomínio merece mais do que gestão. Merece 
excelência.
WhatsApp/Telefone 21 96593-0473
Instagram —
Imagine entrar em um ambiente sempre limpo, organizado, seguro e funcional, onde cada detalhe reflete 
cuidado e profissionalismo.
É isso que oferecemos: facilities de alta performance que transformam condomínios residenciais e espaços 
comerciais em lugares onde viver e trabalhar é um prazer.
Nossa equipe vai muito além do básico — antecipamos problemas, cuidamos de cada detalhe e garantimos 
eficiência, para que você tenha tranquilidade total e valorização do patrimônio.
Com serviços planejados e executados com precisão, cada canto do seu condomínio transmite conforto, 
segurança e bem-estar para moradores, clientes e colaboradores.
<PARSED TEXT FOR PAGE: 10 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Não espere que pequenos problemas se tornem grandes dores de cabeça. Fale conosco hoje e descubra como 
transformar seu condomínio em um espaço impecável, seguro e valorizado, sem esforço e sem preocupações.
Sinergia
Categoria Engenharia e Arquitetura
Tagline Transforme seu projeto em realidade com excelência 
e segurança!
WhatsApp/Telefone 21 3273-7362
Instagram br.sinergia
Na construção e reforma, cada detalhe importa — e é exatamente aí que a experiência de um Engenheiro Civil 
faz toda a diferença. Com visão estratégica, conhecimento técnico e compromisso absoluto com a qualidade, 
transformamos ideias em obras sólidas, modernas e esteticamente impecáveis.
Do planejamento à entrega, garantimos execução precisa, dentro do prazo e com o máximo aproveitamento de 
recursos, evitando desperdícios e surpresas no orçamento. Seja para construir do zero, revitalizar um espaço 
ou ampliar sua estrutura, nosso trabalho é guiado por inovação, segurança e beleza arquitetônica.
Sua obra merece mais que um executor: merece um profissional que compreenda sua visão e a eleve a um 
novo patamar, sua obra merece a SINERGIA. Construa com quem entende, realize com quem se importa.
Higiene, Limpeza e Descartáveis
Categoria Higiene, Limpeza e Descartáveis
Tagline Mais que produtos, entregamos confiança e cuidado 
em cada detalhe.
WhatsApp/Telefone 21 96593-0473
Instagram —
Chamada secundária Sua limpeza, nossa missão. Sua tranquilidade, nossa 
prioridade.
Na rotina acelerada da sua igreja, empresa ou comércio, limpeza e higiene não podem esperar — e é por isso 
que somos o parceiro que garante qualidade, agilidade e o melhor custo-benefício, sempre no momento certo.
Fornecemos materiais de limpeza, higiene e descartáveis que unem potência e economia, deixando seus 
ambientes sempre prontos, seguros e impecáveis para receber clientes, membros e visitantes e cuidar da sua 
equipe.
Aqui, atraso não existe: entregamos com pontualidade para que você nunca pare por falta de suprimentos.
Aqui, você não é mais um: criamos soluções sob medida para manter sua operação sempre no mais alto 
padrão.
<PARSED TEXT FOR PAGE: 11 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Aqui, o cuidado é contínuo: você recebe mais do que produtos, recebe tranquilidade todos os dias.
Henrique — Reforço Escolar
Categoria Reforço Escolar
Tagline Aula particular on-line de Matemática e Física, com 
foco individual e aprendizado no seu ritmo.
WhatsApp/Telefone 21 99682-1985
Instagram —
Imagine poder aprender no seu ritmo, com total foco em você, sem distrações e com alguém preparado para 
transformar cada dúvida em conhecimento sólido. É exatamente isso que as aulas particulares oferecem: um 
atalho poderoso entre onde você está e onde deseja chegar.
Enquanto muitos lutam para acompanhar turmas cheias e métodos genéricos, quem investe em aulas 
particulares conquista velocidade, clareza e resultados reais. Cada minuto de estudo se torna estratégico, cada 
explicação é feita sob medida e cada avanço é percebido de imediato.
Não se trata apenas de aprender mais rápido, mas de conquistar confiança, superar bloqueios e abrir portas 
para oportunidades que só quem domina de verdade pode alcançar.
Pergunte-se: quanto vale ter alguém 100% focado em você, guiando cada passo rumo ao seu sucesso? A 
resposta é clara: aulas particulares não são um gasto, são um investimento inteligente no seu futuro. O 
próximo passo é seu: escolha acelerar sua jornada de aprendizado agora.
Refrigera Tec
Categoria Refrigeração e Ar-Condicionado
Tagline Respire tranquilidade. Viva o conforto. Confie em 
quem entende de climatização.
WhatsApp/Telefone 21 97968-6874
Instagram —
Você já parou para pensar em quanto o seu bem-estar, a produtividade da sua equipe e até a saúde da sua 
família dependem do bom funcionamento do ar-condicionado?
Um ar mal cuidado pode esconder inimigos invisíveis: fungos, bactérias, poeira e impurezas que circulam 
silenciosamente, prejudicando a qualidade do ar e aumentando riscos de doenças respiratórias. Além disso, a 
falta de manutenção pode elevar o consumo de energia e gerar custos inesperados com reparos caros.
É por isso que a Refrigera Tec existe: para trazer segurança, economia e qualidade de vida através de soluções 
inteligentes em manutenção de ar condicionado e projetos de refrigeração sob medida.
<PARSED TEXT FOR PAGE: 12 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Não espere o problema aparecer! Quem faz manutenção se antecipa, economiza e vive tranquilo. Agende agora
uma visita da Refrigera Tec e descubra como transformar seu ambiente em um espaço de bem-estar e 
eficiência. Seu conforto não pode esperar. Entre em contato hoje mesmo!
Cordas de Amor Cerimônias
Categoria Cerimônias e Celebrações
Tagline Onde Cada Detalhe Ecoa Amor.
WhatsApp/Telefone (21) 99052-6210
Instagram @cdacerimonias — 
https://www.instagram.com/cdacerimonias
Nota atualizada
Contato atualizado pelo usuário. Substituir integralmente o telefone antigo e qualquer Instagram anterior 
em banco, perfil, botões e futuras campanhas.
Na Cordas de Amor Cerimônias, acreditamos que cada celebração é muito mais do que um evento: é uma 
verdadeira sinfonia de emoções. Nosso maior propósito é transformar o seu sonho em uma experiência real, 
única e inesquecível.
Cada cerimônia é planejada com delicadeza, carregada de beleza, significado e amor em cada detalhe. Do 
primeiro olhar ao último acorde, tudo é pensado para refletir a essência da sua história.
Trabalhamos com sensibilidade, carinho e dedicação, porque sabemos que momentos assim não se repetem. 
Cada elemento ganha vida para criar memórias que serão guardadas para sempre no coração.
Mais do que organizar, nós celebramos junto com você cada conquista e cada emoção. Com charme, 
sofisticação e autenticidade, damos forma ao que antes existia apenas no imaginário. O cenário, as flores, os 
sons e as palavras se unem em perfeita harmonia. E assim, sua história é eternizada de forma única, especial e 
eternamente lembrada.
Maquininha de Cartão — Ton
Categoria Maquininha de Cartão
Tagline Leve suas vendas a outro nível!
WhatsApp/Telefone 21 99682-1985
Instagram —
Quer pagar menos taxa no seu negócio? Com o plano Ton Pro é possível!
<PARSED TEXT FOR PAGE: 13 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Você já tem maquininha de cartão? Ótimo! Mas será que ela realmente é a melhor para o seu negócio? Muitos 
empreendedores continuam com taxas altas, atrasos nos repasses e recursos limitados sem perceber que estão 
deixando dinheiro na mesa.
Seja para quem ainda não tem ou para quem já usa, a verdade é clara: a escolha da maquininha certa faz toda 
a diferença. Uma máquina moderna, com taxas justas e repasse rápido, não só aumenta seu faturamento como 
também traz credibilidade, agilidade e confiança aos seus clientes.
Pense nisso: cada compra que você facilita no cartão é uma oportunidade de fidelizar clientes e vender mais. 
Agora, imagine fazer isso com mais economia, mais tecnologia e mais vantagens. Se você ainda não tem, está 
perdendo vendas. Se você já tem, mas não a melhor, está perdendo lucro. Não aceite menos do que seu negócio
merece. Troque por uma maquininha que realmente impulsiona seus resultados e leve sua empresa a outro 
nível.
Regra de publicação
Percentuais, taxas, promoções e condições comerciais da revista antiga não devem ser reutilizados sem 
validação atual.
10. Assets de marca aprovados / em uso
Força Solar do Brasil — logo oficial
Usar como logo do perfil/card. Não substituir pela arte promocional.
<PARSED TEXT FOR PAGE: 14 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Força Solar do Brasil — cover promocional
Usar como cover/hero promocional, separado da logo.
FT Portaria
Asset premium aprovado.
Força Tarefa Segurança Privada
Asset premium final aprovado.
<PARSED TEXT FOR PAGE: 15 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Ton / Maquininha
Visual aprovado para identificação/promoção do perfil.
Xavier Imóveis
Versão refinada aprovada.
Farias Construções
Preserva mascote/conceito já usado em materiais reais.
<PARSED TEXT FOR PAGE: 16 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Cordas de Amor Cerimônias
Asset premium aprovado.
Refrigera Tec
Asset premium aprovado.
Higiene, Limpeza e Descartáveis
Asset premium aprovado.
<PARSED TEXT FOR PAGE: 17 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Consultor Ambiental
Asset atualizado para dialogar com postos e empresas de ônibus.
ASSETS AINDA PENDENTES
Sinergia Engenharia e Arquitetura e Reforço Escolar Henrique ainda precisam de asset premium definitivo.
O schema já deve aceitar substituição posterior sem refazer layout.
11. PACOTE 01 — Imagens Estratégicas Base
REGRA MÃE
Estas imagens são matéria-prima visual do site: sem texto, sem logo, sem números, sem dashboards, sem UI.
Servem como hero, fundo, marca d’água ou apoio editorial. Texto e interface são sobrepostos no site via 
CSS/HTML.
<PARSED TEXT FOR PAGE: 18 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Imagem 1 — Hero institucional do Sobre
Topo da página Sobre. Reunião executiva premium; transmite liderança, visão, propósito e empreendedorismo.
Imagem 2 — Reunião executiva / mentoria
STATUS
PENDENTE DE REFAZER no padrão puro/fotográfico. A versão anterior continha informação gráfica e não 
deve ser usada.
Imagem 3 — Networking entre empresários
Sobre, blocos de conexão/networking e marcas d’água em seções institucionais.
<PARSED TEXT FOR PAGE: 19 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Imagem 4 — Comunhão com propósito
Valores, comunidade, propósito e integração entre fé, relacionamento e desenvolvimento.
Imagem 5 — Planejamento e estratégia
Seções de método, planejamento, organização, crescimento e estratégia.
<PARSED TEXT FOR PAGE: 20 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Imagem 6 — Empreendedor atendendo cliente
Resultados, institucional e blocos sobre excelência de atendimento/serviço.
Imagem 7 — Empresários em roda de conversa
Sobre, encontros, troca de experiências, mentoria e inteligência coletiva.
<PARSED TEXT FOR PAGE: 21 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Imagem 8 — Liderança e direção
Liderança, direcionamento, governança e desenvolvimento de equipe.
Imagem 9 — Fé + empreendedorismo (versão evangélica)
Blocos que conectam fé evangélica, propósito e atuação profissional; usar com discrição.
<PARSED TEXT FOR PAGE: 22 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Imagem 10 — Fundo editorial premium (contexto local)
Marca d’água/fundo editorial neutro e sofisticado, adequado a seções brancas/azuis com overlay.
11.1 Imagens criadas que NÃO devem ser usadas como PACOTE 01
 wide_clean_infographic_website_style_banner_in_po.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 a_wide_polished_infographic_ux_presentation_image.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 a_clean_professional_infographic_dashboard_promot.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 a_clean_modern_infographic_marketing_slide_in_por.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 wide_warm_modern_promotional_banner_scene_for_a.png — geração intermediária/supersedida; não 
usar como imagem-base institucional.
 wide_high_quality_warm_and_modern_promotional_we.png — geração intermediária/supersedida; não 
usar como imagem-base institucional.
 wide_professional_warmly_lit_promotional_scene_w.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 a_wide_polished_promotional_banner_advertisement.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 wide_promotional_banner_hero_image_for_a_platform.png — geração intermediária/supersedida; não 
usar como imagem-base institucional.
 a_warm_cinematic_shallow_depth_of_field_golden.png — geração intermediária/supersedida; não usar 
como imagem-base institucional.
 terraço_curvo_sobre_montanhas_e_mar.png — geração intermediária/supersedida; não usar como 
imagem-base institucional.
 reunião_profissional_ao_entardecer.png — geração intermediária/supersedida; não usar como imagem￾base institucional.
<PARSED TEXT FOR PAGE: 23 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
12. Evolução estrutural: plataforma-mãe multi-igrejas
A expansão para outras igrejas é uma mudança estrutural prioritária. O projeto deve evoluir de um site de 
uma igreja para uma plataforma multi-tenant/white-label controlada, com uma base-mãe e unidades por 
igreja.
 Hierarquia de domínio: Rede Igreja Empreendedor Serviços/Produtos Eventos/Métricas. → → → →
 Cada igreja terá fachada, liderança, textos, fotos, empreendedores e conteúdo próprios, sem duplicar o 
código do sistema.
 Padrão de apresentação por unidade: “Empreendedores do Reino de Deus — [nome da igreja/local]” ou 
equivalente aprovado; o núcleo da marca permanece e a identificação local muda.
 Fachada da igreja, pastor/pastor auxiliar e parte das fotos institucionais devem ser locais. Algumas 
imagens-base podem ser compartilhadas, mas cada igreja precisa de identidade visual suficiente para não 
parecer uma cópia literal.
 Cada igreja poderá ter personalização visual controlada sem romper a identidade-mãe.
 O Super Admin enxerga toda a rede; cada igreja possui visão isolada de seus próprios dados.
 Busca futura pode oferecer “Buscar nesta igreja” e “Buscar em toda a Rede Empreendedores do Reino”.
 Comparador entre igrejas: identificar serviços existentes em uma e ausentes em outra.
 Matriz de oferta por igreja: categoria/serviço × igreja, permitindo perguntas como “o que Mesquita tem e a 
Batista não tem?”.
 Campo de inteligência pode permitir perguntas em linguagem natural, mas deve responder somente com 
dados reais do banco.
 Criar taxonomia central de serviços/produtos para comparação consistente entre igrejas.
12.1 Campos/entidades que a arquitetura deverá introduzir
 network_id
 church_id / tenant_id
 churches
 church_brand_settings
 church_leadership
 church_admins / memberships
 service_taxonomy
 church_service_availability
 campaigns
 subscribers
 audit_logs
 estimated_member_base
13. Analytics, telemetria e funis
A plataforma deve medir o máximo que seja útil, proporcional e ético. Cada evento deve poder ser filtrado por 
rede, igreja, perfil, período, sessão, visitante e campanha.
Aquisição
 session_started
 landing_view
 source/medium/campaign/UTM
<PARSED TEXT FOR PAGE: 24 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
 QR source
 device class
 browser
 referrer
Busca
 search_started
 search_submitted
 search_term
 search_results_count
 search_zero_results
 suggestion_clicked
 category_clicked
Resultados
 result_impression
 result_clicked
 position_in_results
Perfil
 profile_view
 profile_unique_view
 profile_time
 profile_scroll_depth
 gallery_open
 gallery_image_view
 gallery_next
 gallery_prev
 service_section_view
 contact_cta_view
Contato/Compartilhamento
 whatsapp_click (qual perfil/qual contato/origem)
 instagram_click
 phone_click
 website_click
 profile_link_copy
 profile_share_click
Demanda
 unmet_demand_view
 unmet_demand_interest
 requested_service_term
Avaliações
 review_request_view
 review_started
 review_submitted
<PARSED TEXT FOR PAGE: 25 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
 rating_value
 feedback_type
Satisfação da plataforma
 satisfaction_survey_started
 satisfaction_survey_submitted
Retenção
 returning_session
 sessions_per_user
 active_days
 last_seen
Campanhas
 campaign_sent
 campaign_delivered
 campaign_opened
 campaign_clicked
 campaign_returned_to_platform
INTERPRETAÇÃO CORRETA
Clique no WhatsApp mede intenção de contato, não prova que a mensagem foi enviada nem que houve 
contratação. Relatórios devem nomear corretamente cada etapa.
14. Dashboards e relatórios
 Dashboard Central da Rede: todas as igrejas, comparações, crescimento, cobertura de serviços, campanhas,
qualidade e administração.
 Dashboard por Igreja: ao selecionar uma igreja, apresentar SOMENTE os dados daquela unidade.
 Dashboard por Empreendedor: impressões, visualizações, termos que levaram ao perfil, tempo, galeria, 
WhatsApp, Instagram, avaliações, evolução.
 Funil: entrada busca resultado perfil contato avaliação. → → → → →
 Relatório mensal por igreja: alcance, usuários únicos, sessões, pesquisas, perfis, contatos, serviços mais 
buscados, serviços ausentes, recorrência e evolução.
 Relatório de adoção: estimated_member_base versus visitantes únicos, sempre rotulado como indicador 
aproximado, não como prova de que todo visitante é membro.
 Relatório de campanha/divulgação: culto, QR Code, revista, WhatsApp, Instagram, evento; medir 
antes/depois.
 Relatório de lacunas: serviços buscados e não encontrados, além de comparação com outras igrejas que já 
possuem aquela oferta.
 Relatórios devem ser modernos, bonitos, realistas, exportáveis e conter “Leituras do período” baseadas em 
dados, sem diagnóstico inventado.
<PARSED TEXT FOR PAGE: 26 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
14.1 Exemplo de leitura gerencial
Se uma igreja informa base estimada de 1.000 membros e registra apenas 10 visitantes únicos no mês, o 
sistema não deve afirmar automaticamente “faltou divulgação”. Deve mostrar o alcance aproximado (1%) e 
sinalizar baixa adoção/alcance como hipótese, cruzando com campanhas, QR Codes, recorrência e outras 
evidências.
15. Pesquisa de satisfação e avaliação dos serviços
 Três alvos: Serviço/Profissional, Plataforma/Site e Revista.
 Nas reuniões, incentivar de forma clara o preenchimento da pesquisa de satisfação; não bloquear o uso da 
plataforma para obrigar resposta.
 Avaliação de serviço deve começar confirmando se a pessoa realmente utilizou/contratou o serviço.
 Critérios possíveis: atendimento, qualidade, cumprimento do combinado, comunicação, resolução de 
problemas, nota geral e comentário.
 Pergunta específica quando houver problema: avaliar atenção dada e busca de solução. Princípio: 
problema pode acontecer; o tratamento e a resolução importam.
 Comentários públicos devem passar por moderação; preservar identificação interna para reduzir abuso.
 Permitir resposta do empreendedor em fluxo futuro.
 Não criar ranking humilhante. Usar os dados para qualidade, melhoria e confiança.
16. Cadastro para novidades e CRM por igreja
 Criar convite elegante (modal/bottom sheet ou seção contextual) para receber novidades da igreja.
 Campos: nome, telefone/WhatsApp e e-mail.
 Validação obrigatória de formato, DDD, e-mail, limites e sanitização.
 Confirmação visual dos dados antes de concluir.
 Proteção antispam/humano por mecanismo adequado (ex.: Turnstile/CAPTCHA) sem depender apenas de 
uma checkbox simbólica.
 Consentimento explícito para receber comunicações; guardar origem, data e canais aceitos.
 Cadastro pertence à igreja em que a pessoa estava navegando, com possibilidade de visão central 
consolidada.
 Preferências futuras: promoções, novos serviços/produtos, eventos, capacitações, novidades de perfis 
seguidos.
 Descadastro simples e rastreável.
17. Motor de campanhas e automação de relacionamento
 Quando houver atualização relevante de perfil — promoção, novo serviço, novo produto ou novidade — 
permitir marcar como “Divulgar para a comunidade”.
 Campanhas de empreendedores devem, pelo menos inicialmente, passar por aprovação do administrador 
da igreja/rede antes do disparo.
 Audiência pode incluir assinantes da igreja, pessoas que visualizaram o perfil/categoria e seguidores do 
empreendedor, sempre dentro de consentimento válido.
 Evitar “qualquer movimento = e-mail”. Definir relevância, frequência, deduplicação e, quando fizer 
sentido, resumo semanal.
<PARSED TEXT FOR PAGE: 27 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
 Envio via backend por provedor de e-mail (ex.: Resend/Postmark ou equivalente), parecendo sair da 
própria plataforma.
 Medir enviado entregue aberto clicado retorno à plataforma perfil WhatsApp. → → → → → →
 Possível função futura: “Quero receber novidades deste empreendedor”.
18. Governança, administração local e auditoria central
Papel Escopo
SUPER_ADMIN Visão e controle de toda a rede, todas as igrejas, 
auditoria e configurações centrais.
CHURCH_ADMIN Gerencia empreendedores, conteúdo, campanhas, 
cadastros, avaliações e relatórios da própria igreja.
CHURCH_MODERATOR Moderação de conteúdo, avaliações e cadastros 
dentro do escopo local.
ENTREPRENEUR Gerencia somente o próprio perfil, serviços, 
produtos, fotos e novidades permitidas.
VIEWER / LEADERSHIP Pastor/liderança pode ver relatórios e métricas sem 
alterar dados.
 Administrador local pode desativar/arquivar/cancelar dentro da igreja, mas não apagar o histórico central 
de auditoria.
 Preferir soft delete/status (ACTIVE, INACTIVE, ARCHIVED, SUSPENDED, DELETED_SOFT) a hard delete.
 Audit log central deve registrar ação, usuário/admin, igreja, objeto, estado anterior, estado novo, data/hora 
e motivo quando aplicável.
 Registrar login, logout, sessão, tempo ativo razoavelmente calculado, última ação, alterações, campanhas, 
moderação, relatórios/exportações — sem registrar teclas ou atividade fora da plataforma.
 Dashboard central deve permitir acompanhar atividade e pendências de cada administrador local.
19. Segurança, privacidade e LGPD — requisitos de produto
 Minimização de dados e transparência sobre finalidades.
 Separação entre visitante anônimo/pseudônimo e usuário identificado.
 Nunca usar fingerprinting oculto para descobrir identidade.
 Consentimento quando necessário para comunicações e vinculação de comportamento a cadastro.
 Política de retenção e mecanismos de exclusão/desvinculação quando aplicável.
 RLS e segregação por church_id/tenant_id.
 Audit log protegido; service role nunca exposta no frontend.
 Uploads pendentes privados; assets publicados entregues via CDN.
 Rate limiting e validação de payload em endpoints de telemetria e formulários públicos.
20. Arquivos/fontes incorporados ao entendimento do projeto
Arquivo Papel atual
Empreendedores do Reino de Deus - Empreendendo 
com Proposito.pdf
Fonte conceitual de fé, propósito, vocação, 
mordomia, trabalho como ministério, integridade, 
provisão, cooperação e impacto.
Empreendedores-do-Reino-de-Deus.zip e páginas 1–
10 extraídas
Fonte editorial/comercial da revista que originou a 
base real dos 12 perfis e seus textos.
<PARSED TEXT FOR PAGE: 28 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
Empreendedores do Reino de Deus.pdf (7 páginas) Referência histórica/complementar: capa Vol. 01 de 
18/08/2025, página do Pr. Amadeu e versões de 
perfis. O sumário contém placeholders genéricos; 
não usar esses placeholders. Não é autoridade única 
da revista atual.
conteudo_editorial_perfis.json Base estruturada com 12 perfis e textos editoriais; 
aplicar as atualizações deste dossiê, especialmente 
Cordas de Amor e Consultor Ambiental.
manifest_assets.json Manifesto de assets aprovado à época; este dossiê 
prevalece para assets/decisões atualizadas.
Vídeos de tela de 29/09, 30/09 e 01/10 Evidenciaram problemas de UX: visual básico, busca 
ampla demais, input de busca mantendo termo, 
Sobre pobre, Revista com navegação incorreta e 
seções sem riqueza visual.
Revista_Empreendedores_do_Reino_V0.pdf Artefato criado durante a conversa e posteriormente 
rejeitado como solução adequada para a Revista. Não
usar como revista canônica.
BRIEF_VISUAL_UX_V0.md / prompts e pacotes 
Lovable anteriores
Histórico de prototipação. Quando houver conflito, 
prevalece este dossiê e o estado real lido via plugin 
Lovable.
20.1 Hierarquia de autoridade
 1º — Atualizações explícitas do usuário registradas neste dossiê.
 2º — Estado técnico real do projeto, verificado via plugin do Lovable.
 3º — Arquivos canônicos de conteúdo/brand atualmente aprovados.
 4º — Revistas e materiais históricos como fonte complementar.
 5º — Pacotes/prompts antigos apenas como histórico; não reintroduzir regra supersedida.
21. Inventário consolidado de correções para a próxima 
evolução
 Precisão da busca específica (“material de construção” não deve trazer Sinergia por associação ampla).
 Input de busca deve limpar após a consulta na página de resultados.
 Cordas de Amor: atualizar WhatsApp para (21) 99052-6210 e Instagram para @cdacerimonias / 
instagram.com/cdacerimonias.
 Marcas d’água/imagens discretas nas principais seções azuis e brancas.
 Página Sobre completa com narrativa e imagens institucionais.
 Criar menu/página Liderança.
 Preparar plataforma multi-igrejas antes de avançar demais no redesign.
 Dashboards/relatórios central, por igreja e por empreendedor.
 Pesquisa de satisfação e avaliação do serviço.
 CRM/cadastro de novidades por igreja.
 Motor de campanhas e automações.
 Administrador local por igreja com auditoria central imutável.
 Galeria real por perfil: até 10 fotos reais, sem geração artificial por negócio.
 Revista continua congelada até definir fonte editorial canônica.
<PARSED TEXT FOR PAGE: 29 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
22. PRÓXIMO PASSO OBRIGATÓRIO — antes da Fase 2 visual
POR QUE NÃO IR DIRETO PARA A FASE 2
Depois da homologação da Fase 1, surgiu uma decisão estrutural maior: a plataforma será multi-igrejas, 
com administração local, dashboards segmentados, campanhas, CRM e auditoria central. Isso afeta o 
modelo de dados e permissões. Portanto, o próximo passo é um Gate Arquitetural Multi-Igrejas / Pré-Fase 2, 
e não um redesign isolado.
22.1 Procedimento automático no novo chat
7. Usar o plugin Lovable imediatamente.
8. Listar workspaces/projetos e localizar Reino Conecta.
9. Se não localizar, parar e orientar a reconexão da conta/workspace correto. Não gastar crédito em prompts 
manuais.
10. Quando localizar, inspecionar schema, migrations, rotas, estado da Fase 1 e créditos/capacidade 
disponíveis.
11. Usar PLAN (ou CHAT/PLAN equivalente) para pedir um plano de delta arquitetural multi-tenant. NÃO usar 
BUILD nessa primeira mensagem.
12. Validar o plano aqui. Só depois consolidar um único BUILD para a adaptação estrutural necessária.
13. Somente após PASS estrutural abrir a Fase 2 visual premium.
22.2 Instrução-base a enviar ao Lovable via plugin — MODO PLAN
GATE ARQUITETURAL MULTI-IGREJAS / PRÉ-FASE 2 — EMPREENDEDORES DO REINO
NÃO EXECUTAR BUILD. Inspecione o estado real do projeto Reino Conecta, incluindo
a Fase 1 já implementada. Proponha o delta mínimo e seguro para evoluir de uma 
única igreja para uma plataforma-mãe multi-tenant, preservando os 12 perfis e o 
frontend atual.
O plano deve cobrir: networks/churches; church_id/tenant_id em dados e eventos; 
segregação RLS; papéis SUPER_ADMIN, CHURCH_ADMIN, CHURCH_MODERATOR, 
ENTREPRENEUR e VIEWER/LEADERSHIP; auditoria central imutável/soft delete; 
liderança por igreja; taxonomia central de serviços/produtos; comparação de 
oferta entre igrejas; estimated_member_base; dashboard central e por igreja; 
relatórios; CRM/subscribers por igreja; consentimentos; campanhas e tracking; 
avaliações/satisfação; busca local vs rede; compatibilidade com o schema existente 
e migração dos 12 perfis atuais para a igreja da Nazarena de Mesquita.
Também incorpore as correções funcionais já aprovadas: precisão da busca 
específica; limpar input após pesquisa; dados atualizados de Cordas de Amor; 
escopo do Consultor Ambiental; preparação para galerias reais de até 10 fotos; 
página Liderança; página Sobre; Revista permanece congelada.
Entregue somente: diagnóstico do estado atual, delta de schema/RLS, estratégia de 
<PARSED TEXT FOR PAGE: 30 / 30>
Empreendedores do Reino — Dossiê Mestre de Continuidade — 01/10/2026
migração sem perda, impacto no frontend, ordem de implementação, riscos, testes, 
estimativa de créditos/mensagens e decisões realmente pendentes. Termine com 
PRONTO PARA BUILD ou AINDA FALTA MATERIAL.
23. Fase 2 visual — somente depois do Gate Multi-Igrejas
 Home cinematográfica e editorial.
 Nova tipografia premium.
 Busca/Ver Todos com fundo visual dinâmico/rotação de imagens, overlay legível e prefers-reduced-motion.
 Marcas d’água e imagens institucionais em seções azuis/brancas.
 Reduzir aparência de catálogo básico e cards repetitivos.
 Página Sobre rica em conteúdo e imagens.
 Preparar Liderança no mesmo sistema visual.
 Não construir dashboard completo nem Revista nessa fase, salvo replanejamento explícito.
24. Pendências conhecidas
 Reconectar o plugin Lovable ao workspace que contém Reino Conecta.
 Refazer a Imagem Institucional 02 no padrão puro/fotográfico.
 Criar/aprovar asset premium para Sinergia.
 Criar/aprovar asset premium para Reforço Escolar Henrique.
 Receber futuramente até 10 fotos REAIS de cada empreendedor e inserir no respectivo perfil.
 Confirmar oficialmente o Pastor Auxiliar e obter foto oficial antes da publicação da página Liderança.
 Confirmar grafia completa/atribuição institucional do idealizador JF Uchôa para rodapé e créditos.
 Definir a revista canônica antes de reabrir a implementação de /revista.
 Definir domínio/remetente de e-mail quando o motor de campanhas for implementado.
25. Bloco de handoff para qualquer novo chat
COMANDO AO PRÓXIMO CHAT
Leia este documento como fonte mestra de continuidade. Não reconstrua decisões antigas por memória. 
Primeiro conecte/inspecione o projeto pelo plugin Lovable; confirme que está no Reino Conecta; respeite o 
protocolo de economia de créditos; trate as atualizações deste dossiê como vigentes; e inicie pelo Gate 
Arquitetural Multi-Igrejas / Pré-Fase 2 em modo PLAN. Não iniciar Build visual antes desse gate.


---

# FECHAMENTO PARA O NOVO CHAT

Ao receber este arquivo:
1. não faça uma nova síntese antes de agir;
2. confirme o estado real pela Lovable;
3. continue **exatamente pelo passo da Site URL**;
4. preserve o domínio `empreendernoreino.com.br`;
5. não publique sem autorização;
6. mantenha o projeto na ordem de prioridades registrada.
