# <a name="use-the-activity-feed-rest-api"></a>Use a API REST de feed de atividade

Você pode usar a API de feed no Microsoft Graph de atividade para retomar actiity de um usuário em plataformas e dispositivos. Solicitações de API de feed de atividade são realizadas em nome de um usuário por meio de [permissões delegadas](../../../concepts/permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions) e a [permissão de atividade do usuário](../../../concepts/permissions_reference.md), que pode ser usado com contas pessoais ou comercial e escola. 

As atividades do usuário são representadas pelo recurso de [atividade](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_activity) e são organizadas em um feed baseadas em tempo representada pela coleção me / atividades. 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>O que torna uma atividade do usuário excelente?

As atividades do usuário não apenas início apps — eles são links profundos em conteúdo específico em seu aplicativo. As atividades do usuário que você criar só não pode ser usadas em seu próprio aplicativo, mas também aparecem na Cortana e a linha do tempo do Windows — orientando mais reengagement de aplicativo e tornando mais fácil para os usuários continuar a usar seu aplicativo em vários dispositivos.  

### <a name="what-should-become-an-activity"></a>O que deve se tornar uma atividade? 

Como cada aplicativo é diferente, ele é entender a melhor maneira de mapear ações dentro de seu aplicativo para as atividades do usuário de cada desenvolvedor app. Por exemplo, jogos puderem criar uma atividade para cada campanha, documentos de criação de aplicativos podem criar uma atividade para cada documento exclusivo e aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho. 

Conforme você define activitites no seu aplicativo, aplique as seguintes diretrizes:

**Faça:** Registre uma única atividade para um grupo de ações do usuário relacionados. Se seu aplicativo é usado para uma sequência de conteúdos relacionados, provavelmente faz sentido para registrar uma única atividade da sessão inteira do compromisso.  

*Cenários de lista de reprodução:* Isso é especialmente relevante para listas de reprodução de música ou programas de TV — uma atividade do usuário único pode ser atualizada para mostrar seu progresso. Nesse caso, você terá uma atividade do usuário único com vários [itens do histórico](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_historyitem) que representam os períodos de compromisso em vários dias ou semanas.  

**Faça:** Armazenar dados de usuário para a nuvem. Se você deseja oferecer suporte às atividades de referência cruzada de dispositivo, será necessário certificar-se de que o conteúdo necessário para esta atividade retome o contato está armazenado em um local de nuvem. Por exemplo, se você publicar uma atividade sempre que um usuário edita um documento, o documento deve ser armazenado na nuvem em vez de localmente no dispositivo do usuário para permitir que reengagement entre dispositivos.  

**Não:** Crie uma atividade do usuário para ações que os usuários não precisam para retomar no futuro. Se seu aplicativo for usado para concluir as operações únicas e simples, que não persiste de status para rastrear no futuro, você provavelmente não precisará gravar uma atividade do usuário. 

Para ser claro, embora as atividades do usuário aparecem na linha de tempo do Windows, isso não foi criado como uma ferramenta de controle de versão — escolher uma atividade baseados em documentos sempre deve mostrar a versão mais recente desse documento (incluindo alterações feitas por outro usuário).

**Não:** Crie uma atividade do usuário para Ações concluídas por *outros usuários*. Se alguém lhe envia ao usuário uma mensagem ou @mentions usuário dentro de seu aplicativo, você não deve escrever uma nova atividade. Essas interações são atendidas por meio da exibição de notificações.  

*Cenários de colaboração:* Se várias pessoas estão trabalhando na mesma atividade (por exemplo, um documento do Word), haverá casos quando outro usuário fez alterações ao documento depois que você fez a última edição. Nesse caso, os desenvolvedores de aplicativos talvez queira atualizar os elementos visuais na atividade para refletir as alterações feitas no documento. Para fazer isso, o aplicativo pode atualizar a atividade existente sem criar um novo item de histórico. 

>**Observação:** Se você estiver publicando atividades para um aplicativo web, é importante incluir ambos um `activationURL` e um `fallbackURL` para cada uma das suas atividades. As atividades iniciará o usuário volta para seu aplicativo conforme o esperado com experiências Microsoft como linha de tempo do Windows. 

## <a name="app-interaction-patterns-and-user-activities"></a>Padrões de interação do aplicativo e as atividades do usuário 
As atividades do usuário que você criar irá variar com base no padrão de interação do seu aplicativo. Enquanto todos os aplicativos são diferentes, a maioria se encaixam em uma das seguintes padrões de interação: 

* **Aplicativos baseados no documento** — criar uma atividade por documento com um ou mais registros de histórico refletindo os períodos de uso. É importante atualizar seu cartão de atividade, como as alterações são feitas ao documento. 
* **Aplicativos de reprodução de mídia** — criar uma atividade por um agrupamento lógico de conteúdo como o conteúdo de uma lista de reprodução, programa ou autônomo. 
* **Jogos** — criar uma atividade para cada salvo jogo ou no mundo. Se seu jogo suporta apenas uma única sequência dos níveis, você pode escrever a mesma atividade ao longo do tempo, embora talvez você queira atualizar seu cartão para mostrar seu progresso ou realizações a mais recente. 
* **Utilitário apps** — se não há nada dentro de seu aplicativo que os usuários desejam continuar, você não deve publicar atividades. Um bom exemplo é um aplicativo simple de finalidade única como calculadora. 
* **Aplicativos de linha de negócios** — muitos aplicativos existirem para gerenciar tarefas simples ou os fluxos de trabalho. Crie uma atividade para cada fluxo de trabalho separado, acessada por meio do seu aplicativo. Por exemplo, cada relatório de despesas seria uma atividade separada, pois talvez você queira clique em que a atividade para ver se ela foi aprovada.

*Alguns aplicativos complexos incluem vários padrões de interação. Talvez você queira siga os padrões de criação de atividade de usuário diferente para diferentes cenários manipulados pelo seu aplicativo.*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>Próximas etapas

- Consulte o [recurso de atividade](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_activity) e definir atividades do seu aplicativo para ajudar os usuários a retomar tarefas importantes.
- Explore as amostras de [amostras de cartão adaptável](https://adaptivecards.io/samples/) para ideias tornar suas atividades **pop**.  
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

**Procurando mais ideias?** 

- Veja [como o Microsoft experiências estão usando atividades](https://channel9.msdn.com/events/Build/2017/B8108).
- Saiba mais sobre [a atividade feed API e pegue onde posso parou](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011).
