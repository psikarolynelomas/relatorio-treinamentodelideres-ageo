# Planejamento — Pipeline da Liderança (AGEO · Agosto)

Workbook impresso de exercícios, entregue em PDF, construído sobre a identidade visual
do relatório do PDL.

| | |
|---|---|
| **Entrega** | PDF A4 retrato, impressão colorida |
| **Uso** | Impresso e distribuído aos participantes |
| **Interação** | Papel e caneta nos exercícios · QR code nos formulários |
| **Versões** | V1 fiel (8 páginas) · V2 autoral (12 páginas) |
| **Fonte de design** | `index.html` e `styles.css` na raiz do repositório |
| **Fonte de conteúdo** | `apresentacao_original.pptx` + `conteudo_novo.txt` + áudios |

---

## 1. Objetivo do material

Não é um material para ser assistido nem lido. É um **caderno de exercícios que o
participante leva embora preenchido**. O sucesso não é "entendeu o Pipeline de
Liderança" — é sair da sala com as folhas escritas e uma ação marcada na agenda de
amanhã.

Cinco resultados observáveis por participante:

1. Sabe qual passagem do pipeline está incompleta na realidade dele.
2. Registrou esse diagnóstico no formulário — vira dado para a Sinapsy.
3. Tem um Plano de 30 dias escrito à mão, com evidência e com alguém que cobra.
4. Assumiu um compromisso executável em 24 horas.
5. Avaliou o treinamento.

A divisão de papéis entre papel e QR é limpa e vale ser explorada no design:
**o papel é o que o líder guarda; o formulário é o que a Sinapsy mede.**

O ciclo fecha em si mesmo — o QR de avaliação deste material alimenta o relatório que
estamos usando como referência de design.

---

## 2. O que o original acerta e onde ele trava

### Acerta

- A sequência está certa: diagnosticar → planejar → comprometer → avaliar.
- As 6 afirmações do autodiagnóstico são curtas, comportamentais e em primeira pessoa.
- Parar / Começar / Continuar / Evidência / Apoio é um bom quadro. "Evidência" e "Apoio"
  são o que transforma plano em hábito.
- As notas do apresentador existem e são boas.

### Trava

| # | Problema | Efeito no papel |
|---|---|---|
| 1 | Foi desenhado como slide 16:9, não como folha de exercício | Em A4 retrato nada aproveita a altura; os campos ficam achatados |
| 2 | **Não há espaço real para escrever.** As barras do Plano de 30 dias têm 14mm de altura e nenhuma pauta | Ninguém escreve uma frase ali. O exercício central do material não funciona |
| 3 | A escada `EU → OUTROS → LÍDERES → FUNÇÃO` aparece na capa e nunca é explicada | O modelo inteiro vira decoração |
| 4 | Não existe ponte entre diagnóstico e plano. A instrução crítica — *pegue as duas menores notas e classifique a lacuna em habilidade, tempo ou valor* — está só nas notas do apresentador | Num material impresso, nota de apresentador não existe. O participante nunca vê |
| 5 | O QR do autodiagnóstico ocupa uma folha inteira só com o código | Desperdiça uma folha e tira o QR do contexto do exercício |
| 6 | Os QRs não têm a URL em texto | Se a câmera falhar, acabou. Papel não tem link clicável |
| 7 | O slide 5 acumula dois papéis: exercício das 24h e encerramento | Falta um fechamento de verdade — que é o que o áudio 2 pede |
| 8 | Calibri e cinza-azulado `#5C6973` | Destoa da paleta quente da referência e some na impressão |
| 9 | Os círculos 1–5 têm 10mm e ficam colados | Difícil circular a caneta sem invadir o vizinho |
| 10 | "Qr Code" escrito assim, duas vezes | Correção ortográfica — não conta como mudança de conteúdo |

---

## 3. Decisões de formato

| Item | Definição |
|---|---|
| Página | A4 retrato, 210 × 297 mm |
| Margens | 18 mm, sem sangria — blocos coloridos não encostam na borda, para rodar em impressora comum |
| Cor | RGB para impressão de escritório. Se for para gráfica, converto para CMYK (o `#F8471E` perde brilho em CMYK e precisa de ajuste) |
| Fontes | Sora 800 e Inter, embutidas no PDF |
| Produção | HTML + CSS de impressão → PDF pelo Chrome headless. Mesmo código-fonte da referência |
| Paginação | Múltiplo de 4, para fechar certo em frente-e-verso e em caderno grampeado |

### A regra de paginação que organiza tudo

Impresso frente e verso, as páginas que ficam **lado a lado** com o caderno aberto são
as pares com as ímpares seguintes: (2,3), (4,5), (6,7)…

Então toda **instrução vai em página par** e o **exercício correspondente na ímpar
seguinte**. O participante lê a instrução e escreve sem precisar virar folha. Isso
resolve sozinho metade do problema de usabilidade do material.

---

## 4. Arquitetura das páginas

### V1 — Fiel · 8 páginas (4 folhas)

Regra: **nenhuma palavra de conteúdo muda.** Vale corrigir ortografia, reposicionar
elementos, fundir ou dividir páginas, e trazer para a folha o que estava só nas notas
do apresentador quando for texto que já existe.

| Pág | Conteúdo | Origem |
|---|---|---|
| 1 | **Capa** — selo AGEO + Sinapsy, título, barra laranja, subtítulo, faixa "Treinamento prático • material editável" | original s1 |
| 2 | **A escada** — `EU → OUTROS → LÍDERES → FUNÇÃO` em diagrama grande, sai da capa e ganha a folha | original s1 (relocado) |
| 3 | **Autodiagnóstico** — 6 afirmações, escala 1–5 para circular, e o QR do formulário no rodapé com a URL em texto | original s2 + s3 (fundidos) |
| 4 | **Instrução — Plano de 30 Dias** | `conteudo_novo` bloco 1 |
| 5 | **Plano de 30 Dias** ← exercício, folha limpa, 5 blocos com pauta | original s4 |
| 6 | **Instrução — compromisso de 24 horas** | `conteudo_novo` bloco 2 |
| 7 | **Compromisso de 24 horas** ← exercício, folha limpa, 3 blocos com pauta | original s5 |
| 8 | **Avaliação + Encerramento** — QR da avaliação em cima, "Obrigada!" com a foto da equipe embaixo | original s6 + áudio 2 |

Pares que ficam lado a lado: (2,3) escada e diagnóstico · (4,5) instrução e plano ·
(6,7) instrução e compromisso. Os dois exercícios ficam com a folha inteira.

### V2 — Autoral · 12 páginas (6 folhas)

Mantém todo o conteúdo original e acrescenta o que falta para o argumento fechar.

| Pág | Conteúdo | Status |
|---|---|---|
| 1 | Capa | = V1 |
| 2 | **A escada: o que muda a cada passagem** — desenvolve os três eixos que já estão no subtítulo da capa e nunca aparecem: habilidades, uso do tempo, valores profissionais | novo · resolve o problema 3 |
| 3 | Autodiagnóstico — cada item marcado com o degrau que testa | = V1 + marcação |
| 4 | **Como ler sua nota** — duas menores notas; a lacuna é de habilidade, tempo ou valor? | novo · resolve o problema 4. É a página que faz o diagnóstico virar plano |
| 5 | QR do autodiagnóstico, com espaço próprio | separado da p.3 |
| 6 | Instrução — Plano de 30 Dias | = V1 |
| 7 | Plano de 30 Dias ← exercício | = V1 |
| 8 | Instrução — compromisso de 24 horas | = V1 |
| 9 | Compromisso de 24 horas ← exercício | = V1 |
| 10 | **O que acontece depois** — o combinado de acompanhamento: quem cobra, quando, como | novo · dá sobrevida ao plano |
| 11 | QR da avaliação | = V1 |
| 12 | **Encerramento** — "Obrigada!", foto da equipe, referência bibliográfica | = V1 |

Todos os pares lado a lado funcionam: (2,3) escada e diagnóstico · (4,5) leitura da nota
e registro no formulário · (6,7) e (8,9) instrução e exercício · (10,11) acompanhamento
e avaliação.

Toda copy nova passa por `/humanizer` antes de entrar.

---

## 5. Design

### Tokens, herdados de `styles.css`

```
--ink       #1F1F1F    --cream     #EAE7DC    --orange  #F8471E
--ink-soft  #56544C    --cream-2   #F3F1E9    --yellow  #FFDF2C
--card      #FFFFFF    --dark      #22231C    --blue    #2441CB
```

Sora 800 nos títulos, Inter no texto.

### Ajustes obrigatórios para papel

- **O fundo creme não pode cobrir a folha inteira.** Chapar `#EAE7DC` em 8 páginas gasta
  tinta, encarece e sai manchado em impressora comum. O creme fica em faixas e cartões;
  o corpo da página é branco do papel.
- Corpo de texto em `#1F1F1F` sobre branco. Nada de cinza claro.
- `#5C6973` sobre creme dá **4,56:1**. Troca por `--ink-soft #56544C`, que dá **6,13:1**.
- Branco sobre laranja dá **3,55:1** — só em texto grande, nunca em corpo de texto. A
  referência faz isso na página 8; não vamos repetir.
- Blocos escuros (`--dark`) no máximo em duas páginas, e nunca nas de escrever.

### Cor por bloco

| Bloco | Cor |
|---|---|
| Diagnóstico | laranja |
| Plano de 30 dias | azul |
| Compromisso 24h | amarelo com âncora escura |
| Avaliação e encerramento | creme |

---

## 6. A experiência de preencher

É aqui que o material ganha ou perde. Especificações concretas:

**Pauta.** Linha de escrita a cada **9 mm**, em `rgba(31,31,31,.18)` — visível para guiar,
discreta o bastante para não competir com a caneta. Nunca uma caixa vazia sem pauta:
sem linha, a pessoa escreve torto e desiste no meio.

**Plano de 30 Dias — página inteira.** Cabeçalho enxuto (~45 mm), sobram ~215 mm para
5 blocos de ~43 mm: tag da categoria, a pergunta e **2 linhas** de escrita cada.

**Compromisso de 24 horas — página inteira.** 3 blocos de ~70 mm, com **4 linhas** cada.
São as respostas que mais importam e as que o original mais aperta.

**Escala 1–5.** Círculos de **9 mm** de diâmetro com **7 mm** entre eles, alinhados à
direita da afirmação, com cabeçalho "1 raramente … 5 consistentemente" uma vez no topo
em vez de repetido em cada linha. Traço de 1pt, vazado — feito para circular a caneta.

**QR code.** **38 mm** de lado, correção de erro alta por causa do logo Sinapsy no centro,
preto puro sobre branco (nada de laranja: reduz o contraste de leitura). Sempre com a
**URL em texto logo abaixo** — no papel não existe link clicável e câmera falha.

- autodiagnóstico → `https://form.respondi.app/xd7sBWfV`
- avaliação → `https://form.respondi.app/3VutxWx6`

Extraí os dois destinos decodificando os QRs do pptx. Confirmar antes de gerar o PDF.

**Identificação.** Proponho uma linha de **Nome e Data** na capa. É a única adição que eu
faria mesmo na V1 — um caderno que é distribuído, preenchido e às vezes recolhido precisa
disso. Fácil de vetar (ver decisão 3).

---

## 7. Conteúdo

- **V1:** texto intocado. Só ortografia ("Qr Code" → "QR Code") e quebras de linha.
- `conteudo_novo.txt` confirmado: bloco 1 = instrução da atividade 1, bloco 2 = instrução
  da atividade 2. O terceiro bloco é cópia idêntica do segundo — descartado.
- **V2:** copy nova só nas 3 páginas adicionadas.
- A referência bibliográfica (Charan, Drotter e Noel) sai do rodapé de uma página só e
  ganha lugar fixo no encerramento.

---

## 8. Skills por etapa

| Momento | Skill | Por quê |
|---|---|---|
| Toda copy nova — V2, microcopy, encerramento | `/humanizer` | tirar a cara de IA: contraste "não X, mas Y", tríades forçadas, frase de efeito no fim |
| Segunda passada, se sobrar padrão | `stop-slop` | complementa o humanizer. Não rodar os dois no mesmo trecho sem ler o resultado |
| Diagrama da escada | `artifact-diagramming` | o SVG dos 4 degraus tem que mostrar mecanismo, não enfeitar |
| Formalizar os tokens | `design-system` | vira token set reaproveitável nos próximos materiais da Sinapsy |
| Legibilidade, hierarquia, escala tipográfica | `ui-ux-pro-max` | as guidelines valem igual no papel: medida de linha, peso, espaçamento |
| Geração e fechamento do PDF | `pdf` | A4, fontes embutidas, junção das páginas, verificação |
| Alternativa de produção | `opendesign-pdf` | se o caminho Chrome headless der problema com fonte ou quebra de página |
| Preview para você aprovar | `artifact-design` | cada versão vira uma página de aprovação antes de virar PDF |
| Auditoria antes de fechar | `impeccable` | hierarquia e carga cognitiva página a página |
| Antes de mostrar a V2 | `grilling` | furar o próprio argumento da V2 antes de a cliente furar |

Saíram do plano por causa da mudança de formato: `pptx`, `dataviz`, `emil-design-eng`
e tudo que dependia de interação em tela.

---

## 9. Fases

| Fase | Entrega |
|---|---|
| 0 | Estrutura no repositório e este planejamento ✅ |
| 1 | Assets — QRs em 38 mm/300dpi, selo AGEO, logo Sinapsy, `equipe.jpeg` tratada |
| 2 | `shared/tokens.css` e `shared/print.css` — grade A4, pauta, componentes |
| 3 | V1 completa → PDF de prova → sua aprovação |
| 4 | V2, com a copy nova passando pelo humanizer → PDF de prova → aprovação |
| 5 | Teste de impressão real (uma folha de cada tipo), ajuste de margem e tinta, PDFs finais |

**A fase 5 não é opcional.** Material impresso só está pronto depois de sair de uma
impressora de verdade. Cor na tela mente.

---

## 10. Decisões pendentes

1. **As duas URLs dos formulários estão certas?** Decodifiquei dos QRs do pptx:
   `form.respondi.app/xd7sBWfV` no autodiagnóstico e `form.respondi.app/3VutxWx6` na
   avaliação. Se os formulários mudaram, preciso dos links novos.
2. **Frente e verso ou só frente?** Estou desenhando para frente e verso — é o que faz a
   instrução ficar ao lado do exercício. Se for só frente, a lógica de paginação muda.
3. **Linha de Nome e Data na capa?** É adição de conteúdo, então precisa do seu aval para
   entrar na V1.
4. **Impressora de escritório ou gráfica?** Muda sangria e conversão de cor.
5. **Este repositório é público.** O relatório do PDL já está lá. Confirma que o material
   de treinamento da AGEO também pode ficar.
