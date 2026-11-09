# Movune — Rodada 1 de validação com usuários

## Propósito e limites

Este guia orienta sessões moderadas de aproximadamente **45 minutos** para validar a compreensibilidade dos principais fluxos do protótipo Movune com profissionais e responsáveis operacionais de clínicas de Fisioterapia e Pilates.

Use exclusivamente os dados sintéticos já disponíveis no protótipo. O protótipo serve para validar decisões de fluxo, linguagem e interface; ele não representa um produto em produção, não armazena dados reais e não comprova regras de autorização, persistência, pagamento, consumo, prontuário ou integração externa.

Não peça à pessoa participante que conclua ações que alterem o cenário sintético. Quando uma tarefa chegar a uma confirmação final, interrompa antes dela e siga para as perguntas de acompanhamento.

## Objetivo da rodada

Entender se pessoas que operam a rotina de uma clínica conseguem:

- orientar-se entre Agenda, Clientes e Financeiro sem perder o contexto de clínica/unidade;
- distinguir um atendimento individual de Fisioterapia de uma turma coletiva de Pilates;
- entender conflitos, limites de frequência, capacidade e lista de espera sem presumir consequências não informadas;
- localizar e interpretar informações financeiras sem confundi-las com presença, evolução clínica ou consumo de sessão/crédito;
- reconhecer o que pode fazer, o que está bloqueado e por quê.

## Hipóteses a validar

| ID | Hipótese |
| --- | --- |
| H1 | A Agenda permite localizar uma ocorrência e compreender data, horário, responsável, sala, modalidade e estado sem orientação do moderador. |
| H2 | No agendamento individual, a pessoa compreende a diferença entre pagamento pendente, disponibilidade de plano e bloqueio por frequência já alocada. |
| H3 | A pessoa reconhece Pilates como uma ocorrência coletiva, entende a capacidade `4 de 4` e não espera criação automática de uma vaga ou promoção automática da lista de espera. |
| H4 | A pessoa encontra o contexto financeiro de uma cliente e distingue plano ativo, vencimento, pagamento pendente/registrado, renovação e reativação. |
| H5 | A pessoa consegue localizar um lançamento na área Financeiro e entende que seus detalhes não mudam o contexto da cliente. |
| H6 | Estados, avisos, badges e controles são compreendidos por texto e estrutura, não apenas por cor. |

## Perfil recomendado

Recrutar de 5 a 7 pessoas, priorizando diversidade de responsabilidades:

- fisioterapeutas que também organizam a própria agenda;
- profissionais de Pilates que organizam turmas e participantes;
- recepcionistas ou secretárias responsáveis por agenda, cadastro e pagamentos;
- responsáveis operacionais ou administrativos de clínicas pequenas e médias.

Incluir, quando possível, pessoas com níveis diferentes de familiaridade com sistemas de gestão. Não é necessário conhecimento prévio de Movune. Evitar participantes que tenham participado diretamente das decisões de interface do protótipo.

## Preparação da sessão

1. Abrir a versão local do protótipo no cenário inicial e confirmar que os dados são sintéticos.
2. Usar uma janela limpa, em desktop ou dispositivo móvel conforme o perfil da sessão. Anotar tamanho de tela e tema utilizados.
3. Não explicar previamente onde ficam os recursos nem como executar as tarefas.
4. Não concluir criação de agendamento, pagamento, plano, interesse em espera ou qualquer ação que altere o estado sintético. Se for necessário testar uma confirmação em sessão futura, preparar um ambiente resetável e obter autorização explícita.
5. Registrar observações durante a sessão sem interromper a pessoa; pedir esclarecimento somente após a tarefa ou quando ela declarar que terminou.

## Roteiro moderado — 45 minutos

| Etapa | Tempo | Objetivo |
| --- | ---: | --- |
| Abertura e contexto | 5 min | Alinhar propósito, consentimento e expectativas. |
| Aquecimento e orientação | 3 min | Observar leitura inicial da interface e contexto de clínica/unidade. |
| Tarefa 1 — Agenda e atendimento individual | 8 min | Validar descoberta, leitura e contexto da ocorrência. |
| Tarefa 2 — Novo agendamento e limite de frequência | 8 min | Validar bloqueio, linguagem e preservação do rascunho. |
| Tarefa 3 — Turma Pilates lotada e espera | 8 min | Validar modelo coletivo, capacidade e decisão humana. |
| Tarefa 4 — Financeiro no contexto da cliente | 6 min | Validar entendimento de plano e pendência. |
| Tarefa 5 — Área Financeiro e lançamento | 4 min | Validar localização e detalhes de lançamento. |
| Encerramento | 3 min | Recolher percepção geral e prioridades. |

## Abertura, consentimento e contextualização

### Texto sugerido para o moderador

> Obrigado por participar. Vamos avaliar um protótipo do Movune para a operação de clínicas de Fisioterapia e Pilates. Estamos testando a clareza da interface e dos fluxos, não o seu desempenho. Não há respostas certas ou erradas.
>
> O que você verá usa apenas dados fictícios e não é um sistema em produção. Algumas ações serão interrompidas antes da confirmação para não alterar o cenário de demonstração. Enquanto realiza as tarefas, por favor diga em voz alta o que espera encontrar e o que está tentando fazer.
>
> Com sua autorização, vamos registrar anotações sobre a sessão. Não usaremos informações pessoais ou dados reais de pacientes. Você pode pular qualquer pergunta ou encerrar a sessão a qualquer momento. Podemos começar?

Registrar consentimento: **[ ] Sim  [ ] Não**. Se não houver consentimento, encerrar a sessão.

### Aquecimento

**Instrução:** “Sem clicar ainda, o que você entende que está vendo? Como identificaria a clínica ou unidade em que está trabalhando?”

Observar: leitura do cabeçalho, compreensão da navegação e quaisquer termos confusos.

## Tarefas e perguntas de acompanhamento

### Tarefa 1 — Localizar e compreender um atendimento individual

**Cenário para ler:**

> Você recebeu uma dúvida sobre o atendimento de Fisioterapia de Ana Souza no meio da semana. Encontre esse atendimento e me diga o que você entende sobre ele antes de realizar qualquer alteração.

**Critérios de conclusão:** a pessoa abre o detalhe da ocorrência e localiza cliente, data/hora, profissional, sala, modalidade e estado da ocorrência. Se quiser, pode abrir o contexto da cliente; não deve alterar dados.

**Não ensinar:** não indicar a aba, o dia, o card ou o botão de detalhes.

**Perguntas neutras após a tarefa:**

- “O que nesta tela fez você confiar — ou desconfiar — de que era o atendimento correto?”
- “Como você descreveria a diferença entre o estado do agendamento e o estado da cliente?”
- “Se precisasse consultar algo mais sobre essa pessoa, para onde iria em seguida?”

**Observar:** busca de informação, leitura de estados, uso do drawer, retorno ao contexto anterior, troca ou perda de identidade/ocorrência.

### Tarefa 2 — Revisar um novo atendimento com limite de frequência

**Cenário para ler:**

> Você precisa tentar organizar um novo atendimento de Fisioterapia para Ana Souza no período disponível. Siga até o ponto em que você decidiria revisar ou confirmar o agendamento. Pare antes de confirmar qualquer coisa e me diga o que a interface permite e o que impede.

**Cenário sintético esperado:** o Plano Movimento de Ana Souza está com a frequência integralmente alocada no período relevante.

**Critérios de conclusão:** a pessoa encontra o fluxo de novo agendamento, seleciona Ana Souza e identifica o aviso de frequência totalmente alocada e a indisponibilidade de avançar para revisão/confirmação.

**Limite do moderador:** não sugerir atendimento avulso, cobrança adicional, expansão de plano, exceção ou qualquer consequência posterior. Essas consequências não são definidas por este cenário.

**Perguntas neutras após a tarefa:**

- “O que você entende que bloqueou o próximo passo?”
- “Como você diferencia essa mensagem de uma pendência de pagamento?”
- “O que você esperaria poder fazer a seguir?”
- “Há algo aqui que parece uma regra da clínica, uma informação financeira ou uma consequência de sessão? Por quê?”

**Observar:** compreensão do bloqueio, leitura de pagamento pendente sem inferir bloqueio financeiro, tentativas de contorno, expectativa de ação posterior e preservação dos dados preenchidos.

### Tarefa 3 — Avaliar uma turma de Pilates lotada e a lista de espera

**Cenário para ler:**

> Uma pessoa quer participar da turma de Pilates de 17 de setembro, às 10h30. Verifique se há vaga e explique o que você faria com esse interesse. Não confirme nenhuma ação.

**Cenário sintético esperado:** a turma tem `4 de 4 participantes` e interessados em lista de espera.

**Critérios de conclusão:** a pessoa identifica uma única ocorrência coletiva, vê capacidade, participantes e estados individuais, localiza os interessados e entende que aguardam revisão humana.

**Perguntas neutras após a tarefa:**

- “Como você entendeu se esta é uma turma ou atendimentos individuais?”
- “O que acontece com a pessoa interessada neste momento?”
- “Se uma vaga surgir, o que você espera que ocorra?”
- “Que informação faltaria para você tomar uma decisão manual com segurança?”

**Observar:** se a pessoa espera promoção automática, se confunde interessada com participante/reserva, compreensão de capacidade e leitura dos estados individuais.

### Tarefa 4 — Consultar a situação financeira da cliente

**Cenário para ler:**

> Agora, consulte a situação financeira de Ana Souza. Quero que você me diga qual plano está ativo, se há alguma pendência e onde você procuraria pagamentos anteriores. Não registre um pagamento.

**Critérios de conclusão:** a pessoa chega à aba Financeiro da mesma cliente, encontra plano ativo, vencimento, situação de pagamento e histórico pago/em aberto, quando permitido pelo cenário.

**Perguntas neutras após a tarefa:**

- “O que significa esse status de pagamento para você?”
- “Isso muda o atendimento, a presença ou o consumo de sessão? O que na tela orienta sua resposta?”
- “Onde você procuraria um pagamento já registrado?”
- “Como você diferencia Registrar pagamento de Renovar ou Reativar?”

**Observar:** entendimento de permissão financeira, separação entre pagamento e clínica/agenda, interpretação de vencimento, ação de registrar pagamento e ações de renovação/reativação quando visíveis.

### Tarefa 5 — Localizar um lançamento no Financeiro

**Cenário para ler:**

> Sem sair do contexto operacional, encontre no Financeiro um lançamento relacionado a uma cliente e veja os detalhes dele. Não faça nenhuma ação financeira.

**Critérios de conclusão:** a pessoa abre a área Financeiro, localiza um lançamento usando os controles disponíveis e abre os detalhes pelo ícone correspondente, sem confundir esse detalhe com o perfil da cliente.

**Perguntas neutras após a tarefa:**

- “Como você decidiu que este era o lançamento certo?”
- “O que você espera ver ao abrir os detalhes?”
- “Qual é a diferença entre abrir detalhes e abrir o contexto financeiro da cliente?”
- “Os filtros, período e total ajudam na sua conferência? O que mudaria?”

**Observar:** compreensão de período/filtros/totais, distinção entre detalhes do lançamento e atalho para a cliente, leitura de situação e categoria.

## Perguntas de encerramento

1. “Qual parte pareceu mais clara ou mais segura para usar?”
2. “Em que momento você teve mais dúvida sobre o que aconteceria depois?”
3. “Há algum termo, status ou ação que você nomearia de outra forma?”
4. “O que faria você confiar neste fluxo em uma rotina movimentada?”
5. “Se pudesse melhorar apenas uma coisa antes de testar novamente, qual seria?”
6. “Há alguma regra operacional importante que a interface pareceu assumir sem explicar?”

## Critérios de observação

Registrar evidência observável, não apenas impressão do moderador.

| Dimensão | O que registrar |
| --- | --- |
| Conclusão | Concluiu sem ajuda, com pista leve, com orientação direta ou não concluiu. |
| Caminho | Primeiro clique, desvios, retornos e uso de busca/filtros. |
| Erros | Clique em destino equivocado, ação esperada mas ausente, interpretação incorreta ou tentativa de confirmar indevidamente. |
| Hesitações | Pausas, releitura, perguntas, abandono de caminho e sinais de incerteza. |
| Compreensão de status | Como a pessoa explicou estados de ocorrência, cliente/participante, capacidade, espera, pagamento e frequência. |
| Confiança | Grau declarado de confiança e a evidência visual ou textual citada para justificar. |
| Linguagem da pessoa | Termos espontâneos usados para turma, vaga, interesse, pagamento, plano, sessão, bloqueio e cancelamento. |
| Acessibilidade e contexto | Dificuldades com leitura, tamanho, contraste, foco, toque, navegação, viewport ou perda de contexto. |

## Modelo de registro por participante

```markdown
# Sessão [código]

- Data/hora:
- Moderador:
- Plataforma e viewport:
- Tema/tamanho de texto:
- Perfil operacional:
- Familiaridade com sistemas de clínica:
- Consentimento registrado: sim / não

## Observação inicial

- Contexto de clínica/unidade compreendido?
- Comentários espontâneos:

## Tarefas

| Tarefa | Conclusão | Tempo | Ajuda necessária | Evidência observada | Compreensão declarada | Confiança (1–5) | Citação ou termo usado |
| --- | --- | ---: | --- | --- | --- | ---: | --- |
| 1. Atendimento individual |  |  |  |  |  |  |  |
| 2. Limite de frequência |  |  |  |  |  |  |  |
| 3. Turma lotada e espera |  |  |  |  |  |  |  |
| 4. Financeiro da cliente |  |  |  |  |  |  |  |
| 5. Lançamento financeiro |  |  |  |  |  |  |  |

## Problemas e oportunidades

| Achado | Evidência | Área | Severidade inicial | Hipótese afetada | Próximo passo sugerido |
| --- | --- | --- | --- | --- | --- |

## Encerramento

- Principal ponto claro:
- Principal dúvida:
- Mudança priorizada pela pessoa:
- Decisões de produto que precisam de esclarecimento:
```

## Síntese final da rodada

Após todas as sessões, consolidar evidências por padrão recorrente; não somar apenas opiniões isoladas.

| Achado consolidado | Participantes afetados | Evidência recorrente | Impacto no fluxo | Classificação | Recomendação | Dono/decisão |
| --- | ---: | --- | --- | --- | --- | --- |

Incluir também:

- hipóteses confirmadas, refutadas e inconclusivas;
- termos que as pessoas usaram espontaneamente e que diferem da interface;
- diferenças relevantes entre profissionais, recepção e responsáveis operacionais;
- comportamentos esperados que não são definidos pela documentação e exigem decisão de produto, em vez de correção de interface.

## Regra de priorização

Classificar o achado pela evidência e pelo impacto na tarefa — não pela preferência estética isolada.

| Classificação | Definição | Exemplo de encaminhamento |
| --- | --- | --- |
| **Falha bloqueadora** | Impede concluir uma tarefa essencial, induz ação operacional incorreta relevante ou impede entender uma restrição crítica. | Corrigir antes da próxima rodada ou retirar a tarefa da validação. |
| **Dificuldade importante** | A tarefa é concluída, mas exige ajuda, repetidas tentativas ou cria risco plausível de erro na rotina. | Corrigir ou redesenhar antes de ampliar a validação. |
| **Oportunidade de melhoria** | Não impede a tarefa, mas reduz velocidade, confiança, compreensão ou acessibilidade. | Agrupar com evidências semelhantes e priorizar no próximo ciclo. |
| **Decisão de produto em aberto** | A dificuldade decorre de consequência ou política ainda não definida nas fontes do produto; não deve ser resolvida por conveniência de interface. | Registrar a pergunta, os cenários observados e solicitar decisão de produto. |

## Salvaguardas para interpretação dos resultados

- Não concluir que pagamento pendente determina presença, consumo, conclusão de atendimento ou evolução clínica.
- Não concluir que abrir/liberar uma vaga determina a consequência de sessão/crédito ou reposição.
- Não tratar uma pessoa interessada na lista de espera como participante ou reserva confirmada.
- Não supor promoção automática de interessados quando surgir vaga.
- Não converter o bloqueio de frequência integralmente alocada em atendimento avulso, cobrança extra ou exceção automática.
- Não interpretar comportamentos simulados de permissão, arquivo ou pagamento como validação de segurança, persistência ou operação de produção.
