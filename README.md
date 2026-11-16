<p align="right"><b>ðŸ‡§ðŸ‡· PortuguÃªs</b> Â· <a href="README.en.md">ðŸ‡ºðŸ‡¸ English</a></p>

<p align="center">
  <img src="assets/os-coach-banner.png" alt="OS Coach, o Arquiteto de Sistemas de IA: vocÃª constrÃ³i a base. As seis camadas Identidade, Contexto, Regras, Skills, Tools e Agentes formando o Agentic OS, sob o lema arquitetura, lÃ³gica e estrutura. NÃ£o Ã© sobre executar, Ã© sobre estruturar a fundaÃ§Ã£o." width="100%">
</p>

# /os-coach

ðŸ“˜ **Guia visual (landing + passo a passo):** [inematds.github.io/os-coach](https://inematds.github.io/os-coach/)

> **O que Ã© isto, em uma frase:** uma skill do Claude Code que pega na sua mÃ£o e te guia, passo a passo, na construÃ§Ã£o do seu prÃ³prio **OS agÃªntico** (um sistema operacional feito de arquivos, que entende o seu objetivo e trabalha por vocÃª), uma camada de cada vez, dentro de qualquer pasta. VocÃª nÃ£o precisa saber programar. A skill faz o trabalho tÃ©cnico. VocÃª sÃ³ toma as decisÃµes.

Pense nela como um treinador particular. VocÃª diz aonde quer chegar, ela faz duas ou trÃªs perguntas em portuguÃªs claro, e entÃ£o **constrÃ³i os arquivos e pastas de verdade** para vocÃª, explicando o que fez e por quÃª. SessÃ£o apÃ³s sessÃ£o, ela lembra exatamente onde vocÃª parou.

Tudo se apoia numa Ãºnica ideia: **um OS agÃªntico Ã©, na maior parte, encanamento. O modelo de IA Ã© os 20% baratos.** VocÃª nÃ£o consegue conversar com os seus dados se os bastidores estÃ£o uma bagunÃ§a. Por isso a skill arruma os bastidores primeiro, e sÃ³ depois empilha capacidade em cima.

<p align="center">
  <img src="assets/os-layers.png" alt="O OS AgÃªntico: seis camadas construÃ­das de baixo para cima, Identidade, depois Substrato, depois Regras, depois Skills, depois Ferramentas, depois Agentes" width="100%">
</p>

> Seis camadas, construÃ­das de baixo para cima. A Identidade Ã© a fundaÃ§Ã£o, o Substrato (os bastidores) Ã© a maior camada, e os Agentes ficam no topo, sÃ³ depois que tudo abaixo deles estÃ¡ firme.

---

## O que ela faz

VocÃª roda `/os-coach` dentro de qualquer pasta e diz qual Ã© o seu objetivo. A skill:

1. **Inicia um OS de verdade** naquela pasta, registra o seu objetivo com as suas prÃ³prias palavras, e lembra exatamente onde vocÃª estÃ¡ entre as sessÃµes, num arquivo `memory.md`.
2. **Treina uma camada de cada vez.** Faz 2 ou 3 perguntas em portuguÃªs simples, espera a sua resposta, entÃ£o constrÃ³i os arquivos e pastas de verdade para vocÃª e explica o que criou e por quÃª.
3. **Nunca fala como um manual.** Sem jargÃ£o. Quando uma palavra tÃ©cnica Ã© inevitÃ¡vel, ela ganha uma frase curta e uma analogia do dia a dia. Ela assume que vocÃª nunca abriu um terminal na vida.
4. **Se recusa a ser genÃ©rica.** Toda sugestÃ£o Ã© ancorada no seu objetivo real e no que de fato estÃ¡ na sua pasta agora, nÃ£o em conselho de manual.
5. **Audita quando vocÃª pedir.** PeÃ§a uma avaliaÃ§Ã£o e ela pontua todas as seis camadas em relaÃ§Ã£o ao seu objetivo, te dÃ¡ os trÃªs prÃ³ximos movimentos de maior alavancagem em ordem de prioridade, e escreve o relatÃ³rio em `OS-AUDIT.md`.
6. **Protege o que vocÃª marca como sensÃ­vel.** Se vocÃª marca um campo como privado, ela nunca escreve aquele valor na pasta; guarda no lugar uma referÃªncia que nÃ£o te identifica.

---

## As seis camadas

Ela constrÃ³i e audita as camadas na ordem que realmente funciona.

| # | Camada | O que Ã© | Mora em |
|---|---|---|---|
| 1 | **Identidade** | A alma. Quem Ã© este OS, quem ele serve, do que ele se recusa a fazer. | `CLAUDE.md` |
| 2 | **Substrato / Contexto** | Os bastidores. O conhecimento destilado em que o OS roda. A maior camada. | `substrate/` |
| 3 | **Regras & Hooks** | As cercas. RestriÃ§Ãµes preto-no-branco e reflexos automÃ¡ticos. | `rules/` |
| 4 | **Skills** | Os verbos conquistados. Tarefas repetÃ­veis empacotadas para rodar igual toda vez. | `skills/` |
| 5 | **Ferramentas / ConexÃµes** | Os fios para fora. ConexÃµes somente-leitura e bem delimitadas a fontes de dados reais. | `tools.md` |
| 6 | **Agentes** | PapÃ©is com julgamento que orquestram as skills. | `agents/` |

---

## Como uma sessÃ£o flui

VocÃª dÃ¡ sempre sÃ³ um pequeno passo por vez. O treinador faz 2 ou 3 perguntas em portuguÃªs claro, constrÃ³i os arquivos de verdade quando vocÃª responde, anota onde vocÃª estÃ¡, e te aponta a prÃ³xima camada. Tudo lÃª e escreve num mesmo `memory.md`, entÃ£o ele sempre sabe de onde vocÃª parou, mesmo sessÃµes depois. PeÃ§a uma auditoria a qualquer momento e ele pontua o OS inteiro em relaÃ§Ã£o ao seu objetivo e devolve o resultado para dentro do ciclo.

<p align="center">
  <img src="assets/coach-loop.png" alt="O loop de treino: perguntar, construir, persistir, prÃ³ximo, todos lendo e escrevendo no memory.md, com a auditoria realimentando o ciclo" width="100%">
</p>

1. **Pergunta** algumas perguntas simples sobre a camada atual, entÃ£o para e espera.
2. **ConstrÃ³i** o arquivo ou pasta de verdade daquela camada quando vocÃª responde, sob medida para o seu objetivo.
3. **Persiste** a decisÃ£o e o seu lugar em `memory.md`, para que nada se perca entre os turnos.
4. **PrÃ³ximo**, segue para a camada de baixo ou de cima conforme a ordem de construÃ§Ã£o mandar.
5. **Audita** quando vocÃª pede, pontuando cada camada em relaÃ§Ã£o ao seu objetivo e escrevendo `OS-AUDIT.md`, que realimenta os prÃ³ximos movimentos.

---

## Novidades de outubro de 2026

As seis camadas sÃ£o as mesmas. O treino e a auditoria passaram a cobrar o que o ecossistema INEMA aprendeu desde junho:

- **Identidade portÃ¡til e que aprende:** `AGENTS.md` para o Codex e outros agentes lerem o mesmo OS, e as seÃ§Ãµes `## Self-learning` + `## Lessons` no `CLAUDE.md` (cada correÃ§Ã£o vira regra de uma linha).
- **Substrato que atravessa sessÃµes:** `context/current-state.md`, `tasks/current.md` e `handoffs/latest.md` (com cÃ³pia datada em `handoffs/history/`).
- **Regras com nÃ­vel de permissÃ£o e registro de falhas:** N0 (sÃ³ conversa) atÃ© N4 (age sozinho, sem aviso), e um `FALHAS.md` com uma linha por erro; o erro que repete vira regra fixa ou gancho.
- **Skills, Tools e Agentes:** gatilho claro em cada skill, nÃ­vel de permissÃ£o em cada conexÃ£o, modelo escolhido num arquivo sÃ³, e um segundo revisor antes do que Ã© importante sair.
- **Opcional, depois dos Agentes:** uma pasta `longrun/` com objetivo e prova de pronto para o OS trabalhar horas sozinho ([kit ExecuÃ§Ã£o Longa](https://inematds.github.io/execucao-longa/guia/)).

Curso completo com todos esses pontos: [Engenharia de Sistemas Operacionais de IA (AIOS)](https://inematds.github.io/oscoach/).

---

## Comandos

```
/os-coach start <seu objetivo>   ComeÃ§a um OS novinho em folha
/os-coach next                   Vai para a prÃ³xima camada nÃ£o terminada e treina ela
/os-coach layer <nome>           Pula para uma camada especÃ­fica (identity, substrate, rules, skills, tools, agents)
/os-coach status                 Mostra o mapa de progresso a partir da memÃ³ria
/os-coach audit                  Pontua o OS inteiro em relaÃ§Ã£o ao seu objetivo e te dÃ¡ os prÃ³ximos passos
/os-coach help                   Explica o que ela faz e mostra os comandos
```

---

## InstalaÃ§Ã£o

```bash
cp -r os-coach ~/.claude/skills/
```

Depois, dentro de qualquer pasta que vocÃª queira transformar num OS:

```
/os-coach start Quero nunca mais perder o prazo de um cliente
```

### PrÃ©-requisitos

- [Claude Code](https://claude.com/claude-code) instalado
- Ã‰ sÃ³ isso. Sem dependÃªncias, sem chaves de API, sem etapa de build.

---

## O que ela cria

Tudo aparece na pasta em que vocÃª a roda, entÃ£o a pasta *Ã©* o OS:

- `memory.md`, o estado corrente, para o treinador sempre saber de onde vocÃª parou.
- `CLAUDE.md`, a sua camada de Identidade, o arquivo-alma enxuto que o OS inteiro lÃª primeiro.
- `substrate/sources.md` e `substrate/compendium.md`, os bastidores.
- `rules/always.md` e `rules/never.md`, as suas cercas.
- `skills/<nome>/SKILL.md`, a sua primeira tarefa repetÃ­vel.
- `tools.md`, as conexÃµes somente-leitura de que o seu objetivo precisa.
- `agents/<nome>/AGENT.md`, o primeiro papel que vale promover, uma vez que as skills existam.
- `OS-AUDIT.md`, um boletim guardÃ¡vel sempre que vocÃª roda uma auditoria.

---

## Um exemplo de verdade

Aqui estÃ¡ uma execuÃ§Ã£o real, condensada. Uma fotÃ³grafa de casamento autÃ´noma quer parar de perder prazos. Os clientes aparecem como `Casal A`, `Casal B` porque a fotÃ³grafa marcou os nomes dos clientes como sensÃ­veis, entÃ£o o treinador guarda referÃªncias que nÃ£o identificam em vez dos nomes reais.

**VocÃª:**

```
/os-coach start Eu vivo perdendo prazos de cliente e quero nunca mais atrasar uma entrega
```

O OS Coach confirma o objetivo, prepara a pasta, e faz trÃªs perguntas curtas: para quem isto Ã©, a Ãºnica pergunta que vocÃª gostaria de poder simplesmente fazer a ele, e uma coisa que ele deve sempre fazer mais uma que ele nunca deve fazer. VocÃª responde: sÃ³ eu; "o que vence nos prÃ³ximos 10 dias e do que eu jÃ¡ estou atrasada"; sempre me avise dentro de 3 dias de uma data contratada; nunca mande mensagem para um cliente sem a minha aprovaÃ§Ã£o. Ele entÃ£o escreve o seu arquivo de Identidade:

```markdown
# Quem eu sou
Eu sou o sistema operacional de uma fotÃ³grafa de casamento autÃ´noma. Eu existo para que nenhuma entrega de cliente atrase nunca.
...
## Recusas inegociÃ¡veis (nunca)
- Eu nunca mando mensagem para um cliente sem vocÃª ler e aprovar antes.
- Eu nunca deixo um prazo passar em silÃªncio. Se algo estÃ¡ em risco, eu levanto a bandeira alto.
```

**VocÃª:** `/os-coach next`

Ele abre o Substrato, pergunta onde moram os seus agendamentos e o que Ã© sensÃ­vel, entÃ£o constrÃ³i um rastreador que calcula os dois prazos a partir da data de cada casamento (a prÃ©via Ã© casamento mais 1 semana, a galeria completa Ã© casamento mais 6 semanas) e responde a sua pergunta na hora:

```
Dentro de 3 dias, a sua linha de sempre-avisar acabou de disparar:
- Casal B, galeria completa vence em 2026-07-01 (faltam 3 dias)

Vencendo dentro de 10 dias:
- Casal C, prÃ©via vence em 2026-07-02 (faltam 4 dias)
```

**VocÃª:** `/os-coach audit`

```
## Boletim
| Camada     | Nota        | Por quÃª |
|------------|-------------|---------|
| Identidade | SÃ³lida      | O CLAUDE.md declara a missÃ£o e duas recusas. |
| Substrato  | Iniciada    | O rastreador responde "vence em breve" mas ainda nÃ£o "jÃ¡ estÃ¡ atrasado" atÃ© vocÃª marcar o que foi entregue. |
| Regras     | Faltando    | As referÃªncias dos clientes agora moram na pasta sem nada impedir um backup pÃºblico. |

## Os trÃªs movimentos que mais importam
1. Regras: escreva rules/never.md (nunca faÃ§a backup pÃºblico desta pasta). Um vazamento nÃ£o tem como desfazer, e uma galeria vence em 3 dias.
2. Substrato: marque quais galerias foram entregues para que "vence em breve" tambÃ©m consiga responder "jÃ¡ estÃ¡ atrasado".
3. Skills: transforme a checagem de prazo em um comando repetÃ­vel.
```

Sua pasta agora se parece com isto:

```
photo-os/
  CLAUDE.md          # Identidade, a alma
  memory.md          # de onde vocÃª parou
  substrate/
    sources.md       # onde os dados reais moram
    compendium.md    # o rastreador de prazos
  OS-AUDIT.md        # o boletim mais recente
```

Cada arquivo Ã© real, ancorado no seu objetivo, e seu para guardar.

---

## Como ela Ã© construÃ­da

- `SKILL.md`, o controlador. Ã‰ invocada sÃ³ pelo usuÃ¡rio, guarda as regras de ouro (fale como gente, um pequeno passo por vez, quem constrÃ³i Ã© vocÃª, nunca seja genÃ©rica, sempre persista, proteja dados sensÃ­veis, sem travessÃµes), as guardas, e a lÃ³gica de cada fluxo.
- `references/layer-playbook.md`, o detalhe de treino de cada camada: uma explicaÃ§Ã£o em portuguÃªs claro, uma analogia, as 2 ou 3 perguntas a fazer, o artefato a construir, e a checagem de pronto.
- `references/audit-rubric.md`, como pontuar cada camada (Faltando, Iniciada, SÃ³lida, Compondo), o teste de nÃ£o-genÃ©rico, a precedÃªncia de priorizaÃ§Ã£o, e as checagens de campo sensÃ­vel e de escrita de volta.

As referÃªncias sÃ£o carregadas sÃ³ quando necessÃ¡rio, entÃ£o o controlador fica enxuto.

---

## OS Coach Ã— OpenClaw: vocÃª constrÃ³i a base, ele roda o agente

O OS Coach **nÃ£o executa** tarefas por vocÃª no dia a dia. Ele **estrutura a fundaÃ§Ã£o**: Identidade, Substrato, Regras, Skills, Ferramentas e Agentes, a arquitetura sobre a qual um agente confiÃ¡vel consegue rodar. **Primeiro vocÃª constrÃ³i a base; sÃ³ depois um agente entra em execuÃ§Ã£o em cima dela.**

Ã‰ aÃ­ que entra uma plataforma de execuÃ§Ã£o como o **OpenClaw** (o "Jarvis" que roda os agentes): ela pega a base que vocÃª preparou aqui e a coloca para trabalhar, mensagens (WhatsApp, Telegram, e-mail), automaÃ§Ãµes, ferramentas e dashboards. **O OS Coach prepara a base; o OpenClaw roda o agente.**

<p align="center">
  <img src="assets/os-coach-vs-openclaw.png" alt="OS Coach versus OpenClaw: Ã  esquerda o OS Coach constrÃ³i a base (arquitetura, lÃ³gica e estrutura: Identidade, Contexto, Regras, Skills, Tools, Agentes, formando o Agentic OS); Ã  direita o OpenClaw roda o agente em execuÃ§Ã£o (mensagens, automaÃ§Ãµes, ferramentas e dashboards, monitorando, tomando aÃ§Ãµes, aprendendo e entregando resultados)" width="100%">
</p>

> **VocÃª constrÃ³i a base. Ele roda o agente.** O erro nÂº 1 Ã© pular direto para a execuÃ§Ã£o sem fundaÃ§Ã£o, e Ã© por isso que o OS Coach vem primeiro.

---

## Perguntas frequentes

**Eu preciso saber programar?**
NÃ£o. O treinador faz todo o trabalho tÃ©cnico, ele cria os arquivos e pastas para vocÃª. VocÃª sÃ³ responde perguntas em portuguÃªs claro e toma as decisÃµes. Ele assume que vocÃª nunca abriu um terminal.

**Meus dados saem da minha mÃ¡quina?**
NÃ£o. Tudo o que ele constrÃ³i sÃ£o arquivos comuns na pasta em que vocÃª o rodou. A camada de Ferramentas conecta Ã s suas fontes em modo somente-leitura e mantÃ©m segredos (senhas, chaves) fora da pasta. Se vocÃª marca um campo como sensÃ­vel, o treinador guarda uma referÃªncia que nÃ£o te identifica em vez do valor real, e nunca escreve um arquivo que diz excluir um campo e entÃ£o o inclui.

**Quanto custa ou o que exige?**
SÃ³ o Claude Code. Sem chaves de API, sem dependÃªncias, sem etapa de build. VocÃª roda `/os-coach` e vai.

**E se uma camada ainda nÃ£o se aplica a mim?**
O treinador a marca como `nÃ£o iniciada` com um motivo de uma linha, em vez de inventar trabalho para inglÃªs ver, e segue em frente. VocÃª nunca Ã© empurrado a construir um agente antes de existirem as skills que ele orquestraria.

**Em que isso difere de sÃ³ escrever um `CLAUDE.md`?**
Um `CLAUDE.md` Ã© apenas a camada de Identidade. O OS Coach constrÃ³i todas as seis camadas, mantÃ©m elas coerentes, e as audita em relaÃ§Ã£o ao seu objetivo ao longo do tempo. A Identidade Ã© a alma, mas o substrato, as regras, as skills, as ferramentas e os agentes sÃ£o o que fazem o OS de fato trabalhar.

**Isso Ã© sÃ³ para empresas?**
NÃ£o. Qualquer objetivo com bastidores funciona: uma prÃ¡tica de pesquisa, uma busca por emprego, uma casa, um pipeline criativo. Se vocÃª tem conhecimento espalhado e uma coisa que gostaria de poder simplesmente perguntar, serve.

**Onde ele guarda de onde eu parei?**
No `memory.md` da sua pasta. Toda execuÃ§Ã£o o lÃª primeiro e o atualiza por Ãºltimo, entÃ£o vocÃª pode parar no meio de uma construÃ§Ã£o e retomar depois, mesmo numa sessÃ£o nova, sem perder o seu lugar.

**Posso editar o que ele constrÃ³i?**
Pode, e deve. Os arquivos sÃ£o seus. Edite-os direto, entÃ£o rode `/os-coach audit` para ver como as suas mudanÃ§as pontuam em relaÃ§Ã£o ao seu objetivo.

---

Projeto adaptado da comunidade INEMA TDS - Marca Arckhe