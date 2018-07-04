# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="9ee5b-101">Problemas conhecidos com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9ee5b-101">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="9ee5b-p101">Este artigo descreve os problemas conhecidos com o Microsoft Graph. Confira as informações sobre as atualizações mais recentes no [Log de alterações do Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p101">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="9ee5b-104">Usuários</span><span class="sxs-lookup"><span data-stu-id="9ee5b-104">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="9ee5b-105">Sem acesso instantâneo após a criação</span><span class="sxs-lookup"><span data-stu-id="9ee5b-105">No instant access after creation</span></span>

<span data-ttu-id="9ee5b-p102">Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Office 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro 404 HTTP.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p102">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="9ee5b-110">Restrições de foto</span><span class="sxs-lookup"><span data-stu-id="9ee5b-110">Photo restrictions</span></span>

<span data-ttu-id="9ee5b-p103">A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio. Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando a visualização da API unificada do Office 365, o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis com a propriedade **photo** do recurso [usuário](../api-reference/v1.0/resources/user.md) do Microsoft Graph. A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p103">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](../api-reference/v1.0/resources/user.md) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### <a name="using-delta-query"></a><span data-ttu-id="9ee5b-114">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="9ee5b-114">Using delta query</span></span>

<span data-ttu-id="9ee5b-115">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-115">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="groups-and-microsoft-teams"></a><span data-ttu-id="9ee5b-116">Grupos e o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9ee5b-116">Groups and Microsoft Teams</span></span>

><span data-ttu-id="9ee5b-117">**Observação** o Microsoft Teams está atualmente como visualização e disponível apenas no ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-117">**Note** Microsoft Teams is currently in preview and is available only in the Microsoft Graph beta endpoint.</span></span>

### <a name="policy"></a><span data-ttu-id="9ee5b-118">Política</span><span class="sxs-lookup"><span data-stu-id="9ee5b-118">Policy</span></span>

<span data-ttu-id="9ee5b-119">O uso do Microsoft Graph para criar e nomear um grupo do Office 365 ultrapassa qualquer política de grupo do Office 365 que seja configurada pelo Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-119">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="9ee5b-120">Permissões para grupos e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9ee5b-120">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="9ee5b-p104">O Microsoft Graph expõe duas permissões (*Group.Read.All* e *Group.ReadWrite.All*) para obter acesso a APIs de grupos e Microsoft Teams. Essas permissões devem ser consentidas por um administrador (que é uma alteração da visualização).  No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p104">Microsoft Graph exposes two permissions (*Group.Read.All* and *Group.ReadWrite.All*) for access to the APIs for groups and Microsoft Teams. These permissions must be consented to by an administrator (which is a change from preview).  In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="9ee5b-p105">Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p105">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="9ee5b-126">Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-126">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="9ee5b-127">Criar e excluir grupos</span><span class="sxs-lookup"><span data-stu-id="9ee5b-127">Creating and deleting groups</span></span>
* <span data-ttu-id="9ee5b-128">Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-128">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="9ee5b-129">[Definições do diretório](../api-reference/v1.0/resources/directoryobject.md), tipo e sincronização do grupo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-129">Group [directory settings](../api-reference/v1.0/resources/directoryobject.md), type, and synchronization</span></span>
* <span data-ttu-id="9ee5b-130">Membros e proprietários de grupo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-130">Group owners and membership</span></span>

<span data-ttu-id="9ee5b-131">Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-131">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="9ee5b-132">Conversas, eventos e foto de grupo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-132">Group conversations, events, photo</span></span>
* <span data-ttu-id="9ee5b-133">Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-133">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="9ee5b-134">Favoritos do usuário e contagem de não vistos</span><span class="sxs-lookup"><span data-stu-id="9ee5b-134">User favorites and unseen count</span></span>
* <span data-ttu-id="9ee5b-135">Canais e chats do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9ee5b-135">Microsoft Teams channels and chats</span></span>

### <a name="teams-in-microsoft-teams-preview"></a><span data-ttu-id="9ee5b-136">Equipes no Microsoft Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="9ee5b-136">Teams in Microsoft Teams (preview)</span></span>

<span data-ttu-id="9ee5b-p106">Os grupos do Microsoft Teams e do Office 365 [têm funcionalidades parecidas](../api-reference/beta/resources/teams_api_overview.md). Todas as APIs de grupo podem ser usadas com as equipes, com a exceção de que a API Criar grupo não permite atualmente a criação de uma equipe.  As versões futuras da API oferecerão suporte para isso.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p106">Microsoft Teams and Office 365 groups [share similar functionality](../api-reference/beta/resources/teams_api_overview.md). All group APIs can be used with teams, with the exception that the Create group API does not currently allow you to create a team.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-channels-preview"></a><span data-ttu-id="9ee5b-140">Canais do Microsoft Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="9ee5b-140">Microsoft Teams channels (preview)</span></span>

<span data-ttu-id="9ee5b-p107">Atualmente você pode ler e criar canais, mas não pode atualizá-los ou excluí-los.  Versões futuras da API terão suporte.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p107">Currently, you can read and create channels, but you cannot update or delete them.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-chat-threads-and-chat-messages-preview"></a><span data-ttu-id="9ee5b-143">Threads de chat e mensagens de chat do Microsoft Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="9ee5b-143">Microsoft Teams chat threads and chat messages (preview)</span></span>

<span data-ttu-id="9ee5b-p108">Atualmente é possível criar threads de chat em canais, mas não é possível ler os threads de chat existentes ou adicionar respostas a eles. Além disso, não é possível ler ou gravar chats diretos entre usuários que estejam fora do escopo de uma equipe ou de um canal.  As versões futuras da API agregarão recursos adicionais nessa área.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p108">Currently, you can create chat threads in channels, but you cannot read existing chat threads or add replies to them. Also, you cannot read or write direct chats between users that are outside the scope of a team or channel.  Future API releases will add additional capabilities in this area.</span></span>

### <a name="microsoft-teams-users-list-of-joined-teams-preview"></a><span data-ttu-id="9ee5b-147">Lista de equipes unidas do usuário do Microsoft Teams (visualização)</span><span class="sxs-lookup"><span data-stu-id="9ee5b-147">Microsoft Teams user's list of joined teams (preview)</span></span>

<span data-ttu-id="9ee5b-p109">Atualmente, [listar as equipes em que um usuário ingressou](../api-reference/beta/api/user_list_joinedteams.md) só funciona para o usuário "eu" para o qual o chamador [delegou permissões](permissions_reference.md).  Versões futuras terão suporte a esta operação para qualquer ID de usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p109">Currrently, [listing the teams a user has joined](../api-reference/beta/api/user_list_joinedteams.md) only works for the 'me' user for which the caller has [delegated permissions](permissions_reference.md).  Future releases will support this operation for any specified user ID.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="9ee5b-150">Adicionando e obtendo anexos de postagens de grupo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-150">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="9ee5b-p110">A [adição](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/post_post_attachments) de anexos a postagens de grupo a [listagem](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/post_list_attachments) e a obtenção de anexos de postagens do grupo atualmente retornam a mensagem de erro "A solicitação de OData não tem suporte." Uma correção foi implementada nas versões `/v1.0` e `/beta`, e deve estar amplamente disponível até o final de janeiro de 2016.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p110">[Adding](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/post_post_attachments) attachments to group posts, [listing](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/post_list_attachments) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="9ee5b-153">Definir a propriedade allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="9ee5b-153">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="9ee5b-154">Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-154">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="9ee5b-155">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="9ee5b-155">Using delta query</span></span>

<span data-ttu-id="9ee5b-156">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-156">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>


## <a name="calendars"></a><span data-ttu-id="9ee5b-157">Calendários</span><span class="sxs-lookup"><span data-stu-id="9ee5b-157">Calendars</span></span>

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="9ee5b-158">Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="9ee5b-158">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="9ee5b-159">Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):</span><span class="sxs-lookup"><span data-stu-id="9ee5b-159">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="9ee5b-160">Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-160">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="9ee5b-p111">[Listar os calendários do usuário](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_calendars) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/calendar) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p111">[Listing the user's calendars](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_calendars) lets you get the **name**, **color** and **id** properties of each [calendar](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="9ee5b-163">Você também pode [listar os eventos](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/calendar_list_events) de um calendário baseado em ICS.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-163">You can also [list the events](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/calendar_list_events) of an ICS-based calendar.</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="9ee5b-164">Acessar um calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="9ee5b-164">Accessing a shared calendar</span></span>

<span data-ttu-id="9ee5b-165">Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-165">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="9ee5b-p112">Você pode receber HTTP 500 com o código de erro `ErrorInternalServerTransientError`. O erro ocorre porque:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p112">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="9ee5b-168">Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-168">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="9ee5b-169">A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-169">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="9ee5b-170">Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-170">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="9ee5b-171">Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-171">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="9ee5b-172">Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-172">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="9ee5b-173">Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-173">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="9ee5b-174">Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-174">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="9ee5b-175">O destinatário remove o calendário previamente compartilhado com ele.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-175">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="9ee5b-176">O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-176">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="9ee5b-p114">O destinatário aceita novamente o calendário compartilhado usando o Outlook na Web. Em breve você poderá usar outros clientes do Outlook.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p114">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="9ee5b-179">O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-179">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="9ee5b-p115">Um calendário compartilhado com você na nova abordagem é exibido como qualquer outro na sua caixa de correio. Você pode usar a API REST de calendário para visualizar e editar eventos no calendário compartilhado, como se fosse seu próprio calendário. Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p115">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```


## <a name="contacts"></a><span data-ttu-id="9ee5b-183">Contatos</span><span class="sxs-lookup"><span data-stu-id="9ee5b-183">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="9ee5b-184">Contatos de organização disponíveis somente na versão beta</span><span class="sxs-lookup"><span data-stu-id="9ee5b-184">Organization contacts available in only beta</span></span>

<span data-ttu-id="9ee5b-p116">Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p116">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="9ee5b-187">Pasta Contatos padrão</span><span class="sxs-lookup"><span data-stu-id="9ee5b-187">Default contacts folder</span></span>

<span data-ttu-id="9ee5b-188">Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-188">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="9ee5b-p117">Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_contacts) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p117">A fix will be made available. Meanwhile, you can use the following [list contacts](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="9ee5b-191">Na consulta acima:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-191">In the above query:</span></span>

1. <span data-ttu-id="9ee5b-192">`/me/contacts?$top=1` obtém as propriedades de um [contato](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/contact) na pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-192">`/me/contacts?$top=1` gets the properties of a [contact](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="9ee5b-193">A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-193">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="9ee5b-194">Acessar contatos por meio de uma pasta de contatos na versão beta</span><span class="sxs-lookup"><span data-stu-id="9ee5b-194">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="9ee5b-195">Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](../api-reference/beta/resources/contact.md) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-195">In the `/beta` version, there is currently an issue that prevents accessing a [contact](../api-reference/beta/resources/contact.md) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="9ee5b-196">Acessando um contato a partir de um nível superior do [contactFolder](../api-reference/beta/resources/contactfolder.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-196">Accessing a contact from a top level [contactFolder](../api-reference/beta/resources/contactfolder.md) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="9ee5b-p118">Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p118">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="9ee5b-199">Como alternativa, você pode simplesmente [obter](../api-reference/beta/api/contact_get.md) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-199">As an alternative, you can simply [get](../api-reference/beta/api/contact_get.md) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="9ee5b-200">Mensagens</span><span class="sxs-lookup"><span data-stu-id="9ee5b-200">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="9ee5b-201">O parâmetro de comentário para criar um rascunho</span><span class="sxs-lookup"><span data-stu-id="9ee5b-201">The comment parameter for creating a draft</span></span>

<span data-ttu-id="9ee5b-202">O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) não se torna parte do corpo do rascunho de mensagem resultante.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-202">The **comment** parameter for creating a reply or forward draft ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) does not become part of the body of the resultant message draft.</span></span>

## <a name="bookings"></a><span data-ttu-id="9ee5b-203">Bookings</span><span class="sxs-lookup"><span data-stu-id="9ee5b-203">Microsoft Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="9ee5b-204">ErrorExceededFindCountLimit ao consultar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="9ee5b-204">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="9ee5b-205">A obtenção da lista de `bookingBusinesses` falha com o seguinte código de erro quando a organização tem várias empresas de reservas e a conta que está fazendo a solicitação não é um administrador:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-205">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several booking businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="9ee5b-206">O conjunto de empresas retornado pela solicitação pode ser limitado com a inclusão de um parâmetro de consulta, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-206">The set of businesses returned by the request can be limited by including a query parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```

## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="9ee5b-207">Unidades, arquivos e streaming de conteúdo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-207">Drives, files and content streaming</span></span>

* <span data-ttu-id="9ee5b-208">O acesso pela primeira vez a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse seu site pessoal por um navegador resulta em uma resposta 401.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-208">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="9ee5b-209">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="9ee5b-209">Query parameter limitations</span></span>

* <span data-ttu-id="9ee5b-210">Não há suporte para vários namespaces.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-210">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="9ee5b-211">Não há suporte para GETs em `$ref` e conversão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-211">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="9ee5b-p119">Não há suporte para `@odata.bind`. Isso significa que os desenvolvedores não poderão definir corretamente `Accepted` ou `RejectedSenders` em um grupo.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p119">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="9ee5b-214">`@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-214">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="9ee5b-215">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-215">`$expand`:</span></span>
  * <span data-ttu-id="9ee5b-216">Não há suporte para `nextLink`</span><span class="sxs-lookup"><span data-stu-id="9ee5b-216">No support for `nextLink`</span></span>
  * <span data-ttu-id="9ee5b-217">Não há suporte para mais de um nível de expansão</span><span class="sxs-lookup"><span data-stu-id="9ee5b-217">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="9ee5b-218">Não há suporte com parâmetros adicionais (`$filter`, `$select`)</span><span class="sxs-lookup"><span data-stu-id="9ee5b-218">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="9ee5b-219">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-219"></span></span>
  * <span data-ttu-id="9ee5b-220">Não há suporte para filtros no ponto de extremidade `/attachments`.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-220">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="9ee5b-221">Se presente, o parâmetro `$filter` é ignorado.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-221">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="9ee5b-222">Não há suporte para filtragem de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-222">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="9ee5b-223">`$search`:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-223"></span></span>
  * <span data-ttu-id="9ee5b-224">A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-224">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="9ee5b-225">Não há suporte para pesquisa de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-225">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="9ee5b-226">Consulta delta</span><span class="sxs-lookup"><span data-stu-id="9ee5b-226">Delta query</span></span>

* <span data-ttu-id="9ee5b-227">O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-227">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="9ee5b-228">As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-228">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="9ee5b-229">Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-229">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="9ee5b-230">Alterações da API Application e servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="9ee5b-230">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="9ee5b-p121">Há alterações para as entidades [application](../api-reference/beta/resources/application.md) e [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p121">There are changes to the [application](../api-reference/beta/resources/application.md) and [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="9ee5b-233">Limitações atuais:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-233">Current limitations:</span></span>

* <span data-ttu-id="9ee5b-234">Algumas propriedades do aplicativo (como appRoles e addIns) não estarão disponíveis até que todas as alterações sejam concluídas.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-234">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="9ee5b-235">Somente aplicativos multilocatários podem ser registrados.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-235">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="9ee5b-236">Atualizar aplicativos é restrito aos aplicativos registrados após a atualização inicial beta.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-236">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="9ee5b-237">Usuários do Azure Active Directory podem registrar aplicativos e adicionar proprietários adicionais.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-237">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="9ee5b-238">Suporte para protocolos OpenID Connect e OAuth.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-238">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="9ee5b-239">Atribuições de política para uma falha de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-239">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="9ee5b-240">Falha em operações em ownedObjects que exigem appId (por exemplo, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="9ee5b-240">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="9ee5b-241">Em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-241">In development:</span></span>

* <span data-ttu-id="9ee5b-242">Capacidade de registrar aplicativos de um único locatário.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-242">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="9ee5b-243">Atualizações para o servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-243">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="9ee5b-244">Migração de aplicativos Azure AD existentes para um modelo atualizado.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-244">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="9ee5b-245">Suporte para appRoles, clientes pré-autorizados, reivindicações opcionais, reivindicações de associação de grupo e identidade visual.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-245">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="9ee5b-246">Os usuários de conta Microsoft (MSA) podem registrar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-246">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="9ee5b-247">Suporte para protocolos SAML e WsFed.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-247">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="9ee5b-248">Extensões</span><span class="sxs-lookup"><span data-stu-id="9ee5b-248">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="9ee5b-249">Não há suporte para o controle de alterações</span><span class="sxs-lookup"><span data-stu-id="9ee5b-249">Change tracking is not supported</span></span>

<span data-ttu-id="9ee5b-250">O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-250">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="9ee5b-251">Criar um recurso e uma extensão aberta ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-251">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="9ee5b-p122">Você não pode especificar uma extensão aberta ao mesmo tempo que cria uma instância de **administrativeUnit**, **device**, **group**, **organization** ou **user**. Primeiro você deve criar a instância e, depois, especificar os dados da extensão aberta em uma solicitação ``POST`` subsequente nessa instância.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p122">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="9ee5b-254">Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="9ee5b-254">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="9ee5b-255">Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-255">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="9ee5b-256">Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-256">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="9ee5b-257">Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos</span><span class="sxs-lookup"><span data-stu-id="9ee5b-257">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="9ee5b-258">Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-258">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="9ee5b-259">Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="9ee5b-259">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="9ee5b-260">Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contact**, **event**, **message** ou **post**.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-260">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="9ee5b-261">Processamento em lotes JSON</span><span class="sxs-lookup"><span data-stu-id="9ee5b-261">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="9ee5b-262">Nenhum lote aninhado</span><span class="sxs-lookup"><span data-stu-id="9ee5b-262">No nested batch</span></span>

<span data-ttu-id="9ee5b-263">Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-263">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="9ee5b-264">Todas as solicitações individuais devem ser síncronas</span><span class="sxs-lookup"><span data-stu-id="9ee5b-264">All individual requests must be synchronous</span></span>

<span data-ttu-id="9ee5b-p124">Todas as solicitações contidas em uma solicitação de lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p124">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="9ee5b-267">Sem transações</span><span class="sxs-lookup"><span data-stu-id="9ee5b-267">No transactions</span></span>

<span data-ttu-id="9ee5b-p125">No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade `atomicityGroup` em solicitações individuais será ignorada.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p125">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="9ee5b-270">URIs devem ser relativas</span><span class="sxs-lookup"><span data-stu-id="9ee5b-270">URIs must be relative</span></span>

<span data-ttu-id="9ee5b-p126">Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p126">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="9ee5b-273">Limite de tamanho de lote</span><span class="sxs-lookup"><span data-stu-id="9ee5b-273">Limit on batch size</span></span>

<span data-ttu-id="9ee5b-274">No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-274">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="9ee5b-275">Dependências simplificadas</span><span class="sxs-lookup"><span data-stu-id="9ee5b-275">Simplified dependencies</span></span>

<span data-ttu-id="9ee5b-p127">Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p127">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="9ee5b-278">Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-278">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="9ee5b-279">Serial – todas as solicitações individuais dependem da solicitação individual anterior.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-279">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="9ee5b-280">Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-280">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="9ee5b-281">Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-281">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="9ee5b-282">Aplicativos de Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="9ee5b-282">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="9ee5b-283">Os aplicativos CSP devem usar o ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="9ee5b-283">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="9ee5b-p128">Aplicativos de provedor de solução de nuvem (CSP) devem adquirir tokens de pontos de extremidade do Azure AD (v1) para chamar a Microsoft Graph com êxito em seus clientes gerenciados por parceiros. Atualmente, não há suporte para aquisição de um token pelo ponto de extremidade Azure AD v 2.0 mais recente.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p128">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="9ee5b-286">A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente</span><span class="sxs-lookup"><span data-stu-id="9ee5b-286">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="9ee5b-287">Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-287">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="9ee5b-288">Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-288">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="9ee5b-289">Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-289">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="9ee5b-290">Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-290">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="9ee5b-291">Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-291">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="9ee5b-p129">**OBSERVAÇÃO:** esta não é uma solução permanente e destina-se apenas a desbloquear o desenvolvimento.  Esta solução alternativa não será necessária uma vez que a questão acima mencionada seja corrigida.  Esta solução alternativa não precisa ser desfeita após a correção.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p129">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="9ee5b-p130">Abra uma sessão do Azure AD v2 PowerShell e conecte-se ao locatário do parceiro `customer`digitando suas credenciais de administrador na janela de entrada. Você pode baixar e instalar o Azure AD PowerShell V2 [aqui](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p130">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="9ee5b-297">Crie o servicePrincipal do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-297">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="9ee5b-298">Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365</span><span class="sxs-lookup"><span data-stu-id="9ee5b-298">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="9ee5b-p131">Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](https://msdn.microsoft.com/pt-BR/office/office365/api/api-catalog) específicas do ponto de extremidade. Para o Azure Active Directory, veja a postagem no blog [Microsoft Graph ou Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) sobre os recursos que só estão disponíveis pela API do Graph do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p131">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/pt-BR/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="9ee5b-302">Comentários</span><span class="sxs-lookup"><span data-stu-id="9ee5b-302">Feedback</span></span>

> <span data-ttu-id="9ee5b-p132">Seus comentários são importantes para nós. Junte-se a nós na página [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span><span class="sxs-lookup"><span data-stu-id="9ee5b-p132">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
