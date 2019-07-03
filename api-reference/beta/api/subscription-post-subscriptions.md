---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: b23cfa1eec29ed77f822cdaa0ff3073100df722b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458196"
---
# <a name="create-subscription"></a><span data-ttu-id="3ce47-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="3ce47-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce47-104">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3ce47-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ce47-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ce47-105">Permissions</span></span>

<span data-ttu-id="3ce47-106">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ce47-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="3ce47-107">Por exemplo, para obter notificações por mensagens, seu aplicativo precisa da `Mail.Read` permissão.</span><span class="sxs-lookup"><span data-stu-id="3ce47-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="3ce47-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="3ce47-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3ce47-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ce47-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ce47-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-110">Supported resource</span></span> | <span data-ttu-id="3ce47-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ce47-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ce47-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ce47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ce47-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ce47-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="3ce47-114">contato</span><span class="sxs-lookup"><span data-stu-id="3ce47-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="3ce47-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-115">Contacts.Read</span></span> | <span data-ttu-id="3ce47-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-116">Contacts.Read</span></span> | <span data-ttu-id="3ce47-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-117">Contacts.Read</span></span> |
|<span data-ttu-id="3ce47-118">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="3ce47-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="3ce47-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-119">Not supported</span></span> | <span data-ttu-id="3ce47-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ce47-120">Files.ReadWrite</span></span> | <span data-ttu-id="3ce47-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-121">Not supported</span></span> |
|<span data-ttu-id="3ce47-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="3ce47-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="3ce47-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="3ce47-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-124">Not supported</span></span> | <span data-ttu-id="3ce47-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ce47-126">evento</span><span class="sxs-lookup"><span data-stu-id="3ce47-126">event</span></span>](../resources/event.md) | <span data-ttu-id="3ce47-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-127">Calendars.Read</span></span> | <span data-ttu-id="3ce47-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-128">Calendars.Read</span></span> | <span data-ttu-id="3ce47-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-129">Calendars.Read</span></span> |
|[<span data-ttu-id="3ce47-130">grupo</span><span class="sxs-lookup"><span data-stu-id="3ce47-130">group</span></span>](../resources/group.md) | <span data-ttu-id="3ce47-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-131">Group.Read.All</span></span> | <span data-ttu-id="3ce47-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-132">Not supported</span></span> | <span data-ttu-id="3ce47-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-133">Group.Read.All</span></span> |
|[<span data-ttu-id="3ce47-134">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="3ce47-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="3ce47-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-135">Group.Read.All</span></span> | <span data-ttu-id="3ce47-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-136">Not supported</span></span> | <span data-ttu-id="3ce47-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-137">Not supported</span></span> |
|[<span data-ttu-id="3ce47-138">mensagem</span><span class="sxs-lookup"><span data-stu-id="3ce47-138">message</span></span>](../resources/message.md) | <span data-ttu-id="3ce47-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-139">Mail.Read</span></span> | <span data-ttu-id="3ce47-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-140">Mail.Read</span></span> | <span data-ttu-id="3ce47-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ce47-141">Mail.Read</span></span> |
|[<span data-ttu-id="3ce47-142">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="3ce47-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="3ce47-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="3ce47-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3ce47-144">Not supported</span></span> | <span data-ttu-id="3ce47-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ce47-146">Usuário</span><span class="sxs-lookup"><span data-stu-id="3ce47-146">user</span></span>](../resources/user.md) | <span data-ttu-id="3ce47-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-147">User.Read.All</span></span> | <span data-ttu-id="3ce47-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-148">User.Read.All</span></span> | <span data-ttu-id="3ce47-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce47-149">User.Read.All</span></span> |

> <span data-ttu-id="3ce47-150">**Observação:** Há limitações adicionais para assinaturas de itens no OneDrive e no Outlook.</span><span class="sxs-lookup"><span data-stu-id="3ce47-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="3ce47-151">Limitações para criar e gerenciar assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="3ce47-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="3ce47-152">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="3ce47-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="3ce47-153">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="3ce47-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="3ce47-154">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="3ce47-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="3ce47-155">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="3ce47-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="3ce47-156">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3ce47-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="3ce47-157">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="3ce47-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="3ce47-158">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="3ce47-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="3ce47-159">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="3ce47-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="3ce47-160">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="3ce47-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ce47-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce47-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="3ce47-162">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce47-162">Request headers</span></span>

| <span data-ttu-id="3ce47-163">Nome</span><span class="sxs-lookup"><span data-stu-id="3ce47-163">Name</span></span>       | <span data-ttu-id="3ce47-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ce47-164">Type</span></span> | <span data-ttu-id="3ce47-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce47-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ce47-166">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ce47-166">Authorization</span></span>  | <span data-ttu-id="3ce47-167">string</span><span class="sxs-lookup"><span data-stu-id="3ce47-167">string</span></span>  | <span data-ttu-id="3ce47-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ce47-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3ce47-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ce47-170">Response</span></span>

<span data-ttu-id="3ce47-171">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ce47-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce47-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ce47-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ce47-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce47-173">Request</span></span>

<span data-ttu-id="3ce47-174">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="3ce47-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="3ce47-175">Esse `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="3ce47-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="3ce47-176">Este exemplo de solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="3ce47-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3ce47-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce47-177">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ce47-178">C#</span><span class="sxs-lookup"><span data-stu-id="3ce47-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ce47-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ce47-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ce47-180">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3ce47-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3ce47-181">Estes são os valores válidos para a propriedade de recurso:</span><span class="sxs-lookup"><span data-stu-id="3ce47-181">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="3ce47-182">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="3ce47-182">Resource type</span></span> | <span data-ttu-id="3ce47-183">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ce47-183">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="3ce47-184">Email</span><span class="sxs-lookup"><span data-stu-id="3ce47-184">Mail</span></span>|<span data-ttu-id="3ce47-185">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="3ce47-185">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="3ce47-186">me/messages</span><span class="sxs-lookup"><span data-stu-id="3ce47-186">me/messages</span></span>|
|<span data-ttu-id="3ce47-187">Contatos</span><span class="sxs-lookup"><span data-stu-id="3ce47-187">Contacts</span></span>|<span data-ttu-id="3ce47-188">me/contacts</span><span class="sxs-lookup"><span data-stu-id="3ce47-188">me/contacts</span></span>|
|<span data-ttu-id="3ce47-189">Calendários</span><span class="sxs-lookup"><span data-stu-id="3ce47-189">Calendars</span></span>|<span data-ttu-id="3ce47-190">me/events</span><span class="sxs-lookup"><span data-stu-id="3ce47-190">me/events</span></span>|
|<span data-ttu-id="3ce47-191">Usuários</span><span class="sxs-lookup"><span data-stu-id="3ce47-191">Users</span></span>|<span data-ttu-id="3ce47-192">usuários</span><span class="sxs-lookup"><span data-stu-id="3ce47-192">users</span></span>|
|<span data-ttu-id="3ce47-193">Grupos</span><span class="sxs-lookup"><span data-stu-id="3ce47-193">Groups</span></span>|<span data-ttu-id="3ce47-194">grupos</span><span class="sxs-lookup"><span data-stu-id="3ce47-194">groups</span></span>|
|<span data-ttu-id="3ce47-195">Conversas</span><span class="sxs-lookup"><span data-stu-id="3ce47-195">Conversations</span></span>|<span data-ttu-id="3ce47-196">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="3ce47-196">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="3ce47-197">Unidades</span><span class="sxs-lookup"><span data-stu-id="3ce47-197">Drives</span></span>|<span data-ttu-id="3ce47-198">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="3ce47-198">me/drive/root</span></span>|
|<span data-ttu-id="3ce47-199">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="3ce47-199">Security alert</span></span>|<span data-ttu-id="3ce47-200">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="3ce47-200">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="3ce47-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ce47-201">Response</span></span>

<span data-ttu-id="3ce47-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ce47-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="3ce47-205">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="3ce47-205">Notification endpoint validation</span></span>

<span data-ttu-id="3ce47-206">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="3ce47-206">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="3ce47-207">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="3ce47-207">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
  ]
}
-->
