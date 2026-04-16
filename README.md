# Calculadora Elton Fernandes — Reajuste ANS

Calculadora web para comparação de reajustes aplicados por operadoras de planos de saúde em contratos individuais/familiares com os índices máximos autorizados pela **ANS – Agência Nacional de Saúde Suplementar**.

Ferramenta educacional desenvolvida em homenagem ao **Prof. Elton Fernandes** — Mentoria Estratégica em Direito da Saúde.

---

## Para que serve

Em ações judiciais de revisão de reajuste abusivo — frequentemente associadas à tese do **falso coletivo** — beneficiários de planos comercializados como coletivos empresariais podem ter recebido reajustes muito superiores ao teto que a ANS autoriza para planos individuais.

Esta calculadora permite apurar de forma rápida e visual a diferença entre o que foi efetivamente cobrado pela operadora e o que seria devido caso fossem aplicados os índices regulados pela ANS.

---

## Funcionalidades

### Calculadora Rápida (Seção 1)

Entrada mínima para resultado imediato:

- Valor da mensalidade **antes** e **depois** do reajuste
- Mês/ano em que o reajuste foi aplicado

Resultado: percentual aplicado pela operadora, limite ANS do ciclo correspondente, excesso em pontos percentuais, valor que seria devido, excesso mensal e excesso projetado em 12 meses.

### Comparativo Detalhado (Seção 2)

Para casos com histórico de múltiplos anos:

- **Valor inicial da mensalidade** (antes do 1º reajuste) — ponto de partida de ambas as curvas
- Histórico por ano (modo simplificado) ou mês a mês (para casos com faixa etária, coparticipação, entrada/saída de beneficiário)
- Dados do contrato: beneficiário, operadora, produto, mês de aniversário

### Resultado (Seção 3)

- 5 KPIs: período analisado, total pago à operadora, total devido (curva ANS), indébito total e indébito do triênio
- Tabela mês a mês com linhas de aniversário destacadas
- Observações automáticas em cada aniversário (ex: *"Reajuste operadora: +25,40%. Limite ANS: +9,63%. Excesso: 15,77 p.p."*)
- Notas metodológicas completas
- Exportação: **Imprimir / Salvar PDF** e **Exportar CSV**

---

## Índices ANS incluídos

26 ciclos completos, de **Mai/2000 a Abr/2026**:

| Ciclo | Índice | | Ciclo | Índice |
|---|---|---|---|---|
| Mai/00 – Abr/01 | 5,42% | | Mai/13 – Abr/14 | 9,04% |
| Mai/01 – Abr/02 | 8,71% | | Mai/14 – Abr/15 | 9,65% |
| Mai/02 – Abr/03 | 7,69% | | Mai/15 – Abr/16 | 13,55% |
| Mai/03 – Abr/04 | 9,27% | | Mai/16 – Abr/17 | 13,57% |
| Mai/04 – Abr/05 | 11,75% | | Mai/17 – Abr/18 | 13,55% |
| Mai/05 – Abr/06 | 11,69% | | Mai/18 – Abr/19 | 10,00% |
| Mai/06 – Abr/07 | 8,89% | | Mai/19 – Abr/20 | 7,35% |
| Mai/07 – Abr/08 | 5,76% | | Mai/20 – Abr/21 | 8,14% |
| Mai/08 – Abr/09 | 5,48% | | Mai/21 – Abr/22 | -8,19% |
| Mai/09 – Abr/10 | 6,76% | | Mai/22 – Abr/23 | 15,50% |
| Mai/10 – Abr/11 | 6,73% | | Mai/23 – Abr/24 | 9,63% |
| Mai/11 – Abr/12 | 7,69% | | Mai/24 – Abr/25 | 6,91% |
| Mai/12 – Abr/13 | 7,93% | | Mai/25 – Abr/26 | 6,06% |

---

## Metodologia

A calculadora constrói duas curvas independentes de valor mensal:

1. **Curva Operadora** — valores exatamente como pagos, mês a mês.
2. **Curva ANS** — inicia no mesmo valor da operadora (valor inicial informado) e, a cada aniversário, aplica o índice ANS do ciclo correspondente.

Variações fora do aniversário (faixa etária, entrada/saída de beneficiário, recomposições) são replicadas proporcionalmente em ambas as curvas, isolando o excesso exclusivamente aos reajustes anuais.

A diferença acumulada entre as curvas representa o valor pago a mais pelo beneficiário.

O **triênio** é calculado automaticamente: 36 meses retroativos à data atual, correspondendo ao prazo prescricional aplicável à repetição de indébito.

---

## Como publicar (GitHub Pages)

Este projeto é um site estático de arquivo único (`index.html`). Para publicá-lo:

1. Crie um repositório no GitHub
2. Faça upload do `index.html` (e opcionalmente `README.md` + `LICENSE`)
3. Vá em **Settings → Pages**
4. Em **Source**, selecione a branch `main` e a pasta `/ (root)`
5. Aguarde — a calculadora estará disponível em `https://seu-usuario.github.io/nome-do-repo/`

Não há dependências externas, servidores ou bancos de dados. Todo o cálculo acontece no navegador do usuário.

---

## Ressalva

Esta é uma **ferramenta educacional**. Os valores apurados têm natureza **estimativa** e não substituem:

- Análise técnica-atuarial especializada
- Perícia judicial
- Assessoria jurídica individualizada

Antes de basear qualquer decisão processual nestes cálculos, recomenda-se validação por profissional habilitado.

---

## Licença

Publicado sob a licença MIT. Ver arquivo [LICENSE](LICENSE).

---

## Sobre o Prof. Elton Fernandes

Professor referência em direito da saúde suplementar, condutor de mentoria estratégica voltada à advocacia especializada na área. Esta calculadora foi desenvolvida em homenagem ao seu trabalho de formação técnica na comunidade jurídica.
