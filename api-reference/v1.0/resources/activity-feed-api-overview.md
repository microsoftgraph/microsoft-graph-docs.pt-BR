# <a name="use-the-activity-feed-rest-api"></a>Usar a API REST de feed de atividades

Você pode usar a API de feed de atividades no Microsoft Graph para retomar uma atividade do usuário em vários dispositivos e plataformas. As solicitações da API de feed de atividades são realizadas em nome de um usuário por meio das [permissões delegadas](../../../concepts/permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions) e da [permissão de atividades do usuário](../../../concepts/permissions_reference.md), que podem ser usadas em contas pessoais ou comerciais e escolares. 

As atividades do usuário são representadas pelo recurso [activity](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity) e são organizadas em um feed baseado em tempo representado pela coleção me/activities. 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>O que torna uma atividade do usuário excelente?

As atividades do usuário não apenas iniciam os aplicativos, como também são links profundos ao conteúdo específico do seu aplicativo. As atividades do usuário que você criar não só podem ser usadas em seu próprio aplicativo, como também aparecem na Cortana e na Linha do Tempo do Windows, promovendo novos engajamentos com o aplicativo e facilitando para os usuários continuarem a usar seu aplicativo em vários dispositivos.  

### <a name="what-should-become-an-activity"></a>O que deve se tornar uma atividade? 

Como cada aplicativo é diferente, cabe a cada desenvolvedor de aplicativo entender a melhor maneira de mapear as ações de seu aplicativo às atividades do usuário. Por exemplo, jogos podem criar uma atividade para cada campanha, aplicativos de criação de documentos podem criar uma atividade para cada documento único e aplicativos de linha de negócios podem criar uma atividade para cada fluxo de trabalho. 

Conforme você define as atividades do seu aplicativo, aplique as seguintes diretrizes:

**FAÇA:** registre uma atividade para um grupo de ações do usuário relacionadas. Se seu aplicativo for usado para uma sequência de conteúdo relacionado, provavelmente fará sentido registrar uma única atividade para toda a sessão de engajamento.  

*Cenários de listas de reprodução:* isso é especialmente relevante para listas de reprodução de músicas ou programas de TV — uma única atividade do usuário pode ser atualizada para mostrar o progresso. Nesse caso, você terá uma única atividade do usuário com vários [itens de histórico](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_historyitem) representando os períodos de engajamento em vários dias ou semanas.  

**FAÇA:** armazene os dados dos usuários na nuvem. Se você deseja oferecer suporte a atividades em vários dispositivos, será necessário garantir que o conteúdo necessário para reengajar esta atividade esteja armazenado em um local na nuvem. Por exemplo, se você publicar uma atividade sempre que um usuário editar um documento, este deverá ser armazenado na nuvem e não localmente no dispositivo do usuário, de modo a permitir o reengajamento em vários dispositivos.  

**NÃO FAÇA:** crie uma atividade do usuário para ações que os usuários não precisam retomar no futuro. Se seu aplicativo for usado para concluir operações únicas e simples, cujo status não é persistido para acompanhar no futuro, você provavelmente não precisará criar uma atividade do usuário. 

Para ser claro, mesmo que as atividades do usuário apareçam na Linha do Tempo do Windows, ela não foi criada como uma ferramenta de controle de versão — escolher uma atividade baseada em documento sempre deve mostrar a última versão desse documento (incluindo as alterações feitas por outro usuário).

**NÃO FAÇA:** crie uma atividade do usuário para ações concluídas por *outros usuários*. Se alguém enviar uma mensagem ao usuário ou mencioná-lo usando "@" no seu aplicativo, você não deve criar uma nova atividade. Essas interações são melhor fornecidas por meio da exibição de notificações.  

*Cenários de colaboração:* se várias pessoas estiverem trabalhando em uma mesma atividade (por exemplo, um documento do Word), haverá casos em que outro usuário fará alterações no documento após sua última edição. Nesse caso, os desenvolvedores de aplicativos talvez queiram atualizar os elementos visuais na atividade para refletir as alterações feitas no documento. Para fazer isso, o aplicativo pode atualizar a atividade existente sem criar um novo item de histórico. 

>**Observação:** se você estiver publicando atividades para um aplicativo da Web, é importante incluir um `activationURL` e um `fallbackURL` para cada uma das atividades. As atividades retornarão o usuário ao seu aplicativo conforme o esperado das experiências da Microsoft como a Linha do Tempo do Windows. 

## <a name="app-interaction-patterns-and-user-activities"></a>Padrões de interação do aplicativo e atividades do usuário 
As atividades do usuário que você cria dependem do padrão de interação do seu aplicativo. Embora todos os aplicativos sejam diferentes, a maioria se encaixa em um dos seguintes padrões de interação: 

* **Aplicativos baseados em documentos** — crie uma única atividade por documento com um ou mais registros de histórico refletindo os períodos de uso. É importante atualizar o cartão de atividades conforme as alterações são feitas no documento. 
* **Aplicativos de reprodução de mídia** — crie uma atividade por agrupamento lógico de conteúdo, como uma lista de reprodução, programa ou conteúdo independente. 
* **Jogos** — crie uma atividade para cada jogo ou mundo salvo. Se seu jogo somente oferecer suporte a uma única sequência de níveis, você poderá criar a mesma atividade ao longo do tempo, embora talvez você queira atualizar seu cartão para mostrar o progresso ou as realizações mais recentes. 
* **Aplicativos de utilitário** — se não houver nada no seu aplicativo que os usuários desejam retomar, você não deve publicar atividades. Um bom exemplo disso é um aplicativo simples com uma única finalidade, como uma calculadora. 
* **Aplicativos de linha de negócios** — existem muitos aplicativos para gerenciar tarefas ou fluxos de trabalho simples. Crie uma atividade para cada fluxo de trabalho separado, acessado por meio do seu aplicativo. Por exemplo, cada relatório de despesas seria uma atividade separada, pois talvez você queira clicar na atividade para ver se ela foi aprovada.

*Alguns aplicativos complexos incluem vários padrões de interação. Talvez você queira seguir os padrões de criação de atividades de diferentes usuários para os diferentes cenários manipulados pelo seu aplicativo.*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>Próximas etapas

- Veja o [recurso de atividade](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity) e defina as atividades do seu aplicativo para ajudar os usuários a retomar tarefas importantes.
- Explore os [exemplos de cartões adaptáveis](http://adaptivecards.io/samples/) para obter ideias e **popularizar** suas atividades.  
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).

**Procurando mais ideias?** 
- Veja [como as experiências da Microsoft estão usando as atividades](https://channel9.msdn.com/events/Build/2017/B8108).
- Saiba mais sobre [a API de feed de atividades e continue de onde parei](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011).
