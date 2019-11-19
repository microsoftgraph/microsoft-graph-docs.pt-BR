---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c9926e294abb7ef616c90fafe6b8756228c55de6
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703795"
---
# <a name="create-subscription"></a><span data-ttu-id="46807-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="46807-103">Create subscription</span></span>

<span data-ttu-id="46807-104">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="46807-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="46807-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46807-105">Permissions</span></span>

 <span data-ttu-id="46807-106">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="46807-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="46807-107">Por exemplo, para obter notificações por mensagens, seu aplicativo precisa da `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="46807-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="46807-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="46807-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="46807-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46807-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46807-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="46807-110">Supported resource</span></span> | <span data-ttu-id="46807-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46807-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46807-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46807-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46807-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46807-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="46807-114">contato</span><span class="sxs-lookup"><span data-stu-id="46807-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="46807-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="46807-115">Contacts.Read</span></span> | <span data-ttu-id="46807-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="46807-116">Contacts.Read</span></span> | <span data-ttu-id="46807-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="46807-117">Contacts.Read</span></span> |
|<span data-ttu-id="46807-118">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="46807-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="46807-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-119">Not supported</span></span> | <span data-ttu-id="46807-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46807-120">Files.ReadWrite</span></span> | <span data-ttu-id="46807-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-121">Not supported</span></span> |
|<span data-ttu-id="46807-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="46807-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="46807-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="46807-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-124">Not supported</span></span> | <span data-ttu-id="46807-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="46807-126">evento</span><span class="sxs-lookup"><span data-stu-id="46807-126">event</span></span>](../resources/event.md) | <span data-ttu-id="46807-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="46807-127">Calendars.Read</span></span> | <span data-ttu-id="46807-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="46807-128">Calendars.Read</span></span> | <span data-ttu-id="46807-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="46807-129">Calendars.Read</span></span> |
|[<span data-ttu-id="46807-130">grupo</span><span class="sxs-lookup"><span data-stu-id="46807-130">group</span></span>](../resources/group.md) | <span data-ttu-id="46807-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="46807-131">Group.Read.All</span></span> | <span data-ttu-id="46807-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-132">Not supported</span></span> | <span data-ttu-id="46807-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="46807-133">Group.Read.All</span></span> |
|[<span data-ttu-id="46807-134">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="46807-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="46807-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="46807-135">Group.Read.All</span></span> | <span data-ttu-id="46807-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-136">Not supported</span></span> | <span data-ttu-id="46807-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-137">Not supported</span></span> |
|[<span data-ttu-id="46807-138">message</span><span class="sxs-lookup"><span data-stu-id="46807-138">message</span></span>](../resources/message.md) | <span data-ttu-id="46807-139">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="46807-139">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="46807-140">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="46807-140">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="46807-141">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="46807-141">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="46807-142">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="46807-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="46807-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="46807-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="46807-144">Not supported</span></span> | <span data-ttu-id="46807-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="46807-146">Usuário</span><span class="sxs-lookup"><span data-stu-id="46807-146">user</span></span>](../resources/user.md) | <span data-ttu-id="46807-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="46807-147">User.Read.All</span></span> | <span data-ttu-id="46807-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="46807-148">User.Read.All</span></span> | <span data-ttu-id="46807-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="46807-149">User.Read.All</span></span> |

> <span data-ttu-id="46807-150">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="46807-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="46807-151">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="46807-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="46807-152">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="46807-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="46807-153">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="46807-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="46807-154">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="46807-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="46807-155">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="46807-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="46807-156">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="46807-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="46807-157">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="46807-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="46807-158">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="46807-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="46807-159">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="46807-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="46807-160">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="46807-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="46807-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46807-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="46807-162">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46807-162">Request headers</span></span>

| <span data-ttu-id="46807-163">Nome</span><span class="sxs-lookup"><span data-stu-id="46807-163">Name</span></span>       | <span data-ttu-id="46807-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="46807-164">Type</span></span> | <span data-ttu-id="46807-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="46807-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46807-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="46807-166">Authorization</span></span>  | <span data-ttu-id="46807-167">string</span><span class="sxs-lookup"><span data-stu-id="46807-167">string</span></span>  | <span data-ttu-id="46807-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46807-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="46807-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="46807-170">Response</span></span>

<span data-ttu-id="46807-171">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46807-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46807-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46807-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="46807-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46807-173">Request</span></span>

<span data-ttu-id="46807-174">Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="46807-174">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46807-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="46807-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46807-176">C#</span><span class="sxs-lookup"><span data-stu-id="46807-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46807-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46807-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46807-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46807-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46807-179">Java</span><span class="sxs-lookup"><span data-stu-id="46807-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="46807-180">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="46807-180">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="46807-181">Esse `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="46807-181">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="46807-182">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="46807-182">Resources examples</span></span>

<span data-ttu-id="46807-183">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="46807-183">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="46807-184">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="46807-184">Resource type</span></span> | <span data-ttu-id="46807-185">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46807-185">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="46807-186">Email</span><span class="sxs-lookup"><span data-stu-id="46807-186">Mail</span></span>|<span data-ttu-id="46807-187">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="46807-187">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="46807-188">me/messages</span><span class="sxs-lookup"><span data-stu-id="46807-188">me/messages</span></span>|
|<span data-ttu-id="46807-189">Contatos</span><span class="sxs-lookup"><span data-stu-id="46807-189">Contacts</span></span>|<span data-ttu-id="46807-190">me/contacts</span><span class="sxs-lookup"><span data-stu-id="46807-190">me/contacts</span></span>|
|<span data-ttu-id="46807-191">Calendários</span><span class="sxs-lookup"><span data-stu-id="46807-191">Calendars</span></span>|<span data-ttu-id="46807-192">me/events</span><span class="sxs-lookup"><span data-stu-id="46807-192">me/events</span></span>|
|<span data-ttu-id="46807-193">Usuários</span><span class="sxs-lookup"><span data-stu-id="46807-193">Users</span></span>|<span data-ttu-id="46807-194">usuários</span><span class="sxs-lookup"><span data-stu-id="46807-194">users</span></span>|
|<span data-ttu-id="46807-195">Grupos</span><span class="sxs-lookup"><span data-stu-id="46807-195">Groups</span></span>|<span data-ttu-id="46807-196">grupos</span><span class="sxs-lookup"><span data-stu-id="46807-196">groups</span></span>|
|<span data-ttu-id="46807-197">Conversas</span><span class="sxs-lookup"><span data-stu-id="46807-197">Conversations</span></span>|<span data-ttu-id="46807-198">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="46807-198">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="46807-199">Unidades</span><span class="sxs-lookup"><span data-stu-id="46807-199">Drives</span></span>|<span data-ttu-id="46807-200">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="46807-200">me/drive/root</span></span>|
|<span data-ttu-id="46807-201">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="46807-201">Security alert</span></span>|<span data-ttu-id="46807-202">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="46807-202">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="46807-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="46807-203">Response</span></span>

<span data-ttu-id="46807-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46807-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="46807-207">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="46807-207">Notification endpoint validation</span></span>

<span data-ttu-id="46807-208">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="46807-208">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="46807-209">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="46807-209">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
