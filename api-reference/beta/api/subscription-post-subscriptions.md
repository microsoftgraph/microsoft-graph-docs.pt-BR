---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: ba87a6e1ef5788994ffbb8d79f455d30b4a39acb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271439"
---
# <a name="create-subscription"></a><span data-ttu-id="877ea-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="877ea-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="877ea-104">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="877ea-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="877ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="877ea-105">Permissions</span></span>

<span data-ttu-id="877ea-106">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="877ea-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="877ea-107">Por exemplo, para obter notificações por mensagens, seu aplicativo precisa da `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="877ea-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="877ea-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="877ea-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="877ea-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="877ea-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="877ea-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-110">Supported resource</span></span> | <span data-ttu-id="877ea-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="877ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="877ea-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="877ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="877ea-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="877ea-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="877ea-114">contato</span><span class="sxs-lookup"><span data-stu-id="877ea-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="877ea-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-115">Contacts.Read</span></span> | <span data-ttu-id="877ea-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-116">Contacts.Read</span></span> | <span data-ttu-id="877ea-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-117">Contacts.Read</span></span> |
|<span data-ttu-id="877ea-118">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="877ea-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="877ea-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-119">Not supported</span></span> | <span data-ttu-id="877ea-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="877ea-120">Files.ReadWrite</span></span> | <span data-ttu-id="877ea-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-121">Not supported</span></span> |
|<span data-ttu-id="877ea-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="877ea-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="877ea-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877ea-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="877ea-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-124">Not supported</span></span> | <span data-ttu-id="877ea-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877ea-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="877ea-126">evento</span><span class="sxs-lookup"><span data-stu-id="877ea-126">event</span></span>](../resources/event.md) | <span data-ttu-id="877ea-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-127">Calendars.Read</span></span> | <span data-ttu-id="877ea-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-128">Calendars.Read</span></span> | <span data-ttu-id="877ea-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-129">Calendars.Read</span></span> |
|[<span data-ttu-id="877ea-130">grupo</span><span class="sxs-lookup"><span data-stu-id="877ea-130">group</span></span>](../resources/group.md) | <span data-ttu-id="877ea-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="877ea-131">Group.Read.All</span></span> | <span data-ttu-id="877ea-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-132">Not supported</span></span> | <span data-ttu-id="877ea-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="877ea-133">Group.Read.All</span></span> |
|[<span data-ttu-id="877ea-134">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="877ea-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="877ea-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="877ea-135">Group.Read.All</span></span> | <span data-ttu-id="877ea-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-136">Not supported</span></span> | <span data-ttu-id="877ea-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-137">Not supported</span></span> |
|[<span data-ttu-id="877ea-138">mensagem</span><span class="sxs-lookup"><span data-stu-id="877ea-138">message</span></span>](../resources/message.md) | <span data-ttu-id="877ea-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-139">Mail.Read</span></span> | <span data-ttu-id="877ea-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-140">Mail.Read</span></span> | <span data-ttu-id="877ea-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="877ea-141">Mail.Read</span></span> |
|[<span data-ttu-id="877ea-142">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="877ea-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="877ea-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877ea-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="877ea-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="877ea-144">Not supported</span></span> | <span data-ttu-id="877ea-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877ea-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="877ea-146">Usuário</span><span class="sxs-lookup"><span data-stu-id="877ea-146">user</span></span>](../resources/user.md) | <span data-ttu-id="877ea-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="877ea-147">User.Read.All</span></span> | <span data-ttu-id="877ea-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="877ea-148">User.Read.All</span></span> | <span data-ttu-id="877ea-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="877ea-149">User.Read.All</span></span> |

> <span data-ttu-id="877ea-150">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="877ea-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="877ea-151">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="877ea-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="877ea-152">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="877ea-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="877ea-153">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="877ea-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="877ea-154">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="877ea-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="877ea-155">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="877ea-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="877ea-156">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="877ea-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="877ea-157">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="877ea-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="877ea-158">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="877ea-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="877ea-159">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="877ea-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="877ea-160">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="877ea-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="877ea-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="877ea-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="877ea-162">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="877ea-162">Request headers</span></span>

| <span data-ttu-id="877ea-163">Nome</span><span class="sxs-lookup"><span data-stu-id="877ea-163">Name</span></span>       | <span data-ttu-id="877ea-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="877ea-164">Type</span></span> | <span data-ttu-id="877ea-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="877ea-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="877ea-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="877ea-166">Authorization</span></span>  | <span data-ttu-id="877ea-167">string</span><span class="sxs-lookup"><span data-stu-id="877ea-167">string</span></span>  | <span data-ttu-id="877ea-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="877ea-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="877ea-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="877ea-170">Response</span></span>

<span data-ttu-id="877ea-171">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="877ea-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="877ea-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="877ea-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="877ea-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="877ea-173">Request</span></span>

<span data-ttu-id="877ea-174">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="877ea-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="877ea-175">Esse `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="877ea-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="877ea-176">Este exemplo de solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="877ea-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="877ea-177">Estes são os valores válidos para a propriedade de recurso:</span><span class="sxs-lookup"><span data-stu-id="877ea-177">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="877ea-178">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="877ea-178">Resource type</span></span> | <span data-ttu-id="877ea-179">Exemplos</span><span class="sxs-lookup"><span data-stu-id="877ea-179">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="877ea-180">Email</span><span class="sxs-lookup"><span data-stu-id="877ea-180">Mail</span></span>|<span data-ttu-id="877ea-181">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="877ea-181">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="877ea-182">me/messages</span><span class="sxs-lookup"><span data-stu-id="877ea-182">me/messages</span></span>|
|<span data-ttu-id="877ea-183">Contatos</span><span class="sxs-lookup"><span data-stu-id="877ea-183">Contacts</span></span>|<span data-ttu-id="877ea-184">me/contacts</span><span class="sxs-lookup"><span data-stu-id="877ea-184">me/contacts</span></span>|
|<span data-ttu-id="877ea-185">Calendários</span><span class="sxs-lookup"><span data-stu-id="877ea-185">Calendars</span></span>|<span data-ttu-id="877ea-186">me/events</span><span class="sxs-lookup"><span data-stu-id="877ea-186">me/events</span></span>|
|<span data-ttu-id="877ea-187">Usuários</span><span class="sxs-lookup"><span data-stu-id="877ea-187">Users</span></span>|<span data-ttu-id="877ea-188">usuários</span><span class="sxs-lookup"><span data-stu-id="877ea-188">users</span></span>|
|<span data-ttu-id="877ea-189">Grupos</span><span class="sxs-lookup"><span data-stu-id="877ea-189">Groups</span></span>|<span data-ttu-id="877ea-190">grupos</span><span class="sxs-lookup"><span data-stu-id="877ea-190">groups</span></span>|
|<span data-ttu-id="877ea-191">Conversas</span><span class="sxs-lookup"><span data-stu-id="877ea-191">Conversations</span></span>|<span data-ttu-id="877ea-192">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="877ea-192">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="877ea-193">Unidades</span><span class="sxs-lookup"><span data-stu-id="877ea-193">Drives</span></span>|<span data-ttu-id="877ea-194">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="877ea-194">me/drive/root</span></span>|
|<span data-ttu-id="877ea-195">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="877ea-195">Security alert</span></span>|<span data-ttu-id="877ea-196">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="877ea-196">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="877ea-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="877ea-197">Response</span></span>

<span data-ttu-id="877ea-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="877ea-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="877ea-201">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="877ea-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="877ea-202">C#</span><span class="sxs-lookup"><span data-stu-id="877ea-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_subscription_from_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="877ea-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="877ea-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_subscription_from_subscriptions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="877ea-204">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="877ea-204">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_subscription_from_subscriptions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="notification-endpoint-validation"></a><span data-ttu-id="877ea-205">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="877ea-205">Notification endpoint validation</span></span>

<span data-ttu-id="877ea-206">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="877ea-206">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="877ea-207">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="877ea-207">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
