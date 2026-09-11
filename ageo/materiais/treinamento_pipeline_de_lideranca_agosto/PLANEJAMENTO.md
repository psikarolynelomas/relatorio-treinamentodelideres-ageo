# Planejamento — Pipeline da Liderança (AGEO · Agosto)

Reconstrução da apresentação `apresentacao_original.pptx` em duas versões, usando a identidade visual do relatório do PDL como referência.

- **Fonte de design:** `index.html` + `styles.css` na raiz deste repositório — é o arquivo que gerou o PDF `referencia_de_formato_e_identidade_visual.pdf`.
- **Fonte de conteúdo:** `apresentacao_original.pptx` (6 slides) + `conteudo_novo.txt` + 3 áudios de instrução.

---

## 1. Objetivo da apresentação

Isto não é um material para ser assistido. É um **instrumento de trabalho do fim do treinamento**. O sucesso não é "o participante entendeu o Pipeline de Liderança" — é o participante sair da sala com coisas escritas e uma delas marcada na agenda de amanhã.

Cinco resultados observáveis por participante:

1. Sabe qual passagem do pipeline está incompleta na realidade dele (autodiagnóstico).
2. Registrou esse diagnóstico no formulário — vira dado para a Sinapsy.
3. Tem um Plano de 30 dias escrito, com evidência e com alguém que cobra.
4. Assumiu um compromisso executável em 24 horas.
5. Avaliou o treinamento.

Vale notar o ciclo: o QR de avaliação **desta** apresentação alimenta o relatório que estamos usando como referência de design. O sistema visual fecha em si mesmo.

---

## 2. O que o original acerta e onde ele trava

### Acerta

- A sequência está certa: diagnosticar → planejar → comprometer → avaliar.
- As 6 afirmações do autodiagnóstico são curtas, comportamentais e em primeira pessoa.
- Parar / Começar / Continuar / Evidência / Apoio é um bom quadro. "Evidência" e "Apoio" são justamente o que transforma plano em hábito.
- As notas do apresentador existem e são boas.

### Trava

| # | Problema | Efeito |
|---|---|---|
| 1 | A escada `EU → OUTROS → LÍDERES → FUNÇÃO` aparece na capa e nunca é explicada | O modelo inteiro vira decoração |
| 2 | Não existe ponte entre diagnóstico e plano. A instrução crítica — *pegue as duas menores notas e classifique a lacuna em habilidade, tempo ou valor* — está escondida nas notas do apresentador | O participante pula do "notei" para o "planejo" sem saber o que planejar |
| 3 | O QR do autodiagnóstico ocupa um slide inteiro repetindo o título do anterior, sem instrução do que responder | Tela vazia no momento em que o grupo mais precisa de direção |
| 4 | Não há espaço real para escrever: as barras do Plano de 30 dias são decorativas | Projetado, ninguém escreve; impresso, a altura não comporta uma frase |
| 5 | Rodapé numera 14 e 15 num arquivo de 6 slides; 2 slides sem rodapé | Sinal de recorte de um deck maior (ver Decisão 1) |
| 6 | O slide 5 acumula dois papéis: exercício das 24h **e** encerramento | Falta um fechamento de verdade — que é o que o áudio 2 pede |
| 7 | Calibri e cinza-azulado `#5C6973` | Destoa da paleta quente da referência; hierarquia rasa |
| 8 | Alvos de clique de 0,40in (≈38px) sem estado; `#5C6973` sobre creme dá 4,56:1 | Interação frágil e contraste no limite do AA |
| 9 | "Qr Code" escrito assim, duas vezes | Correção ortográfica — não conta como mudança de conteúdo |

---

## 3. Decisão de formato

**reveal.js + GitHub Pages**, igual à referência. Três motivos:

- Mesmo sistema visual, mesmo repositório, mesmo fluxo de publicação que já funciona.
- Roda projetado (facilitador), no celular (participante) e imprime (workbook).
- É a única opção em que os campos de resposta podem ser interativos de verdade.

O mesmo arquivo serve três modos:

| Modo | Como | Para quem |
|---|---|---|
| Projeção | padrão | facilitador conduz |
| Participante | abre o link no celular, preenche, salva no navegador, baixa o próprio plano | cada líder |
| Impressão | `?print-pdf` + `@media print` | workbook A4 paisagem com pauta de verdade |

---

## 4. Arquitetura de slides

### V1 — Fiel

Regra: **nenhuma palavra de conteúdo muda.** Permitido: ortografia e acentuação, reposicionar, dividir um slide em dois, e promover nota do apresentador para a Notes View do reveal (tecla `S`).

| # | Slide | Origem |
|---|---|---|
| 1 | Capa — badge AGEO + Sinapsy, eyebrow, título, barra laranja, subtítulo, chips. A escada ganha tratamento em SVG (degraus ascendentes), não 4 pílulas empilhadas | original s1 |
| 2 | Autodiagnóstico — 6 afirmações, escala 1–5 interativa, contador "0 / 6" | original s2 |
| 3 | QR do autodiagnóstico — QR grande + URL legível + o que responder + tempo estimado | original s3 |
| 4 | **Como preencher o Plano de 30 Dias** — método à esquerda, cartões de exemplo (Comunicação / Delegação) à direita | `conteudo_novo` bloco 1 |
| 5 | Plano de 30 dias — 5 linhas com campo de escrita real | original s4 |
| 6 | **Como fazer o compromisso de 24h** — os 3 passos numerados | `conteudo_novo` bloco 2 |
| 7 | Compromisso 24h — 3 cartões com campo + faixa "uma ação nas próximas 24 horas" | original s5 |
| 8 | QR da avaliação — mesmo tratamento do slide 3 | original s6 |
| 9 | **Encerramento** — "Obrigada!" + mensagem de boa sorte, espelhando a página 9 da referência | áudio 2 |

**9 slides.**

### V2 — Autoral

Mantém todo o conteúdo original e acrescenta o que falta para o argumento fechar.

| # | Slide | Status |
|---|---|---|
| 1 | Capa | = V1 |
| 2 | **A escada: o que muda a cada passagem** — desenvolve `EU → OUTROS → LÍDERES → FUNÇÃO` e os três eixos que já estão no subtítulo da capa (habilidades, uso do tempo, valores profissionais) | novo · resolve o problema 1 |
| 3 | Autodiagnóstico — cada afirmação marcada com o degrau que ela testa | = V1 + marcação |
| 4 | **Como ler sua nota** — duas menores notas; a lacuna é de habilidade, tempo ou valor? | novo · resolve o problema 2. É o slide que faz o diagnóstico virar plano |
| 5 | QR do autodiagnóstico | = V1 |
| 6 | Como preencher o Plano de 30 Dias | = V1 |
| 7 | Plano de 30 dias | = V1 |
| 8 | Como fazer o compromisso de 24h | = V1 |
| 9 | Compromisso 24h | = V1 |
| 10 | **O que acontece depois** — combinado de acompanhamento: quem cobra, quando, como | novo · dá sobrevida ao plano |
| 11 | QR da avaliação | = V1 |
| 12 | Encerramento | = V1 |

**12 slides.** Toda copy nova passa por `/humanizer` antes de entrar.

---

## 5. Design

### Tokens (herdados de `styles.css`, sem reinventar)

```
--ink       #1F1F1F    --cream     #EAE7DC    --orange  #F8471E
--ink-soft  #56544C    --cream-2   #F3F1E9    --yellow  #FFDF2C
--card      #FFFFFF    --dark      #22231C    --blue    #2441CB
```

Sora 800 nos títulos, Inter no texto. Canvas 1280×760.

### Componentes novos

Mesma gramática da referência: cartão branco, raio 16–20px, sombra suave, borda-topo colorida.

- `.escada` — SVG dos 4 degraus
- `.likert` — escala 1–5 acessível
- `.campo` — textarea que cresce, com pauta na impressão
- `.qr-action` — QR + URL + microcopy
- `.exemplo` — cartão de exemplo com tag de categoria
- `.timer` — cronômetro do facilitador (opcional)

### Cor por bloco

Evita monotonia e dá orientação dentro do deck.

| Bloco | Cor |
|---|---|
| Diagnóstico | laranja |
| Plano de 30 dias | azul |
| Compromisso 24h | amarelo sobre dark |
| Avaliação e encerramento | creme + foto |

### Acessibilidade

- `#5C6973` sobre creme dá **4,56:1**. Troca por `--ink-soft #56544C` → **6,13:1**.
- Branco sobre laranja dá **3,55:1** — só para texto grande, nunca para corpo de texto. A referência faz isso na página 8; não vamos repetir.
- Alvos de toque ≥ 44px. Foco visível. Escala 1–5 como `radiogroup` navegável por seta.
- `prefers-reduced-motion` respeitado.

---

## 6. Interação

1. **Escala 1–5** — `role="radiogroup"`, setas ←→, alvo de 48px, preenchimento laranja, estado salvo. Contador de progresso. Ao completar as 6, aparece discretamente *"suas duas menores: itens X e Y"*, que é exatamente a ponte para o plano.
2. **Campos de escrita** — textarea auto-grow, placeholder com exemplo concreto ("Ex.: parar de revisar cada proposta antes de enviar"), salvo em `localStorage`, sem login.
3. **Botão "Baixar meu plano"** — junta autodiagnóstico + 30 dias + 24h num arquivo. É o que faz o líder não perder o que escreveu.
4. **QR** — regerar em alta resolução com o logo Sinapsy, mais a URL em texto e link clicável no celular:
   - autodiagnóstico → `https://form.respondi.app/xd7sBWfV`
   - avaliação → `https://form.respondi.app/3VutxWx6`

   (extraídos dos QRs do pptx; confirmar antes de publicar)
5. **Impressão** — `@media print`: pauta real em três alturas, círculos 1–5 vazados, QR em preto puro, sem sombra.
6. **Facilitador** — notas na tecla `S`; timer opcional de 10 min no slide do plano.

---

## 7. Conteúdo

- **V1:** texto intocado. Só ortografia ("Qr Code" → "QR Code") e quebras de linha.
- O bloco 2 do `conteudo_novo.txt` aparece **duplicado** no arquivo, duas vezes e idêntico. Tratado como duplicata — usar uma vez (ver Decisão 5).
- **V2:** copy nova só nos 3 slides adicionados e na microcopy dos campos.
- A referência bibliográfica (Charan, Drotter e Noel) sai do rodapé de um slide só e passa a ter um lugar fixo e discreto.

---

## 8. Skills por etapa

| Momento | Skill | Por quê |
|---|---|---|
| Qualquer copy nova — V2, microcopy, placeholders, encerramento | `/humanizer` | tirar a cara de IA: contraste "não X, mas Y", tríades forçadas, frase de efeito no fim |
| Segunda passada, se sobrar padrão | `stop-slop` | complementa o humanizer. Não rodar os dois no mesmo trecho sem ler o resultado |
| Antes de publicar qualquer preview | `artifact-design` | calibrar o investimento de design do artifact |
| Escada do pipeline em SVG | `artifact-diagramming` | diagrama que mostra mecanismo e sobrevive a light/dark |
| Formalizar os tokens | `design-system` | virar token set reaproveitável nos próximos materiais da Sinapsy |
| Revisão de UI/UX, tipografia, alvos, estados | `ui-ux-pro-max` | checklist de guidelines e padrões de interação |
| Polimento final de frontend | `impeccable` | hierarquia, carga cognitiva, estados vazios e de erro |
| Micro-interações da escala e dos campos | `emil-design-eng` | foco, hover, transição — o que faz parecer software bem feito |
| Se entrar gráfico (ex.: perfil do autodiagnóstico) | `dataviz` | forma e paleta corretas antes de escrever código de gráfico |
| Se precisar entregar `.pptx` | `pptx` | ler o original e gerar versão PowerPoint |
| Workbook impresso | `pdf` | PDF final, merge, forms |
| Antes do commit final | `/code-review` + `/simplify` | HTML e CSS limpos antes de publicar |
| Stress-test da estrutura da V2 | `grilling` | furar o próprio argumento antes de mostrar para a cliente |

Fora de skills: Browser pane para QA visual em 1280×760 e no mobile; Artifact para aprovação antes de commitar.

---

## 9. Fases

| Fase | Entrega |
|---|---|
| 0 | Estrutura no repo + este planejamento ✅ |
| 1 | Assets: QRs em alta, badge AGEO, logo Sinapsy, foto |
| 2 | `shared/tokens.css` + componentes novos |
| 3 | V1 completa → preview → aprovação |
| 4 | V2 (copy nova via `/humanizer`) → preview → aprovação |
| 5 | QA (impressão, mobile, teclado, contraste), code-review, publicação no Pages, PDFs |

---

## 10. Decisões pendentes

1. **Esses 6 slides são o treinamento inteiro ou um recorte?** O rodapé numera 14 e 15. Se existe um deck maior, preciso dele — senão a V2 vai propor slides que já existem lá.
2. **Formato de entrega:** site no Pages + PDF resolve? Precisa de `.pptx` editável também?
3. **Foto do encerramento:** uso a `equipe.jpeg` que já está no repo ou tem foto nova deste treinamento?
4. **Dados preenchidos:** ficam só no navegador do participante (privado, some se ele limpar os dados) ou também precisam chegar em algum lugar?
5. **O bloco repetido do `conteudo_novo.txt` é duplicata mesmo?**
6. **Este repositório é público.** O relatório do PDL já está publicado nele. Confirmar que o material de treinamento da AGEO também pode ficar público.
