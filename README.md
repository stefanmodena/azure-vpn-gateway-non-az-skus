# Migracao Azure VPN Gateway non-AZ SKUs

Projeto operacional para inventario, planejamento e migracao de Azure VPN Gateways em SKUs non-AZ para SKUs AZ.

## Objetivo

Migrar ou formalizar excecoes para VPN Gateways impactados ate 30/06/2026, com inventario, classificacao de criticidade, plano por gateway, validacao e fechamento executivo.

## Escopo

- Inventario de subscriptions, resource groups, gateways, SKUs, regioes e IPs publicos.
- Coleta de conexoes VPN, BGP, ASN e indicadores de tuneis.
- Classificacao de criticidade por ambiente e dependencia.
- Desenho de ondas de migracao com janela, impacto, rollback e validacao.
- Evidencias para fechamento executivo.

## Politica de seguranca

Nao versionar arquivos com dados sensiveis ou operacionais coletados do ambiente Azure.

Arquivos e diretorios ignorados:

- `outputs/`
- `work/`
- `.azure/`
- arquivos `.env`
- certificados, chaves, tokens, logs e pacotes compactados

## Repositorio de destino

Destino solicitado: `https://github.com/stefanmodena/codex.git`

Status atual: acesso ainda nao confirmado pelo conector GitHub. O retorno da API foi `404`, o que pode indicar repositorio inexistente, privado sem permissao, ou GitHub App nao instalado no repositorio.

## Proximos passos

1. Confirmar acesso ao repositorio GitHub de destino.
2. Criar branch dedicada para este projeto.
3. Enviar somente arquivos seguros de documentacao e automacao.
4. Manter inventarios e evidencias fora do GitHub, salvo se forem sanitizados.

