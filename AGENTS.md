
## 1. Missão do Vault

Este repositório contém um sistema pessoal de conhecimento construído no Obsidian.

O objetivo não é apenas organizar arquivos.

O objetivo é construir uma **rede de conhecimento navegável por humanos e inteligível por IAs**, preservando contexto, histórico, relações semânticas e evolução das ideias.

O vault possui principalmente estas áreas:

- Sonhos
    
- Psicologia analítica / Jung
    
- Trabalho
    
- Estudos
    
- Projetos
    
- Referências
    
- Conhecimento pessoal e contextual
    

A organização deve favorecer:

**contexto > categorização**

**relações > quantidade de tags**

**semântica > estética**

**preservação > reescrita**

---

# 2. Regras Absolutas

Antes de modificar qualquer arquivo:

1. Nunca apague informação.
    
2. Nunca invente informação.
    
3. Nunca altere o significado de uma anotação.
    
4. Nunca transforme uma hipótese em fato.
    
5. Nunca trate uma interpretação como certeza.
    
6. Nunca invente relações entre notas apenas para aumentar o Graph View.
    
7. Nunca duplique conteúdo que já existe.
    
8. Nunca faça uma grande reorganização sem primeiro explicar o plano.
    
9. Nunca renomeie ou mova dezenas de arquivos de uma vez sem apresentar a proposta.
    
10. Preserve datas, fontes e contexto histórico.
    
11. Preserve a linguagem pessoal quando ela carregar significado.
    
12. Não transforme registros pessoais em textos excessivamente formalizados.
    
13. Não remova detalhes apenas porque parecem irrelevantes.
    
14. Quando houver conflito entre duas notas, preserve ambas e sinalize o conflito.
    
15. Quando não houver informação suficiente para decidir algo, marque como dúvida em vez de inferir.
    

---

# 3. Filosofia de Organização

O vault deve funcionar como uma **Knowledge Graph**.

Pastas são úteis para navegação, mas não devem ser o principal mecanismo de organização.

Uma nota pode pertencer conceitualmente a vários contextos.

Exemplo:

Um conceito de Jung pode estar relacionado simultaneamente a:

- um livro;
    
- uma anotação de estudo;
    
- um sonho;
    
- um símbolo recorrente;
    
- uma reflexão pessoal.
    

Não devemos duplicar a informação em cinco lugares.

Devemos criar relações:

[[Arquétipo]]

[[Sombra]]

[[Sonho - 2026-09-13]]

[[O Livro Vermelho]]

---

# 4. Estrutura Conceitual

Sempre que possível, pensar no vault através destas camadas:

```text
MOC
 ↓
Conceitos
 ↓
Notas específicas
 ↓
Exemplos / registros
 ↓
Fontes
```

Exemplo:

```text
MOC - Jung
   ↓
Sombra
   ↓
Sombra e Persona
   ↓
Sonho - 2026-09-13
```

---

# 5. Tipos de Nota

Sempre que possível, identificar o tipo semântico de uma nota.

Tipos comuns:

- `dream`
    
- `concept`
    
- `person`
    
- `project`
    
- `study`
    
- `reference`
    
- `book`
    
- `work`
    
- `moc`
    
- `reflection`
    
- `journal`
    
- `symbol`
    
- `archetype`
    

Não adicionar `type` indiscriminadamente se isso não trouxer valor.

---

# 6. Frontmatter

Quando houver benefício real, utilizar YAML consistente.

Exemplo:

```yaml
---
type: dream
date: 2026-09-13
---
```

Para projetos:

```yaml
---
type: project
status: active
---
```

Para estudos:

```yaml
---
type: study
topic: ...
---
```

Não preencher campos com informações inventadas.

Não criar dezenas de propriedades apenas para padronização.

Metadata deve servir à recuperação, filtragem ou compreensão da informação.

---

# 7. Linking

Links Obsidian são fundamentais.

Preferir:

```markdown
[[Conceito]]
[[Projeto]]
[[Pessoa]]
[[Livro]]
[[Símbolo]]
```

em vez de depender excessivamente de tags.

## Criar um link quando:

- existe relação conceitual real;
    
- uma nota fornece contexto para outra;
    
- o conceito aparece de maneira significativa;
    
- a relação pode ajudar uma futura consulta humana ou de IA.
    

## Não criar um link quando:

- a palavra simplesmente aparece;
    
- a relação é trivial;
    
- o link deixaria a nota visualmente poluída;
    
- a relação é apenas uma coincidência lexical.
    

---

# 8. Links e Contexto para IA

Ao adicionar links, pensar:

> "Se uma IA encontrasse esta nota isoladamente, quais outras notas ela precisaria conhecer para compreender corretamente seu significado?"

Essas são as relações prioritárias.

Uma nota importante deve, quando apropriado, possuir:

- contexto;
    
- conceitos relacionados;
    
- fontes;
    
- projetos relacionados;
    
- registros relacionados;
    
- notas anteriores/posteriores.
    

---

# 9. MOCs

MOCs (Maps of Content) são notas de navegação.

Não devem simplesmente copiar o conteúdo das outras notas.

Um MOC deve responder:

- O que existe neste domínio?
    
- Quais são os conceitos principais?
    
- Quais notas são centrais?
    
- Quais relações existem?
    
- Por onde devo continuar estudando?
    

Exemplo:

```markdown
# MOC - Jung

## Conceitos fundamentais

- [[Inconsciente Coletivo]]
- [[Arquétipos]]
- [[Sombra]]
- [[Persona]]
- [[Self]]
- [[Anima]]
- [[Animus]]

## Sonhos relacionados

- [[Sonho - ...]]

## Estudos

- [[O Livro Vermelho]]
- [[Comentários sobre o Livro Vermelho]]

## Símbolos recorrentes

- [[Floresta]]
- [[Montanha]]
- [[Coruja]]
```

MOCs devem ser hubs, não depósitos de conteúdo duplicado.

---

# 10. SONHOS

Sonhos são registros históricos e subjetivos.

Eles possuem prioridade máxima de preservação.

Nunca:

- reescrever um sonho como se fosse uma narrativa literária;
    
- remover detalhes estranhos;
    
- corrigir acontecimentos;
    
- transformar interpretação em fato;
    
- inventar símbolos;
    
- inventar sentimentos;
    
- preencher lacunas da memória.
    

O relato original deve permanecer reconhecível.

---

## 10.1 Estrutura dos sonhos

Quando apropriado:

```markdown
# Sonho - DD-MM-YYYY

## Relato

[relato original]

## Pessoas

[[Pessoa]]

## Lugares

[[Lugar]]

## Elementos

[[Símbolo]]
[[Objeto]]
[[Animal]]

## Temas

[[Perseguição]]
[[Transformação]]
[[Ser observado]]

## Interpretação

[interpretação separada do relato]
```

Não adicionar seções que não tenham conteúdo.

---

# 11. SIMBOLOGIA DOS SONHOS

Ao analisar ou organizar símbolos:

Separar claramente:

### Observação

O que realmente apareceu no sonho.

### Associação pessoal

O que o próprio usuário associa ao símbolo.

### Contexto

Como o símbolo aparece em outros sonhos.

### Interpretação

Possíveis significados psicológicos/simbólicos.

### Hipótese

Uma interpretação ainda incerta.

Nunca apresentar uma interpretação como verdade objetiva.

---

# 12. SONHOS RECORRENTES

Quando um símbolo, cenário, personagem ou dinâmica aparece em vários sonhos:

Criar uma nota de conceito somente se existir material suficiente.

Exemplo:

```text
[[Montanha]]
[[Floresta]]
[[Ser observado]]
[[Carro]]
[[Transformação]]
```

A nota do símbolo deve apontar para os sonhos relevantes.

Não copiar os sonhos inteiros para dentro da nota do símbolo.

---

# 13. JUNG

O material relacionado a Jung deve preservar uma distinção clara entre:

1. conceitos de Jung;
    
2. interpretações de autores secundários;
    
3. interpretação pessoal;
    
4. aplicação aos sonhos;
    
5. hipóteses próprias.
    

Nunca atribuir uma ideia ao próprio Jung sem evidência na nota ou fonte correspondente.

Quando uma interpretação pessoal for adicionada, deixar claro que é uma interpretação.

Exemplo:

```markdown
## Conceito

[O que a teoria apresenta]

## Fonte

[[Livro / Autor]]

## Relações

[[Sombra]]
[[Persona]]

## Aplicação pessoal

[Como este conceito parece se relacionar com experiências ou sonhos]

## Hipótese

[Interpretação ainda não confirmada]
```

---

# 14. TRABALHO

As notas de trabalho devem funcionar como uma base de conhecimento técnico e contextual.

Possíveis áreas:

- crédito;
    
- produtos;
    
- processos;
    
- sistemas;
    
- arquitetura;
    
- backend;
    
- frontend;
    
- banco de dados;
    
- SQL;
    
- APIs;
    
- regras de negócio;
    
- conceitos bancários;
    
- aprendizados;
    
- problemas resolvidos;
    
- decisões técnicas.
    

Priorizar relações entre:

```text
Conceito de negócio
      ↓
Produto
      ↓
Regra de negócio
      ↓
Sistema
      ↓
Código
      ↓
Projeto
```

Quando uma nota técnica depender de um conceito de negócio, criar o link.

Exemplo:

```markdown
[[Recebíveis]]
[[Garantia de Recebíveis]]
[[Conta Garantida]]
[[Capital de Giro]]
```

Não registrar informações confidenciais, credenciais, tokens, senhas ou dados pessoais sensíveis.

---

# 15. ESTUDOS

Notas de estudo devem representar evolução do conhecimento.

Não transformar automaticamente anotações em artigos perfeitos.

É aceitável que uma nota contenha:

- dúvidas;
    
- hipóteses;
    
- exemplos;
    
- erros;
    
- descobertas;
    
- explicações próprias.
    

Quando um conceito for compreendido posteriormente, atualizar a nota sem apagar o histórico relevante.

Preferir:

```text
[[Conceito]]
```

e relações entre conceitos a criar uma nova nota para cada pequena anotação.

---

# 16. PROJETOS

Projetos devem funcionar como hubs.

Um projeto pode conectar:

```text
Projeto
├── Objetivo
├── Decisões
├── Tecnologias
├── Problemas
├── Soluções
├── Pessoas
├── Conceitos
└── Referências
```

Evitar colocar todo o conhecimento dentro da nota do projeto.

O projeto deve apontar para as notas que contêm o conhecimento.

---

# 17. Graph View

O Graph View deve representar **relações reais**, não apenas proximidade de arquivos.

Priorizar:

- hubs;
    
- conceitos centrais;
    
- MOCs;
    
- projetos;
    
- símbolos recorrentes;
    
- conexões entre áreas.
    

Uma boa rede pode ter muitas notas com poucas conexões e algumas notas centrais com muitas conexões.

Não tentar fazer todas as notas se conectarem.

---

# 18. Notas Órfãs

Uma nota órfã não deve ser automaticamente conectada a qualquer coisa.

Para cada órfã:

1. identificar seu significado;
    
2. procurar relações reais;
    
3. sugerir links;
    
4. conectar ao MOC apropriado quando existir;
    
5. somente depois considerar criação de um novo MOC.
    

Se não existir relação significativa, pode permanecer órfã.

---

# 19. Duplicatas

Antes de criar uma nota:

1. pesquisar notas semanticamente semelhantes;
    
2. verificar possíveis duplicatas;
    
3. determinar se a nova informação deve ser adicionada à nota existente;
    
4. somente criar uma nova nota quando houver justificativa.
    

Não mesclar automaticamente notas diferentes.

Se duas notas forem parecidas mas possuírem contextos diferentes, preservar ambas.

---

# 20. Tags

Tags devem ser utilizadas com moderação.

Preferir links para conceitos.

Tags podem representar propriedades amplas como:

```text
#trabalho
#estudo
#sonhos
#projeto
#referencia
```

Evitar:

```text
#montanha
#floresta
#coruja
#carro
#jung
#sombra
```

se esses elementos já forem representados adequadamente como notas e links.

---

# 21. Nomenclatura

Manter nomes consistentes.

Antes de renomear:

- verificar backlinks;
    
- verificar referências;
    
- verificar duplicatas;
    
- verificar se o nome atual possui significado histórico.
    

Não renomear simplesmente para "ficar bonito".

Se uma mudança de nomenclatura melhorar significativamente a navegação, apresentar a proposta antes de executar.

---

# 22. Pastas

Pastas são úteis para separar grandes domínios.

Não criar uma árvore extremamente profunda.

Preferir poucos níveis:

```text
/
├── Sonhos/
├── Jung/
├── Trabalho/
├── Estudos/
├── Projetos/
├── Referências/
└── MOCs/
```

A estrutura exata pode variar após auditoria do vault existente.

Nunca reorganizar todas as pastas sem uma análise prévia.

---

# 23. Preservação Histórica

As notas também representam a evolução do pensamento.

Não otimizar tudo para o estado atual.

Uma nota antiga pode conter uma compreensão incorreta que posteriormente foi corrigida.

Quando isso for relevante:

```markdown
## Evolução

[O que foi entendido anteriormente]

## Atualização

[O que mudou]

## Motivo

[Por que mudou]
```

O objetivo é preservar a trajetória do conhecimento.

---

# 24. Contexto para IA

Este vault será utilizado como contexto por modelos de IA.

Portanto, uma nota importante deve ser compreensível mesmo quando recuperada isoladamente.

Evitar referências ambíguas como:

> "isso aconteceu depois"

quando não estiver claro o que "isso" significa.

Preferir:

> "No sonho de 13/09/2026..."

Entretanto, não remover o estilo natural das notas pessoais apenas para satisfazer uma estrutura artificial.

---

# 25. Recuperação Semântica

Ao organizar o vault, pensar em como uma IA faria perguntas como:

- "Quais sonhos possuem o símbolo da floresta?"
    
- "Quais conceitos de Jung aparecem nos meus sonhos?"
    
- "Quais símbolos se repetem ao longo do tempo?"
    
- "Como minha interpretação de determinado símbolo mudou?"
    
- "Quais projetos usam determinada tecnologia?"
    
- "O que aprendi sobre determinado conceito no trabalho?"
    
- "Quais estudos se relacionam a este projeto?"
    
- "Quais conceitos aparecem em múltiplos domínios?"
    

Criar links e MOCs que tornem essas consultas possíveis.

---

# 26. Auditoria Antes de Alteração

Sempre que solicitado a "organizar o vault", executar primeiro uma auditoria.

A auditoria deve identificar:

### Estrutura

- pastas;
    
- tipos de nota;
    
- padrões de nomenclatura.
    

### Grafo

- hubs;
    
- clusters;
    
- órfãos;
    
- possíveis conexões ausentes.
    

### Conteúdo

- duplicatas;
    
- notas incompletas;
    
- conceitos recorrentes;
    
- assuntos centrais.
    

### Metadata

- padrões existentes;
    
- inconsistências;
    
- campos úteis.
    

### MOCs

- existentes;
    
- necessários;
    
- redundantes.
    

A auditoria NÃO deve modificar arquivos.

---

# 27. Processo de Mudança

Para alterações importantes, utilizar este processo:

```text
AUDITAR
   ↓
PROPOR
   ↓
APROVAR
   ↓
MODIFICAR
   ↓
VALIDAR
```

Antes de grandes alterações, apresentar:

```text
Arquivo atual
→ mudança proposta
→ motivo
→ impacto
```

Fazer alterações em pequenos grupos.

Depois de cada grupo, verificar backlinks e referências.

---

# 28. Git

Este repositório utiliza Git.

Antes de mudanças grandes:

- verificar estado atual;
    
- evitar sobrescrever alterações não relacionadas;
    
- fazer mudanças pequenas;
    
- manter commits logicamente separados quando possível.
    

Nunca executar operações destrutivas sem autorização explícita.

Não utilizar Git para apagar histórico como forma de "limpar" o vault.

---

# 29. Critério de Qualidade

Uma organização é considerada boa quando:

1. consigo encontrar uma informação rapidamente;
    
2. consigo descobrir informações relacionadas;
    
3. uma IA consegue recuperar contexto suficiente;
    
4. o Graph View revela clusters reais;
    
5. notas importantes possuem contexto;
    
6. o histórico pessoal não foi destruído;
    
7. existem poucas duplicações;
    
8. links possuem significado;
    
9. MOCs funcionam como mapas;
    
10. a estrutura continua simples o suficiente para ser mantida manualmente.
    

---

# 30. Regra Final

Não organize o vault apenas para parecer organizado.

Organize-o para **pensar melhor, recuperar conhecimento melhor e descobrir relações que antes estavam escondidas**.

O objetivo final é que:

```text
SONHOS
   ↕
JUNG
   ↕
REFLEXÕES
   ↕
ESTUDOS
   ↕
TRABALHO
   ↕
PROJETOS
```

possam coexistir como partes de uma mesma rede de conhecimento quando existir uma relação real entre elas.

O Graph View é uma consequência dessa estrutura.

Ele não é o objetivo.

A qualidade da rede de conhecimento é o objetivo.