---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos com o Microsoft Graph. Confira as informações sobre as atualizações mais recentes no Log de alterações do Microsoft Graph.
author: ''
localization_priority: Priority
ms.openlocfilehash: e32474745bb605bd0f9d1451cf8a8818cb06e7e5
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622646"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="07447-104">Problemas conhecidos com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="07447-104">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="07447-p102">Este artigo descreve os problemas conhecidos com o Microsoft Graph. Confira as informações sobre as atualizações mais recentes no [Log de alterações do Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="07447-p102">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="07447-107">Usuários</span><span class="sxs-lookup"><span data-stu-id="07447-107">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="07447-108">Sem acesso instantâneo após a criação</span><span class="sxs-lookup"><span data-stu-id="07447-108">No instant access after creation</span></span>

<span data-ttu-id="07447-p103">Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Office 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro 404 HTTP.</span><span class="sxs-lookup"><span data-stu-id="07447-p103">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="07447-113">Restrições de foto</span><span class="sxs-lookup"><span data-stu-id="07447-113">Photo restrictions</span></span>

<span data-ttu-id="07447-p104">A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio. Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando a visualização da API unificada do Office 365, o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis com a propriedade **photo** do recurso [usuário](/graph/api/resources/user?view=graph-rest-1.0) do Microsoft Graph. A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="07447-p104">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="using-delta-query"></a><span data-ttu-id="07447-117">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="07447-117">Using delta query</span></span>

<span data-ttu-id="07447-118">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="07447-118">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a><span data-ttu-id="07447-119">A revogação de sessões de entrada retorna um código HTTP errado</span><span class="sxs-lookup"><span data-stu-id="07447-119">Revoke sign-in sessions returns wrong HTTP code</span></span>

<span data-ttu-id="07447-120">O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.</span><span class="sxs-lookup"><span data-stu-id="07447-120">The [user: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) should return a `204 No content` response for successful revocations, and an HTTP error code (4xx or 5xx) if anything goes wrong with the request.</span></span>  <span data-ttu-id="07447-121">No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre true.</span><span class="sxs-lookup"><span data-stu-id="07447-121">However, due to a service issue, this API returns a `200 OK` and a Boolean parameter that is always true.</span></span>  <span data-ttu-id="07447-122">Até que isso seja corrigido, é recomendado que desenvolvedores simplesmente tratem qualquer código de retorno 2xx como bem-sucedido para esta API.</span><span class="sxs-lookup"><span data-stu-id="07447-122">Until this is fixed, developers are simply advised to treat any 2xx return code as success for this API.</span></span>

## <a name="microsoft-teams"></a><span data-ttu-id="07447-123">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="07447-123">Microsoft Teams</span></span>

### <a name="get-teams-and-post-teams-are-not-supported"></a><span data-ttu-id="07447-124">Não há suporte para GET /teams e POST /teams</span><span class="sxs-lookup"><span data-stu-id="07447-124">GET /teams and POST /teams are not supported</span></span>

<span data-ttu-id="07447-125">Confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams?view=graph-rest-1.0) para obter uma lista de equipes.</span><span class="sxs-lookup"><span data-stu-id="07447-125">See [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get a list of teams.</span></span>
<span data-ttu-id="07447-126">Confira [criar equipe](/graph/api/team-put-teams?view=graph-rest-1.0) para criar equipes.</span><span class="sxs-lookup"><span data-stu-id="07447-126">See [create team](/graph/api/team-put-teams?view=graph-rest-1.0) for creating teams.</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="07447-127">Equipes ausentes em listas todas as equipes</span><span class="sxs-lookup"><span data-stu-id="07447-127">Missing teams in list all teams</span></span>

<span data-ttu-id="07447-128">Algumas equipes que foram criadas no passado mas não foram usadas recentemente por um usuário do Microsoft Teams não são listadas por [listar todas as equipes](teams-list-all-teams.md).</span><span class="sxs-lookup"><span data-stu-id="07447-128">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="07447-129">Novas equipes serão listadas.</span><span class="sxs-lookup"><span data-stu-id="07447-129">New teams will be listed.</span></span>
<span data-ttu-id="07447-130">Algumas equipes antigas não têm uma propriedade **resourceProvisioningOptions** que contém “Equipe”, que é configurada em equipes recém-criadas e equipes que são visitadas no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="07447-130">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="07447-131">No futuro, vamos configurar **resourceProvisioningOptions** em equipes existentes que não foram abertas no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="07447-131">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="groups"></a><span data-ttu-id="07447-132">Grupos</span><span class="sxs-lookup"><span data-stu-id="07447-132">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="07447-133">Permissões para grupos e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="07447-133">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="07447-134">O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="07447-134">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="07447-135">As permissões do aplicativo devem ser consentidas por um administrador.</span><span class="sxs-lookup"><span data-stu-id="07447-135">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="07447-136">No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="07447-136">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="07447-p109">Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="07447-p109">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="07447-139">Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="07447-139">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="07447-140">Criar e excluir grupos</span><span class="sxs-lookup"><span data-stu-id="07447-140">Creating and deleting groups</span></span>
* <span data-ttu-id="07447-141">Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo</span><span class="sxs-lookup"><span data-stu-id="07447-141">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="07447-142">[Definições do diretório](/graph/api/resources/directoryobject?view=graph-rest-1.0), tipo e sincronização do grupo</span><span class="sxs-lookup"><span data-stu-id="07447-142">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="07447-143">Membros e proprietários de grupo</span><span class="sxs-lookup"><span data-stu-id="07447-143">Group owners and membership</span></span>

<span data-ttu-id="07447-144">Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:</span><span class="sxs-lookup"><span data-stu-id="07447-144">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="07447-145">Conversas, eventos e foto de grupo</span><span class="sxs-lookup"><span data-stu-id="07447-145">Group conversations, events, photo</span></span>
* <span data-ttu-id="07447-146">Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo</span><span class="sxs-lookup"><span data-stu-id="07447-146">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="07447-147">Favoritos do usuário e contagem de não vistos</span><span class="sxs-lookup"><span data-stu-id="07447-147">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="07447-148">Política</span><span class="sxs-lookup"><span data-stu-id="07447-148">Policy</span></span>

<span data-ttu-id="07447-149">O uso do Microsoft Graph para criar e nomear um grupo do Office 365 ultrapassa qualquer política de grupo do Office 365 que seja configurada pelo Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="07447-149">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="07447-150">Definir a propriedade allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="07447-150">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="07447-151">Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.</span><span class="sxs-lookup"><span data-stu-id="07447-151">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="07447-152">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="07447-152">Using delta query</span></span>

<span data-ttu-id="07447-153">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="07447-153">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="bookings"></a><span data-ttu-id="07447-154">Reservas</span><span class="sxs-lookup"><span data-stu-id="07447-154">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="07447-155">ErrorExceededFindCountLimit ao consultar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="07447-155">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="07447-156">A obtenção da lista de `bookingBusinesses` falha com o seguinte código de erro quando a organização tem várias empresas de Reservas e a conta que está fazendo a solicitação não é um administrador:</span><span class="sxs-lookup"><span data-stu-id="07447-156">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="07447-157">Como alternativa, você pode limitar o conjunto de empresas retornadas pela solicitação, incluindo um parâmetro `query`, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="07447-157">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="07447-158">Calendários</span><span class="sxs-lookup"><span data-stu-id="07447-158">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="07447-159">Acessar um calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="07447-159">Accessing a shared calendar</span></span>

<span data-ttu-id="07447-160">Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:</span><span class="sxs-lookup"><span data-stu-id="07447-160">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="07447-p110">Você pode receber HTTP 500 com o código de erro `ErrorInternalServerTransientError`. O erro ocorre porque:</span><span class="sxs-lookup"><span data-stu-id="07447-p110">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="07447-163">Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.</span><span class="sxs-lookup"><span data-stu-id="07447-163">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="07447-164">A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.</span><span class="sxs-lookup"><span data-stu-id="07447-164">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="07447-165">Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.</span><span class="sxs-lookup"><span data-stu-id="07447-165">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="07447-166">Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.</span><span class="sxs-lookup"><span data-stu-id="07447-166">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="07447-167">Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.</span><span class="sxs-lookup"><span data-stu-id="07447-167">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="07447-168">Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="07447-168">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="07447-169">Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="07447-169">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="07447-170">O destinatário remove o calendário previamente compartilhado com ele.</span><span class="sxs-lookup"><span data-stu-id="07447-170">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="07447-171">O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="07447-171">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="07447-p112">O destinatário aceita novamente o calendário compartilhado usando o Outlook na Web. Em breve você poderá usar outros clientes do Outlook.</span><span class="sxs-lookup"><span data-stu-id="07447-p112">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="07447-174">O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="07447-174">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="07447-p113">Um calendário compartilhado com você na nova abordagem é exibido como qualquer outro na sua caixa de correio. Você pode usar a API REST de calendário para visualizar e editar eventos no calendário compartilhado, como se fosse seu próprio calendário. Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="07447-p113">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="07447-178">Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="07447-178">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="07447-179">Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):</span><span class="sxs-lookup"><span data-stu-id="07447-179">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="07447-180">Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="07447-180">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="07447-p114">[Listar os calendários do usuário](/graph/api/user-list-calendars?view=graph-rest-1.0) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.</span><span class="sxs-lookup"><span data-stu-id="07447-p114">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="07447-183">Você também pode [listar os eventos](/graph/api/calendar-list-events?view=graph-rest-1.0) de um calendário baseado em ICS.</span><span class="sxs-lookup"><span data-stu-id="07447-183">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="07447-184">Suporte de propriedade onlineMeetingUrl do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="07447-184">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="07447-185">Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event?view=graph-rest-1.0) de reunião do Skype indica a URL da reunião online.</span><span class="sxs-lookup"><span data-stu-id="07447-185">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="07447-186">No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.</span><span class="sxs-lookup"><span data-stu-id="07447-186">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

## <a name="calls-and-online-meetings"></a><span data-ttu-id="07447-187">Chamadas e reuniões online</span><span class="sxs-lookup"><span data-stu-id="07447-187">Calls and online meetings</span></span>

> <span data-ttu-id="07447-188">**Observação** As chamadas e reuniões online estão atualmente em visualização e estarão disponíveis apenas no ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="07447-188">**Note** Calling and online meetings are currently in preview and are available only in the Microsoft Graph beta endpoint.</span></span>

- <span data-ttu-id="07447-189">O caminho da navegação `/applications/{id}` não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="07447-189">Navigation path `/applications/{id}` is not supported.</span></span> <span data-ttu-id="07447-190">Não é permitido navegar pelo nó de aplicativos globais para o aplicativo, mesmo que seja o seu próprio. </span><span class="sxs-lookup"><span data-stu-id="07447-190">Navigating through the global applications node to the application, even your own, is not allowed.</span></span> <span data-ttu-id="07447-191">Use o `/app` apenas para navegação.</span><span class="sxs-lookup"><span data-stu-id="07447-191">Please use the `/app` navigation only.</span></span>

## <a name="contacts"></a><span data-ttu-id="07447-192">Contatos</span><span class="sxs-lookup"><span data-stu-id="07447-192">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="07447-193">Contatos de organização disponíveis somente na versão beta</span><span class="sxs-lookup"><span data-stu-id="07447-193">Organization contacts available in only beta</span></span>

<span data-ttu-id="07447-p117">Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.</span><span class="sxs-lookup"><span data-stu-id="07447-p117">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="07447-196">Pasta Contatos padrão</span><span class="sxs-lookup"><span data-stu-id="07447-196">Default contacts folder</span></span>

<span data-ttu-id="07447-197">Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="07447-197">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="07447-p118">Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:</span><span class="sxs-lookup"><span data-stu-id="07447-p118">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="07447-200">Na consulta acima:</span><span class="sxs-lookup"><span data-stu-id="07447-200">In the above query:</span></span>

1. <span data-ttu-id="07447-201">`/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact?view=graph-rest-1.0) na pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="07447-201">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="07447-202">A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="07447-202">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="07447-203">Acessar contatos por meio de uma pasta de contatos na versão beta</span><span class="sxs-lookup"><span data-stu-id="07447-203">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="07447-204">Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.</span><span class="sxs-lookup"><span data-stu-id="07447-204">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="07447-205">Acessando um contato a partir de um nível superior do [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="07447-205">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="07447-p119">Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="07447-p119">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="07447-208">Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="07447-208">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="07447-209">Mensagens</span><span class="sxs-lookup"><span data-stu-id="07447-209">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="07447-210">O parâmetro de comentário para criar um rascunho</span><span class="sxs-lookup"><span data-stu-id="07447-210">The comment parameter for creating a draft</span></span>

<span data-ttu-id="07447-211">O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) não se torna parte do corpo do rascunho de mensagem resultante.</span><span class="sxs-lookup"><span data-stu-id="07447-211">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="07447-212">As mensagens GET retornam chats no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="07447-212">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="07447-213">Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal.</span><span class="sxs-lookup"><span data-stu-id="07447-213">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="07447-214">Essas mensagens de chat tem "IM" como o assunto.</span><span class="sxs-lookup"><span data-stu-id="07447-214">These chat messages have "IM" as their subject.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="07447-215">Unidades, arquivos e streaming de conteúdo</span><span class="sxs-lookup"><span data-stu-id="07447-215">Drives, files and content streaming</span></span>

* <span data-ttu-id="07447-216">O acesso pela primeira vez a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse seu site pessoal por um navegador resulta em uma resposta 401.</span><span class="sxs-lookup"><span data-stu-id="07447-216">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="07447-217">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="07447-217">Query parameter limitations</span></span>

* <span data-ttu-id="07447-218">Não há suporte para vários namespaces.</span><span class="sxs-lookup"><span data-stu-id="07447-218">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="07447-219">Não há suporte para GETs em `$ref` e conversão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="07447-219">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="07447-p121">`@odata.bind` não é compatível. Isso significa que os desenvolvedores não poderão definir corretamente a propriedade de navegação **acceptedSenders** ou **rejectedSenders** em um grupo.</span><span class="sxs-lookup"><span data-stu-id="07447-p121">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span></span>
* <span data-ttu-id="07447-222">`@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.</span><span class="sxs-lookup"><span data-stu-id="07447-222">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="07447-223">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="07447-223"></span></span>
  * <span data-ttu-id="07447-224">Não há suporte para `nextLink`</span><span class="sxs-lookup"><span data-stu-id="07447-224">No support for `nextLink`</span></span>
  * <span data-ttu-id="07447-225">Não há suporte para mais de um nível de expansão</span><span class="sxs-lookup"><span data-stu-id="07447-225">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="07447-226">Não há suporte com parâmetros adicionais (`$filter`, `$select`)</span><span class="sxs-lookup"><span data-stu-id="07447-226">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="07447-227">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="07447-227"></span></span>
  * <span data-ttu-id="07447-228">Não há suporte para filtros no ponto de extremidade `/attachments`.</span><span class="sxs-lookup"><span data-stu-id="07447-228">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="07447-229">Se presente, o parâmetro `$filter` é ignorado.</span><span class="sxs-lookup"><span data-stu-id="07447-229">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="07447-230">Não há suporte para filtragem de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="07447-230">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="07447-231">`$search`:</span><span class="sxs-lookup"><span data-stu-id="07447-231"></span></span>
  * <span data-ttu-id="07447-232">A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.</span><span class="sxs-lookup"><span data-stu-id="07447-232">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="07447-233">Não há suporte para pesquisa de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="07447-233">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="07447-234">Consulta delta</span><span class="sxs-lookup"><span data-stu-id="07447-234">Delta query</span></span>

* <span data-ttu-id="07447-235">O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.</span><span class="sxs-lookup"><span data-stu-id="07447-235">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="07447-236">As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.</span><span class="sxs-lookup"><span data-stu-id="07447-236">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="07447-237">Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.</span><span class="sxs-lookup"><span data-stu-id="07447-237">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="07447-238">Alterações do aplicativo e da API servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="07447-238">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="07447-p123">Há alterações para as entidades [application](/graph/api/resources/application?view=graph-rest-beta) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="07447-p123">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="07447-241">Limitações atuais:</span><span class="sxs-lookup"><span data-stu-id="07447-241">Current limitations:</span></span>

* <span data-ttu-id="07447-242">Algumas propriedades do aplicativo (como appRoles e addIns) não estarão disponíveis até que todas as alterações sejam concluídas.</span><span class="sxs-lookup"><span data-stu-id="07447-242">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="07447-243">Somente aplicativos multilocatários podem ser registrados.</span><span class="sxs-lookup"><span data-stu-id="07447-243">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="07447-244">Atualizar aplicativos é restrito aos aplicativos registrados após a atualização inicial beta.</span><span class="sxs-lookup"><span data-stu-id="07447-244">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="07447-245">Usuários do Azure Active Directory podem registrar aplicativos e adicionar proprietários adicionais.</span><span class="sxs-lookup"><span data-stu-id="07447-245">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="07447-246">Suporte para protocolos OpenID Connect e OAuth.</span><span class="sxs-lookup"><span data-stu-id="07447-246">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="07447-247">Atribuições de política para uma falha de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="07447-247">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="07447-248">Falha em operações em ownedObjects que exigem appId (por exemplo, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="07447-248">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="07447-249">Em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="07447-249">In development:</span></span>

* <span data-ttu-id="07447-250">Capacidade de registrar aplicativos de um único locatário.</span><span class="sxs-lookup"><span data-stu-id="07447-250">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="07447-251">Atualizações para o servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="07447-251">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="07447-252">Migração de aplicativos Azure AD existentes para um modelo atualizado.</span><span class="sxs-lookup"><span data-stu-id="07447-252">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="07447-253">Suporte para appRoles, clientes pré-autorizados, reivindicações opcionais, reivindicações de associação de grupo e identidade visual.</span><span class="sxs-lookup"><span data-stu-id="07447-253">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="07447-254">Os usuários de conta Microsoft (MSA) podem registrar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="07447-254">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="07447-255">Suporte para protocolos SAML e WsFed.</span><span class="sxs-lookup"><span data-stu-id="07447-255">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="07447-256">Extensões</span><span class="sxs-lookup"><span data-stu-id="07447-256">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="07447-257">Não há suporte para o controle de alterações</span><span class="sxs-lookup"><span data-stu-id="07447-257">Change tracking is not supported</span></span>

<span data-ttu-id="07447-258">O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.</span><span class="sxs-lookup"><span data-stu-id="07447-258">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="07447-259">Criar um recurso e uma extensão aberta ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="07447-259">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="07447-p124">Você não pode especificar uma extensão aberta ao mesmo tempo que cria uma instância de **administrativeUnit**, **device**, **group**, **organization** ou **user**. Primeiro você deve criar a instância e, depois, especificar os dados da extensão aberta em uma solicitação ``POST`` subsequente nessa instância.</span><span class="sxs-lookup"><span data-stu-id="07447-p124">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="07447-262">Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="07447-262">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="07447-263">Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="07447-263">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="07447-264">Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="07447-264">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="07447-265">Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos</span><span class="sxs-lookup"><span data-stu-id="07447-265">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="07447-266">Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.</span><span class="sxs-lookup"><span data-stu-id="07447-266">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="07447-267">Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="07447-267">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="07447-268">Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="07447-268">Filtering on schema extension properties (using the `$filter` expression) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="07447-269">Envio em lote JSON</span><span class="sxs-lookup"><span data-stu-id="07447-269">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="07447-270">Nenhum lote aninhado</span><span class="sxs-lookup"><span data-stu-id="07447-270">No nested batch</span></span>

<span data-ttu-id="07447-271">Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.</span><span class="sxs-lookup"><span data-stu-id="07447-271">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="07447-272">Todas as solicitações individuais devem ser síncronas</span><span class="sxs-lookup"><span data-stu-id="07447-272">All individual requests must be synchronous</span></span>

<span data-ttu-id="07447-p126">Todas as solicitações contidas em uma solicitação de lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.</span><span class="sxs-lookup"><span data-stu-id="07447-p126">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="07447-275">Sem transações</span><span class="sxs-lookup"><span data-stu-id="07447-275">No transactions</span></span>

<span data-ttu-id="07447-p127">No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade `atomicityGroup` em solicitações individuais será ignorada.</span><span class="sxs-lookup"><span data-stu-id="07447-p127">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="07447-278">URIs devem ser relativas</span><span class="sxs-lookup"><span data-stu-id="07447-278">URIs must be relative</span></span>

<span data-ttu-id="07447-p128">Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.</span><span class="sxs-lookup"><span data-stu-id="07447-p128">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="07447-281">Limite de tamanho de lote</span><span class="sxs-lookup"><span data-stu-id="07447-281">Limit on batch size</span></span>

<span data-ttu-id="07447-282">No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.</span><span class="sxs-lookup"><span data-stu-id="07447-282">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="07447-283">Dependências simplificadas</span><span class="sxs-lookup"><span data-stu-id="07447-283">Simplified dependencies</span></span>

<span data-ttu-id="07447-p129">Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:</span><span class="sxs-lookup"><span data-stu-id="07447-p129">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="07447-286">Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="07447-286">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="07447-287">Serial – todas as solicitações individuais dependem da solicitação individual anterior.</span><span class="sxs-lookup"><span data-stu-id="07447-287">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="07447-288">Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.</span><span class="sxs-lookup"><span data-stu-id="07447-288">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="07447-289">Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.</span><span class="sxs-lookup"><span data-stu-id="07447-289">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="07447-290">Aplicativos de Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="07447-290">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="07447-291">Os aplicativos CSP devem usar o ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="07447-291">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="07447-p130">Aplicativos de provedor de solução de nuvem (CSP) devem adquirir tokens de pontos de extremidade do Azure AD (v1) para chamar a Microsoft Graph com êxito em seus clientes gerenciados por parceiros. Atualmente, não há suporte para aquisição de um token pelo ponto de extremidade Azure AD v 2.0 mais recente.</span><span class="sxs-lookup"><span data-stu-id="07447-p130">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="07447-294">A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente</span><span class="sxs-lookup"><span data-stu-id="07447-294">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="07447-295">Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="07447-295">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="07447-296">Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="07447-296">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="07447-297">Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="07447-297">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="07447-298">Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="07447-298">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="07447-299">Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="07447-299">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="07447-p131">**OBSERVAÇÃO:** esta não é uma solução permanente e destina-se apenas a desbloquear o desenvolvimento.  Esta solução alternativa não será necessária uma vez que a questão acima mencionada seja corrigida.  Esta solução alternativa não precisa ser desfeita após a correção.</span><span class="sxs-lookup"><span data-stu-id="07447-p131">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="07447-p132">Abra uma sessão do Azure AD v2 PowerShell e conecte-se ao locatário do parceiro `customer`digitando suas credenciais de administrador na janela de entrada. Você pode baixar e instalar o Azure AD PowerShell V2 [aqui](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="07447-p132">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="07447-305">Crie o servicePrincipal do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="07447-305">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="07447-306">Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365</span><span class="sxs-lookup"><span data-stu-id="07447-306">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="07447-p133">Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](https://msdn.microsoft.com/office/office365/api/api-catalog) específicas do ponto de extremidade. Para o Azure Active Directory, veja a postagem no blog [Microsoft Graph ou Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) sobre os recursos que só estão disponíveis pela API do Graph do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="07447-p133">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

