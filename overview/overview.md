# <a name="overview-of-microsoft-graph"></a>Visão geral do Microsoft Graph

O Microsoft Graph expõe várias APIs do Office 365 e outros serviços de nuvem da Microsoft por meio de um único ponto de extremidade: (**https://graph.microsoft.com**). O Microsoft Graph simplifica as consultas que, de outra forma, seriam mais complexas. 
 
Você pode usar a instalação do Microsoft Graph para:

- Acessar os dados de vários serviços de nuvem da Microsoft, como Azure Active Directory, Exchange Online como parte do Office 365, SharePoint, OneDrive, OneNote e Planner.
- Navegar entre entidades e relações.
- Acessar a inteligência e as informações provenientes da nuvem da Microsoft (para usuários comerciais).

**Pilha de desenvolvimento do Microsoft Graph**

![Um diagrama que mostra as camadas da pilha de desenvolvimento do Microsoft Graph. Na parte inferior, está a camada de dados, que inclui usuários, grupos, arquivos, emails, calendários, contatos pessoais, tarefas, contatos da organização, pessoas, Excel e anotações. A próxima camada é autenticação e autorização A próxima é o ambiente de desenvolvimento da sua escolha, como os SDKs da API do Microsoft Graph do Visual Studio, iOS e Android. A camada final é a sua solução, que usa a tecnologia da sua escolha, como .NET, JS, HTML e Ruby, e está hospedada no Microsoft Azure ou em outra plataforma de hospedagem.](./images/MicrosoftGraph_DevStack.png)

<!--<a name="msg_queries"> </a>-->

##<a name="common-microsoft-graph-queries"></a>Consultas comuns do Microsoft Graph

O Microsoft Graph expõe dois pontos de extremidade: /v1.0 e /beta. O ponto de extremidade /v1.0 inclui os recursos que você pode acessar em seu aplicativo de produção. O ponto de extremidade [/beta](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/beta-overview) inclui APIs que estão atualmente em modo de visualização. A tabela a seguir lista algumas consultas comuns que você pode usar para acessar a API do Microsoft Graph.

| **Operação**    | **Ponto de extremidade de serviço** |
|:--------------------------|:----------------------------------------|
|   GET meu perfil |    [`https://graph.microsoft.com/v1.0/me`](https://graph.microsoft.io/en-us/graph-explorer/?request=me&version=v1.0) |
|   GET meus arquivos | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   GET minha foto     | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   GET meu email |    [`https://graph.microsoft.com/v1.0/me/messages`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   GET meu email de alta prioridade | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   GET meu calendário |    [`https://graph.microsoft.com/v1.0/me/calendar`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fcalendar&version=v1.0) |
|   GET meu gerente    | [`https://graph.microsoft.com/v1.0/me/manager`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   GET o último usuário que modificou o arquivo foo.txt |    [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   GET grupos unificados dos quais sou membro|    [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   GET os usuários em minha organização     | [`https://graph.microsoft.com/v1.0/users`](https://graph.microsoft.io/en-us/graph-explorer/?request=users&version=v1.0) |
|   GET conversas em grupo |    `https://graph.microsoft.com/v1.0/groups/{id}/conversations`|
|   GET as pessoas relacionadas a mim    | [`https://graph.microsoft.com/beta/me/people`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   Itens GET mais populares à minha volta |    [`https://graph.microsoft.com/beta/me/insights/trending`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   GET minhas tarefas    | [`https://graph.microsoft.com/beta/me/tasks`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Ftasks&version=beta) |
|   GET minhas anotações |    [`https://graph.microsoft.com/beta/me/notes/notebooks`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fnotes%2Fnotebooks&version=beta) |


>**Observação:** As APIs no ponto de extremidade beta estão sujeitas a mudanças. Não recomendamos que você as use em seus aplicativos de produção. 

<!-- <a name="msg_roof"> </a> -->

## <a name="explore-microsoft-graph"></a>Explorar o Microsoft Graph

- [Comece](https://developer.microsoft.com/en-us/graph/docs/get-started/get-started) a usar o Microsoft Graph e a plataforma de sua escolha.
- Descubra os recursos e as operações que você pode usar em seus aplicativos de produção, procurando no Sumário.
- Visualize as novas [APIs /beta](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/beta-overview).
- Visite o [Explorador do Microsoft Graph](https://graph.microsoft.io/graph-explorer).
- Confira nossos [exemplos de trechos do Microsoft Graph](https://github.com/search?q=org%3Amicrosoftgraph+snippets-sample).

 >  Seus comentários são importantes para nós. Junte-se a nós na página [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph). Marque as suas perguntas com {MicrosoftGraph} e {office365}.



