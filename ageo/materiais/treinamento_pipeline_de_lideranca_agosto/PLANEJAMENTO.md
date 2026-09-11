# Planejamento — Pipeline da Liderança (AGEO · Agosto)

Workbook impresso de exercícios, entregue em PDF, construído sobre a identidade visual
do relatório do PDL.

| | |
|---|---|
| **Entrega** | PDF A4 retrato, impressão colorida, **só frente** |
| **Uso** | Impresso e distribuído aos participantes |
| **Interação** | Papel e caneta nos exercícios · QR code nos formulários |
| **Versões** | V1 fiel (7 folhas) · V2 autoral (10 folhas) |
| **Impressão** | Impressora de escritório |
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
| 1 | **Não há espaço real para escrever.** As barras do Plano de 30 dias têm 14 mm de altura e nenhuma pauta | Ninguém escreve uma frase ali. O exercício central do material não funciona |
| 2 | Foi desenhado como slide 16:9, não como folha de exercício | Em A4 retrato nada aproveita a altura; os campos ficam achatados |
| 3 | A escada `EU → OUTROS → LÍDERES → FUNÇÃO` aparece na capa e nunca é explicada | O modelo inteiro vira decoração |
| 4 | Não existe ponte entre diagnóstico e plano. A instrução crítica — *pegue as duas menores notas e classifique a lacuna em habilidade, tempo ou valor* — está só nas notas do apresentador | Num material impresso, nota de apresentador não existe. O participante nunca vê |
| 5 | O QR do autodiagnóstico ocupa uma folha inteira só com o código | Numa impressão só frente, isso é uma folha inteira por participante |
| 6 | Os QRs não têm a URL em texto | Se a câmera falhar, acabou. Papel não tem link clicável |
| 7 | O slide 5 acumula dois papéis: exercício das 24h e encerramento | Falta um fechamento de verdade — que é o que o áudio 2 pede |
| 8 | Os círculos 1–5 têm 10 mm e ficam colados | Difícil circular a caneta sem invadir o vizinho |
| 9 | A numeração de rodapé está quebrada: diz 14 e 15, e duas páginas não têm rodapé | Folhas soltas sem identificação se perdem e se embaralham |
| 10 | Calibri e cinza-azulado `#5C6973` | Destoa da paleta quente da referência e some na impressão |
| 11 | "Qr Code" escrito assim, duas vezes | Correção ortográfica — não conta como mudança de conteúdo |

---

## 3. Decisões de formato

| Item | Definição |
|---|---|
| Página | A4 retrato, 210 × 297 mm |
| Impressão | Só frente. Cada página é uma folha de papel |
| Margens | 18 mm simétricas, sem sangria. Como não há frente-e-verso, não precisa de margem de lombada — e blocos coloridos não encostam na borda, porque impressora de escritório não imprime até o corte |
| Cor | RGB. Impressora de escritório varia muito de máquina para máquina, então a prova impressa é obrigatória |
| Fontes | Sora 800 e Inter. O Chrome converte para contornos Type3 no PDF, então as letras viajam com o arquivo e imprimem exatas. O PDF da referência foi gerado assim e já rodou em produção |
| Produção | HTML + CSS de impressão → PDF pelo Chrome headless. Mesmo código-fonte da referência |

### A regra que organiza tudo agora

Sem frente e verso, duas coisas passam a valer:

**1. Cada página custa uma folha.** Sete folhas coloridas por participante, onze
participantes: 77 folhas. Toda página tem que justificar a própria existência. Por isso
o QR do autodiagnóstico, que hoje tem folha própria, volta para o pé da página do
exercício, e a escada vira uma faixa no topo do autodiagnóstico em vez de pedir
folha só para ela.

**2. Cada folha precisa funcionar sozinha.** Folha solta se embaralha, cai, é separada
do resto. Então:

- rodapé em toda página, com o nome do material e `pág. X / 7` — o original já tem esse
  elemento, só está com o número errado;
- as páginas de exercício carregam a própria pergunta em cada bloco, para o participante
  não precisar voltar na folha de instrução. O original já faz isso e vamos preservar.

**Bônus de graça:** o verso de cada folha sai em branco. Dá para orientar o grupo a
rascunhar ali antes de passar a limpo, sem nenhum custo adicional de impressão.

**Se precisar cortar custo:** dobrar as instruções no topo das páginas de exercício leva
o material de 7 para 5 folhas. Não é o que você pediu no áudio — você falou em "a
instrução e o exercício" separados — então mantive separado. Fica registrado como
alavanca, se a conta apertar.

---

## 4. Arquitetura das páginas

### V1 — Fiel · 7 folhas

Regra: **nenhuma palavra de conteúdo muda.** Vale corrigir ortografia, reposicionar
elementos, fundir páginas, e trazer para a folha o que estava só nas notas do
apresentador quando for texto que já existe.

| Pág | Conteúdo | Origem |
|---|---|---|
| 1 | **Capa** — painel creme recuado, anel laranja no alto, disco amarelo embaixo, selo AGEO + Sinapsy, título, barra laranja, subtítulo, assinatura "Treinamento prático" | original s1 · **pronta** |
| 2 | **Autodiagnóstico** — faixa da escada no topo, 6 afirmações, escala 1–5 para circular, e o QR do formulário no pé com a URL em texto | original s1 + s2 + s3 |
| 3 | **Instrução — Plano de 30 Dias** | `conteudo_novo` bloco 1 |
| 4 | **Plano de 30 Dias** ← exercício, folha limpa, 5 blocos com pauta | original s4 |
| 5 | **Instrução — compromisso de 24 horas** | `conteudo_novo` bloco 2 |
| 6 | **Compromisso de 24 horas** ← exercício, folha limpa, 3 blocos com pauta | original s5 |
| 7 | **Avaliação + Encerramento** — QR da avaliação em cima, "Obrigada!" com a foto da equipe embaixo | original s6 + áudio 2 |

Duas folhas a menos que na versão anterior deste plano, e nenhuma perda de conteúdo:
o QR volta para o pé do exercício que ele registra, e a escada entra como faixa no
topo do autodiagnóstico.

**A capa está pronta e aprovada.** Direção escolhida: painel creme recuado 12 mm da
borda do papel, com o anel laranja sangrando pela borda do *painel*. Impressora de
escritório não imprime até o corte, então a margem branca deixa de ser defeito e
passa a ser moldura.

**Onde ficou a escada.** Fora da capa, por decisão da cliente. Na V1 ela entra como
faixa horizontal no topo da página do autodiagnóstico — e ali ela trabalha, porque as
6 afirmações testam degraus diferentes. Custo: zero folha extra. Na V2 continua com
página própria e explicada.

**Remoções autorizadas no texto da V1.** Duas, ambas a pedido da cliente:

1. A assinatura da capa perdeu o "• material editável" — informação interna, e o
   participante recebe o material já impresso.
2. Saiu do rodapé da última página o "Base: Pipeline da Liderança — Ram Charan,
   Stephen Drotter e James Noel".

Fora isso, nenhuma palavra do original mudou.

### V2 — Autoral · 10 folhas

Mantém todo o conteúdo original e acrescenta o que falta para o argumento fechar.

| Pág | Conteúdo | Status |
|---|---|---|
| 1 | Capa | = V1 |
| 2 | **A escada: o que muda a cada passagem** — desenvolve os três eixos que já estão no subtítulo da capa e nunca aparecem: habilidades, uso do tempo, valores profissionais | novo · resolve o problema 3 |
| 3 | Autodiagnóstico + QR — cada item marcado com o degrau que testa | = V1 + marcação |
| 4 | **Como ler sua nota** — duas menores notas; a lacuna é de habilidade, tempo ou valor? | novo · resolve o problema 4. É a página que faz o diagnóstico virar plano |
| 5 | Instrução — Plano de 30 Dias | = V1 |
| 6 | Plano de 30 Dias ← exercício | = V1 |
| 7 | Instrução — compromisso de 24 horas | = V1 |
| 8 | Compromisso de 24 horas ← exercício | = V1 |
| 9 | **O que acontece depois** — o combinado de acompanhamento: quem cobra, quando, como | novo · dá sobrevida ao plano |
| 10 | **Avaliação + Encerramento** | = V1 |

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

- **O fundo creme não pode cobrir a folha inteira.** Chapar `#EAE7DC` em 7 páginas gasta
  tinta, encarece e sai manchado em impressora de escritório. O creme fica em faixas e
  cartões; o corpo da página é o branco do papel.
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

É aqui que o material ganha ou perde. Com margens de 18 mm sobram **261 mm** de altura
útil por folha; descontando cabeçalho e rodapé, **206 mm** de área de trabalho.

**Pauta.** Linha de escrita a cada **9 mm**, em `rgba(31,31,31,.18)` — visível para guiar,
discreta o bastante para não competir com a caneta. Nunca uma caixa vazia sem pauta:
sem linha, a pessoa escreve torto e desiste no meio.

**Plano de 30 Dias — folha inteira.** 5 blocos de **41 mm**: tag da categoria, a pergunta
e **2 linhas** de escrita cada.

**Compromisso de 24 horas — folha inteira.** 3 blocos de **69 mm**, com **5 linhas** cada.
São as respostas que mais importam e as que o original mais aperta.

**Escala 1–5.** Círculos de **9 mm** de diâmetro com **7 mm** entre eles, alinhados à
direita da afirmação, com o cabeçalho "1 raramente … 5 consistentemente" uma vez no topo
em vez de repetido em cada linha. Traço de 1 pt, vazado — feito para circular a caneta.

**QR code.** **38 mm** de lado, correção de erro alta por causa do logo Sinapsy no centro,
preto puro sobre branco — laranja reduz o contraste de leitura. Sempre com a **URL em
texto logo abaixo**, porque no papel não existe link clicável e câmera falha.

- autodiagnóstico → `https://form.respondi.app/xd7sBWfV`
- avaliação → `https://form.respondi.app/3VutxWx6`

Confirmados pela cliente.

**Sem campo de nome e data.** Decidido: o caderno é do participante, não é recolhido.

---

## 7. Conteúdo

- **V1:** texto intocado. Só ortografia ("Qr Code" → "QR Code") e quebras de linha.
- `conteudo_novo.txt` confirmado: bloco 1 = instrução da atividade 1, bloco 2 = instrução
  da atividade 2. O terceiro bloco é cópia idêntica do segundo — descartado.
- **V2:** copy nova só nas 3 páginas adicionadas.
- A referência bibliográfica (Charan, Drotter e Noel) foi removida a pedido da cliente.

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
| Preview para aprovação | `artifact-design` | cada versão vira uma página de aprovação antes de virar PDF |
| Auditoria antes de fechar | `impeccable` | hierarquia e carga cognitiva página a página |
| Antes de mostrar a V2 | `grilling` | furar o próprio argumento da V2 antes de a cliente furar |

Saíram do plano por causa do formato impresso: `pptx`, `dataviz`, `emil-design-eng`
e tudo que dependia de interação em tela.

---

## 9. Fases

| Fase | Entrega |
|---|---|
| 0 | Estrutura no repositório e este planejamento ✅ |
| 1 | Assets — QRs em 38 mm/300 dpi, selo AGEO, logo Sinapsy, `equipe.jpeg` tratada |
| 2 | `shared/tokens.css` e `shared/print.css` — grade A4, pauta, componentes |
| 3 | V1 completa → PDF de prova → aprovação |
| 4 | V2, com a copy nova passando pelo humanizer → PDF de prova → aprovação |
| 5 | Teste de impressão real na impressora que vai rodar o material, ajuste de margem e tinta, PDFs finais |

**A fase 5 não é opcional.** Material impresso só está pronto depois de sair de uma
impressora de verdade — e impressora de escritório varia muito. Cor na tela mente.

---

## 10. Definições fechadas

| | |
|---|---|
| URLs dos formulários | Confirmadas: `xd7sBWfV` no autodiagnóstico, `3VutxWx6` na avaliação |
| Frente e verso | Não. Só frente |
| Campo de nome e data | Não |
| Impressão | Impressora de escritório |
| Repositório público | Confirmado |
| Foto do encerramento | `equipe.jpeg`, a mesma do relatório do PDL |

Premissa assumida, sem bloquear: as folhas podem acabar soltas ou grampeadas no canto,
então cada uma é desenhada para funcionar sozinha, com rodapé de identificação e
numeração.
