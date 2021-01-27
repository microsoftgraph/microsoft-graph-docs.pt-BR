---
title: Compartilhar ou delegar um calendário no Outlook
description: No Outlook, um proprietário de calendário pode compartilhá-lo com outro usuário ou delegar outro usuário para gerenciar reuniões no calendário principal do proprietário.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 26319854c20401d96f94a5fa6735777a1645d2a9
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013650"
---
# <a name="share-or-delegate-a-calendar-in-outlook"></a><span data-ttu-id="9b3e5-103">Compartilhar ou delegar um calendário no Outlook</span><span class="sxs-lookup"><span data-stu-id="9b3e5-103">Share or delegate a calendar in Outlook</span></span>

<span data-ttu-id="9b3e5-104">No Outlook, o proprietário do calendário pode compartilhá-lo com outro usuário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-104">In Outlook, a calendar owner can share the calendar with another user.</span></span> <span data-ttu-id="9b3e5-105">O proprietário pode especificar quais informações em eventos não particulares podem ser visualizadas e pode conceder acesso de gravação para os usuários na mesma organização.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-105">The owner can specify which information in non-private events is viewable, and can give write access to the calendar to users in the same organization.</span></span> 

<span data-ttu-id="9b3e5-106">O proprietário também pode delegar outro usuário a gerenciar reuniões no calendário _principal_ do proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-106">The owner can also delegate another user to manage meetings in the owner's _primary_ calendar.</span></span> <span data-ttu-id="9b3e5-107">Delegados são sharees que podem visualizar todas as informações e ter acesso de gravação a eventos não privados.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-107">Delegates are sharees who can view all information in and have write access to non-private events.</span></span> <span data-ttu-id="9b3e5-108">Eles também recebem solicitações de reunião e respostas, além de responder a solicitações de reunião em nome do proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-108">They also receive meeting requests and responses, and respond to meeting requests on behalf of the owner.</span></span> <span data-ttu-id="9b3e5-109">Além disso, o proprietário pode conceder permissões explícitas a delegados para exibir os eventos _particulares_ do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-109">Additionally, the owner can give explicit permissions to delegates to view the owner's _private_ events on the calendar.</span></span> 

<span data-ttu-id="9b3e5-110">Antes que o compartilhamento ou delegação de calendário entre em vigor, o proprietário envia um sharee ou delega um convite e o sharee ou o delegado aceita o convite ou adiciona explicitamente o calendário compartilhado ou delegado para acesso.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-110">Before calendar sharing or delegation can take effect, the owner sends a sharee or delegate an invitation, and the sharee or delegate accepts the invitation, or, explicitly adds the shared or delegated calendar for access.</span></span> <span data-ttu-id="9b3e5-111">O convite e a adição de um calendário compartilhado ou delegado ocorrem em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-111">The invitation and adding a shared or delegated calendar occur in an Outlook client.</span></span> 

<span data-ttu-id="9b3e5-112">Depois de configurar o compartilhamento ou a delegação no Outlook, os aplicativos poderão usar a API do Microsoft Graph para gerenciar o compartilhamento e a delegação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-112">After sharing or delegation is set up in Outlook, apps can then use the Microsoft Graph API to manage the sharing and delegation.</span></span>

<span data-ttu-id="9b3e5-113">O restante deste artigo baseia-se no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-113">The rest of this article is based on the following example scenario:</span></span>

- <span data-ttu-id="9b3e5-114">Alex Rodrigues delegou a Sara Melo seu calendário principal e também permitiu Sara para visualizar eventos privados nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-114">Alex Wilber has delegated Megan Bowen to his primary calendar, and also permitted Megan to view private events in that calendar.</span></span> 
- <span data-ttu-id="9b3e5-115">Alex compartilhou no calendário o evento "festa das crianças" com Adele Vance e Sara Melo, e atribuiu Adele e a Sara permissões `read` para todos os detalhes de eventos não privados no calendário "festas das crianças" e o status de disponibilidade para eventos privados.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-115">Alex shared a "Kids parties" calendar with Adele Vance and Megan Bowen, and gave both Adele and Megan `read` permissions to all the details of non-private events on the "Kids parties" calendar, and free/busy status for private events.</span></span> 

<span data-ttu-id="9b3e5-116">Este artigo descreve programaticamente a execução das seguintes tarefas com um calendário compartilhado ou delegado:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-116">This article describes programmatically carrying out the following tasks with a shared or delegated calendar:</span></span>

- <span data-ttu-id="9b3e5-117">[Obtenha informações de calendário sobre compartilhamento, delegados e permissões permitidas e atualize permissões individuais](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-117">[Get calendar information about sharees, delegates, and allowed permissions, and update individual permissions](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span></span>
- <span data-ttu-id="9b3e5-118">[Obtenha as propriedades que descrevem o compartilhamento ou a delegação de calendário](#get-properties-of-a-shared-or-delegated-calendar).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-118">[Get the properties that describe the sharing or delegation of the calendar](#get-properties-of-a-shared-or-delegated-calendar).</span></span>
- <span data-ttu-id="9b3e5-119">[Obtenha ou defina a configuração de caixa de correio para receber solicitações de reunião e respostas para um calendário delegado](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-119">[Get or set mailbox setting to receive meeting requests and responses for a delegated calendar](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span></span>
- <span data-ttu-id="9b3e5-120">[Exclua um compartilhamento ou um representante de um calendário](#delete-a-sharee-or-delegate-of-a-calendar).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-120">[Delete a sharee or delegate of a calendar](#delete-a-sharee-or-delegate-of-a-calendar).</span></span>

<span data-ttu-id="9b3e5-121">Os aplicativos também podem fazer o seguinte usando a API que geralmente está disponível:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-121">Apps can also do the following using API that is generally available:</span></span>

- [<span data-ttu-id="9b3e5-122">Obter calendário do Outlook compartilhado ou delegado ou seus eventos</span><span class="sxs-lookup"><span data-stu-id="9b3e5-122">Get shared or delegated Outlook calendar or its events</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="9b3e5-123">Criar eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-123">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)

> [!NOTE]
> <span data-ttu-id="9b3e5-124">As propriedades e API para compartilhamento e delegação de calendário conforme descrito neste tópico estão disponíveis atualmente no ponto de extremidade v1.0, com exceção das propriedades de calendário **isShared** e **isSharedWithMe**.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-124">The properties and API for calendar sharing and delegating as described in this topic are currently available in the v1.0 endpoint, with the exception of the calendar properties **isShared** and **isSharedWithMe**.</span></span> <span data-ttu-id="9b3e5-125">Essas duas propriedades são expostas apenas no ponto de extremidade beta.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-125">These two properties are exposed in only the beta endpoint.</span></span>

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a><span data-ttu-id="9b3e5-126">Obtenha informações de calendário sobre compartilhamento, delegados e permissões permitidas e atualize permissões individuais.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-126">Get calendar information about sharees and delegates, and update individual permissions</span></span>

<span data-ttu-id="9b3e5-127">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-127">In this section:</span></span>

- [<span data-ttu-id="9b3e5-128">Proprietário do calendário: obter informações e permissões de compartilhamento e delegação</span><span class="sxs-lookup"><span data-stu-id="9b3e5-128">Calendar owner: Get sharing or delegation information and permissions</span></span>](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [<span data-ttu-id="9b3e5-129">Proprietário do calendário: atualizar permissões para um compartilhamento existente ou delegado em um calendário</span><span class="sxs-lookup"><span data-stu-id="9b3e5-129">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

<span data-ttu-id="9b3e5-130">Todos os calendários estão associados a um conjunto de objetos [calendarPermission](/graph/api/resources/calendarpermission), cada um deles descreve um compartilhamento ou delegado e a permissão associada que o proprietário do calendário configurou.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-130">Each calendar is associated with a collection of [calendarPermission](/graph/api/resources/calendarpermission) objects, each of which describes a sharee or delegate and the associated permission that the calendar owner has set up.</span></span> <span data-ttu-id="9b3e5-131">A enumeração [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) define o intervalo de permissões que o Microsoft Graph dá suporte:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-131">The [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) enumeration defines the range of permissions that Microsoft Graph supports:</span></span>

- <span data-ttu-id="9b3e5-132">`none` Esse valor se aplica somente a `My Organization` que não tem permissões para o calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-132">`none` This value applies to only `My Organization` which does not have any permissions to the calendar.</span></span> <span data-ttu-id="9b3e5-133">Isso não se aplica a usuários individuais, pois somente os usuários com permissões estão associados a um objeto **calendarPermission** para o calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-133">It doesn't apply to individual users, as only users with permissions are associated with a **calendarPermission** object for the calendar.</span></span>
- <span data-ttu-id="9b3e5-134">`freeBusyRead` O sharee pode exibir o status de disponibilidade do proprietário, mas não outros detalhes no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-134">`freeBusyRead` The sharee can view the owner's free/busy status, but not other details on the calendar.</span></span>
- <span data-ttu-id="9b3e5-135">`limitedRead` O sharee pode exibir o status de disponibilidade do proprietário e os títulos e locais de eventos não privados no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-135">`limitedRead` The sharee can view the owner's free/busy status, and the titles and locations of non-private events on the calendar.</span></span>
- <span data-ttu-id="9b3e5-136">`read` O sharee pode visualizar o status de disponibilidade do proprietário em eventos privados e todos os detalhes de eventos não privados no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-136">`read` The sharee can view the owner's free/busy status in private events, and all the details of non-private events on the calendar.</span></span>
- <span data-ttu-id="9b3e5-137">`write` O sharee pode visualizar o status de disponibilidade do proprietário em eventos privados e pode exibir todos os detalhes e editar (criar, atualizar ou excluir) eventos não privados no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-137">`write` The sharee can view the owner's free/busy status in private events, and can view all the details and edit (create, update, or delete) non-private events on the calendar.</span></span>
- <span data-ttu-id="9b3e5-138">`delegateWithoutPrivateEventAccess` O _delegado_ pode visualizar o status de disponibilidade do proprietário em eventos privados e tem `write` acesso a eventos não privados no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-138">`delegateWithoutPrivateEventAccess` The _delegate_ can view the owner's free/busy status in private events, and has `write` access to non-private events on the calendar.</span></span>
- <span data-ttu-id="9b3e5-139">`delegateWithPrivateEventAccess` O _delegado_ pode visualizar o status de disponibilidade do proprietário em eventos privados e tem acesso `write` a eventos não privados no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-139">`delegateWithPrivateEventAccess` The _delegate_ can view details of the owner's private and non-private events, and has `write` access to all the events on the calendar.</span></span>

<span data-ttu-id="9b3e5-140">O calendário principal de um usuário sempre é compartilhado com a "Minha Organização", que representa os usuários na mesma organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-140">The primary calendar of a user is always shared with "My Organization", which represents the users in the same organization as the owner.</span></span> <span data-ttu-id="9b3e5-141">Por padrão, eles podem ler o status de disponibilidade do proprietário no calendário e ter a permissão `freeBusyRead`.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-141">By default, they can read the owner's free/busy status on that calendar and have the `freeBusyRead` permission.</span></span>


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a><span data-ttu-id="9b3e5-142">Proprietário do calendário: obter informações e permissões de compartilhamento e delegação</span><span class="sxs-lookup"><span data-stu-id="9b3e5-142">Calendar owner: Get sharing or delegation information and permissions</span></span>

<span data-ttu-id="9b3e5-143">Este exemplo mostra com o consentimento de Alex ou administrador, como obter os objetos **calendarPermission** associados ao calendário principal de Alex.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-143">This example shows with the consent of Alex or administrator, how to get the **calendarPermission** objects associated with Alex' primary calendar.</span></span> <span data-ttu-id="9b3e5-144">A solicitação retorna dois objetos de permissão:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-144">The request returns two such permission objects:</span></span>

- <span data-ttu-id="9b3e5-145">O primeiro objeto **calendarPermission** é atribuído ao delegado, Sara, e tem os seguintes valores de propriedade:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-145">The first **calendarPermission** object is assigned to the delegate, Megan, and has the following property values:</span></span>

  - <span data-ttu-id="9b3e5-146">**isRemovable** está definida como true, o que permite a cancelamento de uma delegação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-146">**isRemovable** is set to true, providing Alex the option to cancel the delegation.</span></span>
  - <span data-ttu-id="9b3e5-147">**isInsideOrganization** é verdadeiro, pois somente os usuários na mesma organização podem ser delegados.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-147">**isInsideOrganization** is true as only users in the same organization can be delegates.</span></span>
  - <span data-ttu-id="9b3e5-148">**a função** de Sara é `delegateWithPrivateEventAccess`, conforme configurado por Alex.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-148">**role** for Megan is `delegateWithPrivateEventAccess`, as set up by Alex.</span></span>
  - <span data-ttu-id="9b3e5-149">**allowedRoles** inclui os tipos de função `delegateWithoutPrivateEventAccess`e`delegateWithPrivateEventAccess` que oferecem suporte à delegação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-149">**allowedRoles** includes the role types `delegateWithoutPrivateEventAccess` and `delegateWithPrivateEventAccess` that support delegation.</span></span>
  - <span data-ttu-id="9b3e5-150">**emailAddress** especifica Sara.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-150">**emailAddress** specifies Megan.</span></span>

- <span data-ttu-id="9b3e5-151">O segundo objeto **calendarPermission** é um objeto padrão atribuído a "My Organization" e tem os seguintes valores de propriedade:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-151">The second **calendarPermission** object is a default object assigned to "My Organization", and has the following property values:</span></span>

  - <span data-ttu-id="9b3e5-152">**isRemovable** está definido como falso, uma vez que o calendário principal é sempre compartilhado com a organização do proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-152">**isRemovable** is set to false, since the primary calendar is always shared with the owner's organization.</span></span>
  - <span data-ttu-id="9b3e5-153">**isInsideOrganization** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-153">**isInsideOrganization** is true.</span></span>
  - <span data-ttu-id="9b3e5-154">**a função** é`freeBusyRead`, a configuração padrão para "My Organization".</span><span class="sxs-lookup"><span data-stu-id="9b3e5-154">**role** is `freeBusyRead`, the default setting for "My Organization".</span></span>
  - <span data-ttu-id="9b3e5-155">**emailAddress** especifica a subpropriedade **name** como "My Organization"; o **endereço** de "My Organization" é nulo.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-155">**emailAddress** specifies the **name** sub-property as "My Organization"; **address** for "My Organization" is by default null.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-156">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-156">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-157">Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.Read`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-157">Use the least privileged delegated or application permission, `Calendars.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-158">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-158">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-160">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarperms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarperms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarperms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendarperms",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/calendarPermissions",
    "value": [
        {
            "id": "L289RXhjaGFuZ2VMYWJTWVnYW5C",
            "isRemovable": true,
            "isInsideOrganization": true,
            "role": "delegateWithPrivateEventAccess",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read",
                "write",
                "delegateWithoutPrivateEventAccess",
                "delegateWithPrivateEventAccess"
            ],
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a><span data-ttu-id="9b3e5-163">Proprietário do calendário: atualizar permissões para um sharee existente ou delegado em um calendário</span><span class="sxs-lookup"><span data-stu-id="9b3e5-163">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>

<span data-ttu-id="9b3e5-164">Com o consentimento de Alex ou do administrador, você pode atualizar as permissões atribuídas a um compartilhamento ou delegado existente (especificado pela propriedade **função**), contanto que as novas permissões sejam compatíveis com **allowedRoles** configurado inicialmente para o sharee ou o delegado desse calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-164">With the consent of Alex or administrator, you can update the permissions assigned to an existing sharee or delegate (specified by the **role** property), as long as the new permissions are supported by those **allowedRoles** set up initially for the sharee or delegate for that calendar.</span></span> 

<span data-ttu-id="9b3e5-165">Com exceção da propriedade **função**, você não pode atualizar outras propriedades de um sharee ou delegado existente.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-165">Aside from the **role** property, you cannot update other properties of an existing sharee or delegate.</span></span> <span data-ttu-id="9b3e5-166">Alterar o valor da propriedade **emailAddress** exige a exclusão do compartilhamento ou do representante e a configuração de uma nova instância do **calendarPermission** novamente.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-166">Changing the **emailAddress** property value requires deleting the sharee or delegate and setting up a new instance of **calendarPermission** again.</span></span>

<span data-ttu-id="9b3e5-167">O exemplo nesta seção atualiza a propriedade **função**, alterando a permissão de um sharee existente, Adele, de `read` para `write` para o calendário personalizado "Festas infantis".</span><span class="sxs-lookup"><span data-stu-id="9b3e5-167">The example in this section updates the **role** property, changing the permission of an existing sharee, Adele, from `read` to `write` for the custom calendar "Kids parties".</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-168">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-168">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-169">Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.ReadWrite`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-169">Use the least privileged delegated or application permission, `Calendars.ReadWrite`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-170">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-170">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarperm",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJQWRlbGVW"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-172">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarperm-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarperm-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarperm-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "update_calendarperm",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AAMkADAwAABf02bAAAA%3D')/calendarPermissions/$entity",
    "id": "L289RXhjaGFuZ2VMYWJQWRlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="9b3e5-175">Obter propriedades de um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-175">Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="9b3e5-176">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-176">In this section:</span></span>

- [<span data-ttu-id="9b3e5-177">Proprietário do calendário: Obter propriedades de um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-177">Calendar owner: Get properties of a shared or delegated calendar</span></span>](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [<span data-ttu-id="9b3e5-178">Compartilhar ou delegar: obter propriedades de calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-178">Sharee or delegate: Get properties of shared or delegated calendar</span></span>](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

<span data-ttu-id="9b3e5-179">Lembrando deste exemplo, Alex delegou seu calendário principal e concedeu à delegada, Sara Melo, a permissão para exibir itens de calendário marcados como particulares.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-179">Recalling in this example, Alex has delegated his primary calendar and given the delegate, Megan Bowen, the permission to view calendar items that are marked private.</span></span>
<span data-ttu-id="9b3e5-180">Esta seção mostra as propriedades do calendário delegado, primeiro a partir da perspectiva de e com o consentimento do proprietário, Alex, da perspectiva de e com o consentimento da delegada, Sara.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-180">This section shows the properties of the delegated calendar, first from the perspective of and with the consent of the owner, Alex, and then from the perspective of and with the consent of the delegate, Megan.</span></span> <span data-ttu-id="9b3e5-181">O consentimento do administrador também funciona para todos os casos.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-181">Consent from the administrator also works for each case.</span></span>

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="9b3e5-182">Proprietário do calendário: Obter propriedades de um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-182">Calendar owner: Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="9b3e5-183">O exemplo nesta seção obtém as propriedades do calendário principal da perspectiva do proprietário, Alex.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-183">The example in this section gets the properties of the primary calendar from the perspective of the owner, Alex.</span></span> 

<span data-ttu-id="9b3e5-184">Observe as seguintes propriedades de Alex:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-184">Note the following properties on Alex' behalf:</span></span>

- <span data-ttu-id="9b3e5-185">**canshare** é verdadeiro, pois Alex é o proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-185">**canShare** is true as Alex is the owner.</span></span>
- <span data-ttu-id="9b3e5-186">**canViewPrivateItems** é verdadeiro, uma vez que Alex é o proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-186">**canViewPrivateItems** is true since Alex is the owner.</span></span>
- <span data-ttu-id="9b3e5-187">**isShared** é definido como verdadeiro, uma vez que o Alex configurou um delegado para este calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-187">**isShared** is set to true, as Alex has set up a delegate for this calendar.</span></span>
- <span data-ttu-id="9b3e5-188">**isSharedWithMe** é sempre falso para o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-188">**isSharedWithMe** is always false for the calendar owner.</span></span>
- <span data-ttu-id="9b3e5-189">**owner** mostra Alex como proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-189">**owner** shows Alex as the owner.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-190">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-190">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-191">Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.Read`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-191">Use the least privileged delegated or application permission, `Calendars.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-192">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-192">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-194">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAw7QAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": true,
    "isSharedWithMe": false,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a><span data-ttu-id="9b3e5-197">Compartilhar ou delegar: obter propriedades de calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-197">Sharee or delegate: Get properties of shared or delegated calendar</span></span>

<span data-ttu-id="9b3e5-198">O exemplo nesta seção obtém as propriedades do mesmo calendário da perspectiva da delegada, Sara.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-198">The example in this section gets the properties of the same calendar from the perspective of the delegate, Megan.</span></span> 

<span data-ttu-id="9b3e5-199">Observe as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-199">Note the following properties:</span></span>

- <span data-ttu-id="9b3e5-200">**nome** do calendário é, por padrão, o nome de exibição do proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-200">**name** of the calendar is by default the owner's display name.</span></span> <span data-ttu-id="9b3e5-201">Nesse caso, é "Alex Rodrigues", já que o calendário de Alex, foi delegado a Sara.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-201">In this case, it's "Alex Wilber", since this is Alex' calendar delegated to Megan.</span></span> 
- <span data-ttu-id="9b3e5-202">**canShare** é falso, uma vez que Sara não é a proprietária do calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-202">**canShare** is false, since Megan is not the owner of this calendar.</span></span>
- <span data-ttu-id="9b3e5-203">**canViewPrivateItems** é verdadeiro para a delegada Sara, conforme configurado por Alex.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-203">**canViewPrivateItems** is true for the delegate Megan, as set up by Alex.</span></span> <span data-ttu-id="9b3e5-204">Para um sharee que não seja um delegado essa propriedade será sempre falsa.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-204">For a sharee that is not a delegate, this property is always false.</span></span>
- <span data-ttu-id="9b3e5-205">**isShared** é falso.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-205">**isShared** is false.</span></span> <span data-ttu-id="9b3e5-206">Esta propriedade indica apenas ao _proprietário_ do calendário se o calendário foi compartilhado ou delegado.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-206">This property indicates only to a calendar _owner_ whether the calendar has been shared or delegated.</span></span>
- <span data-ttu-id="9b3e5-207">A propriedade **isSharedWithMe** é verdadeira, uma vez que Sara é uma delegada.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-207">**isSharedWithMe** property is true, since Megan is a delegate.</span></span>
- <span data-ttu-id="9b3e5-208">**CanEdit** é verdadeiro, uma vez que os delegados, incluindo Sara, têm acesso de gravação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-208">**canEdit** is true, since delegates, including Megan, have write access.</span></span>
- <span data-ttu-id="9b3e5-209">**owner** está definido como Alex.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-209">**owner** is set to Alex.</span></span>

> [!NOTE] 
> <span data-ttu-id="9b3e5-210">Um compartilhamento ou representante só pode personalizar a propriedade **nome** de um calendário compartilhado/delegado.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-210">A sharee or delegate can customize only the **name** property of a shared/delegated calendar.</span></span> <span data-ttu-id="9b3e5-211">A atualização é visível apenas para eles mesmos; o proprietário do calendário não vê essas alterações no nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-211">The update is visible only to themselves; the calendar owner does not see such calendar name changes.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-212">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-212">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-213">Use a permissão delegada com menos privilégios, `Calendars.Read.Shared`, ou permissão de aplicativo, `Calendars.Read`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-213">Use the least privileged delegated permission, `Calendars.Read.Shared`, or application permission, `Calendars.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-214">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-214">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-216">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-delegate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-delegate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-delegate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_delegate",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('meganb%40contoso.OnMicrosoft.com')/calendars/$entity",
    "id": "AAMkADlAABhbftjAAA=",
    "name": "Alex Wilber",
    "color": "auto",
    "hexColor": "",
    "changeKey": "E6LznKWmX0KTsAD9qRJjeAAAYWo3EQ==",
    "canShare": false,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": true,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": true,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a><span data-ttu-id="9b3e5-219">Obtenha ou defina a configuração de caixa de correio para receber solicitações de reunião e respostas</span><span class="sxs-lookup"><span data-stu-id="9b3e5-219">Get or set mailbox setting to receive meeting requests and responses</span></span>

<span data-ttu-id="9b3e5-220">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-220">In this section:</span></span>

- [<span data-ttu-id="9b3e5-221">Obter a configuração de entrega de delegação para a caixa de correio de um usuário</span><span class="sxs-lookup"><span data-stu-id="9b3e5-221">Get delegation delivery setting for a user's mailbox</span></span>](#get-delegation-delivery-setting-for-a-users-mailbox)
- [<span data-ttu-id="9b3e5-222">Definir a configuração de entrega de delegação para a caixa de correio de um usuário</span><span class="sxs-lookup"><span data-stu-id="9b3e5-222">Set delegation delivery setting for a user's mailbox</span></span>](#set-delegation-delivery-setting-for-a-users-mailbox)

<span data-ttu-id="9b3e5-223">Dependendo do nível de delegação que um proprietário de calendário prefere, o proprietário poderá especificar quem deve receber solicitações de reunião e respostas para gerenciar as reuniões no calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-223">Depending on the level of delegation a calendar owner prefers, the owner can specify who should receive meeting requests and responses to manage meetings on the calendar.</span></span> 

<span data-ttu-id="9b3e5-224">Programaticamente, você pode obter ou definir a propriedade **delegateMeetingMessageDeliveryOptions** do proprietário do calendário [mailboxSettings](/graph/api/resources/mailboxsettings) para especificar para quem o Outlook deve direcionar as instâncias [eventMessageRequest](/graph/api/resources/eventmessagerequest) e [eventMessageResponse](/graph/api/resources/eventmessageresponse):</span><span class="sxs-lookup"><span data-stu-id="9b3e5-224">Programmatically, you can get or set the **delegateMeetingMessageDeliveryOptions** property of the calendar owner's [mailboxSettings](/graph/api/resources/mailboxsettings) to specify to whom Outlook should direct [eventMessageRequest](/graph/api/resources/eventmessagerequest) and [eventMessageResponse](/graph/api/resources/eventmessageresponse) instances:</span></span>

- `sendToDelegateOnly`

    <span data-ttu-id="9b3e5-225">O Outlook para direcionar as instâncias **eventMessageRequest** e **eventMessageResponse** para delegados.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-225">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to only delegates.</span></span> <span data-ttu-id="9b3e5-226">Esta é a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-226">This is the default setting.</span></span> <span data-ttu-id="9b3e5-227">O proprietário pode ver as respostas a uma reunião ou responder a um convite através do **evento** correspondente no calendário delegado.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-227">The owner can see responses to a meeting or respond to an invitation through the corresponding **event** in the delegated calendar.</span></span>
- `sendToDelegateAndInformationToPrincipal`

    <span data-ttu-id="9b3e5-228">O Outlook direciona as instâncias **eventMessageRequest** e **eventMessageResponse** para delegados e para o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-228">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner.</span></span> <span data-ttu-id="9b3e5-229">Somente os representantes veem a opção de aceitar ou recusar uma solicitação de reunião, e a notificação enviada ao proprietário aparece como uma mensagem de e-mail normal.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-229">Only the delegates see the option to accept or decline a meeting request, and the notification sent to the owner appears like a normal email message.</span></span> <span data-ttu-id="9b3e5-230">O proprietário ainda pode responder à reunião, abrindo o **evento** no calendário delegado e respondendo.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-230">The owner can still respond to the meeting by opening the **event** in the delegated calendar and responding.</span></span>
- `sendToDelegateAndPrincipal`

    <span data-ttu-id="9b3e5-231">O Outlook direciona as instâncias **eventMessageRequest** e **eventMessageResponse** para delegados e para o proprietário do calendário, ou seja, que podem responder à solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-231">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner, either of whom can respond to the meeting request.</span></span>

<span data-ttu-id="9b3e5-232">Essa é uma configuração para toda a caixa de correio; portanto, a mesma configuração se aplica a todos os delegados do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-232">This is a mailbox-wide setting, so the same setting applies to all delegates of the mailbox owner.</span></span>

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="9b3e5-233">Obter a configuração de entrega de delegação para a caixa de correio de um usuário</span><span class="sxs-lookup"><span data-stu-id="9b3e5-233">Get delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="9b3e5-234">O exemplo nesta seção obtém as **mailboxSettings** de um proprietário de calendário que permite que o Outlook direcione solicitações e respostas de reunião apenas para delegados de calendário; ou seja, **delegateMeetingMessageDeliveryOptions** é definido como `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-234">The example in this section gets the **mailboxSettings** of a calendar owner who lets Outlook direct meeting requests and responses to only calendar delegates; that is, **delegateMeetingMessageDeliveryOptions** is set to `sendToDelegateOnly`.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-235">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-235">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-236">Use a permissão delegada ou de aplicativo com menos privilégios, `MailboxSettings.Read`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-236">Use the least privileged delegated or application permission, `MailboxSettings.Read`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-237">Para obter mais informações sobre permissões de caixa de correio, confira [permissões de email](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-237">For more information about mailbox permissions, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-238">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-238">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-239">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-239">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-240">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-240">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-241">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-241">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "archiveFolder": "AQMkADAwAGVQAAAKfowAAAA==",
    "timeZone": "Pacific Standard Time",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly",
    "dateFormat": "M/d/yyyy",
    "timeFormat": "h:mm tt",
    "automaticRepliesSetting": {
        "status": "disabled",
        "externalAudience": "all",
        "internalReplyMessage": "",
        "externalReplyMessage": "",
        "scheduledStartDateTime": {
            "dateTime": "2019-12-24T05:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2019-12-25T05:00:00.0000000",
            "timeZone": "UTC"
        }
    },
    "language": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "workingHours": {
        "daysOfWeek": [
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone": {
            "name": "Pacific Standard Time"
        }
    }
}
```

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="9b3e5-242">Definir a configuração de entrega de delegação para a caixa de correio de um usuário</span><span class="sxs-lookup"><span data-stu-id="9b3e5-242">Set delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="9b3e5-243">O exemplo nesta seção atualiza a propriedade **delegateMeetingMessageDeliveryOptions** para `sendToDelegateAndPrincipal`, para que o Outlook direcione solicitações de reunião e respostas do calendário delegado para todos os delegados e o proprietário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-243">The example in this section updates the **delegateMeetingMessageDeliveryOptions** property to `sendToDelegateAndPrincipal`, to have Outlook direct meeting requests and responses of the delegated calendar to all delegates and the owner.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-244">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-244">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-245">Use a permissão delegada ou de aplicativo com menos privilégios, `MailboxSettings.ReadWrite`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-245">Use the least privileged delegated or application permission, `MailboxSettings.ReadWrite`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-246">Para obter mais informações sobre permissões de caixa de correio, confira [permissões de email](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-246">For more information about mailbox permissions, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-247">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
Content-type: application/json

{
  "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-248">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "patch_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a><span data-ttu-id="9b3e5-251">Exclua um compartilhamento ou um representante de um calendário.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-251">Delete a sharee or delegate of a calendar</span></span>

<span data-ttu-id="9b3e5-252">No exemplo abaixo, Alex exclui Sara como um sharee do calendário "Festas infantis".</span><span class="sxs-lookup"><span data-stu-id="9b3e5-252">In the example below, Alex deletes Megan as a sharee of the "Kids parties" calendar.</span></span>

#### <a name="microsoft-graph-permissions"></a><span data-ttu-id="9b3e5-253">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9b3e5-253">Microsoft Graph permissions</span></span>
<span data-ttu-id="9b3e5-254">Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.ReadWrite`, conforme apropriado, para esta operação.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-254">Use the least privileged delegated or application permission, `Calendars.ReadWrite`, as appropriate, for this operation.</span></span> <span data-ttu-id="9b3e5-255">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="9b3e5-255">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="9b3e5-256">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e5-256">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```
# <a name="c"></a>[<span data-ttu-id="9b3e5-257">C#</span><span class="sxs-lookup"><span data-stu-id="9b3e5-257">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharee-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b3e5-258">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b3e5-258">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharee-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b3e5-259">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b3e5-259">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sharee-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "delete_sharee",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="next-steps"></a><span data-ttu-id="9b3e5-260">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9b3e5-260">Next steps</span></span>

<span data-ttu-id="9b3e5-261">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-261">Find out more about:</span></span>

- <span data-ttu-id="9b3e5-262">Como os clientes do Outlook têm suporte para compartilhar e delegar calendários:</span><span class="sxs-lookup"><span data-stu-id="9b3e5-262">How the Outlook clients support sharing and delegating calendars:</span></span>
  - [<span data-ttu-id="9b3e5-263">Compartilhar um calendário do Outlook com outras pessoas </span><span class="sxs-lookup"><span data-stu-id="9b3e5-263">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [<span data-ttu-id="9b3e5-264">Permitir que outra pessoa gerencie o email e o calendário como delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-264">Allow someone else to manage your mail and calendar as a delegate</span></span>](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [<span data-ttu-id="9b3e5-265">Compartilhar seu calendário no Outlook na Web</span><span class="sxs-lookup"><span data-stu-id="9b3e5-265">Share your calendar in Outlook on the web</span></span>](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [<span data-ttu-id="9b3e5-266">Delegação de calendário no Outlook na Web</span><span class="sxs-lookup"><span data-stu-id="9b3e5-266">Calendar delegation in Outlook on the web</span></span>](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [<span data-ttu-id="9b3e5-267">Obter eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-267">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="9b3e5-268">Criar eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="9b3e5-268">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="9b3e5-269">Por que se integrar com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="9b3e5-269">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="9b3e5-270">A [API de calendário](/graph/api/resources/calendar) do Outlook no Microsoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="9b3e5-270">The [calendar API](/graph/api/resources/calendar) in Microsoft Graph beta.</span></span>
