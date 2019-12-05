---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 4a5ffc3ec86c0ce40e4b5fca25b7f0ddcf5dca9f
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844173"
---
# <a name="create-subscription"></a><span data-ttu-id="160f3-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="160f3-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="160f3-104">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="160f3-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="160f3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="160f3-105">Permissions</span></span>

<span data-ttu-id="160f3-106">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="160f3-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="160f3-107">Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="160f3-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="160f3-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="160f3-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="160f3-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="160f3-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="160f3-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-110">Supported resource</span></span> | <span data-ttu-id="160f3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="160f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="160f3-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="160f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="160f3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="160f3-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="160f3-114">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="160f3-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="160f3-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-115">Not supported</span></span> | <span data-ttu-id="160f3-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-116">Not supported</span></span> | <span data-ttu-id="160f3-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="160f3-118">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="160f3-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="160f3-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-119">Not supported</span></span> | <span data-ttu-id="160f3-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-120">Not supported</span></span> | <span data-ttu-id="160f3-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="160f3-122">contato</span><span class="sxs-lookup"><span data-stu-id="160f3-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="160f3-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-123">Contacts.Read</span></span> | <span data-ttu-id="160f3-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-124">Contacts.Read</span></span> | <span data-ttu-id="160f3-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-125">Contacts.Read</span></span> |
|<span data-ttu-id="160f3-126">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="160f3-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="160f3-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-127">Not supported</span></span> | <span data-ttu-id="160f3-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="160f3-128">Files.ReadWrite</span></span> | <span data-ttu-id="160f3-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-129">Not supported</span></span> |
|<span data-ttu-id="160f3-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="160f3-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="160f3-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160f3-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="160f3-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-132">Not supported</span></span> | <span data-ttu-id="160f3-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160f3-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="160f3-134">evento</span><span class="sxs-lookup"><span data-stu-id="160f3-134">event</span></span>](../resources/event.md) | <span data-ttu-id="160f3-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-135">Calendars.Read</span></span> | <span data-ttu-id="160f3-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-136">Calendars.Read</span></span> | <span data-ttu-id="160f3-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-137">Calendars.Read</span></span> |
|[<span data-ttu-id="160f3-138">grupo</span><span class="sxs-lookup"><span data-stu-id="160f3-138">group</span></span>](../resources/group.md) | <span data-ttu-id="160f3-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-139">Group.Read.All</span></span> | <span data-ttu-id="160f3-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-140">Not supported</span></span> | <span data-ttu-id="160f3-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-141">Group.Read.All</span></span> |
|[<span data-ttu-id="160f3-142">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="160f3-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="160f3-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-143">Group.Read.All</span></span> | <span data-ttu-id="160f3-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-144">Not supported</span></span> | <span data-ttu-id="160f3-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-145">Not supported</span></span> |
|[<span data-ttu-id="160f3-146">message</span><span class="sxs-lookup"><span data-stu-id="160f3-146">message</span></span>](../resources/message.md) | <span data-ttu-id="160f3-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="160f3-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="160f3-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="160f3-149">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="160f3-150">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="160f3-150">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="160f3-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160f3-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="160f3-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="160f3-152">Not supported</span></span> | <span data-ttu-id="160f3-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="160f3-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="160f3-154">Usuário</span><span class="sxs-lookup"><span data-stu-id="160f3-154">user</span></span>](../resources/user.md) | <span data-ttu-id="160f3-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-155">User.Read.All</span></span> | <span data-ttu-id="160f3-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-156">User.Read.All</span></span> | <span data-ttu-id="160f3-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="160f3-157">User.Read.All</span></span> |

> <span data-ttu-id="160f3-158">**Observação:** Limitações adicionais se aplicam a assinaturas em itens do OneDrive e do Outlook.</span><span class="sxs-lookup"><span data-stu-id="160f3-158">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="160f3-159">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="160f3-159">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="160f3-160">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="160f3-160">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="160f3-161">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="160f3-161">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="160f3-162">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="160f3-162">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="160f3-163">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="160f3-163">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="160f3-164">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="160f3-164">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="160f3-165">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="160f3-165">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="160f3-166">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="160f3-166">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="160f3-167">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="160f3-167">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="160f3-168">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="160f3-168">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="160f3-169">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="160f3-169">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="160f3-170">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="160f3-170">Request headers</span></span>

| <span data-ttu-id="160f3-171">Nome</span><span class="sxs-lookup"><span data-stu-id="160f3-171">Name</span></span>       | <span data-ttu-id="160f3-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="160f3-172">Type</span></span> | <span data-ttu-id="160f3-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="160f3-173">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="160f3-174">Autorização</span><span class="sxs-lookup"><span data-stu-id="160f3-174">Authorization</span></span>  | <span data-ttu-id="160f3-175">string</span><span class="sxs-lookup"><span data-stu-id="160f3-175">string</span></span>  | <span data-ttu-id="160f3-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="160f3-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="160f3-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="160f3-178">Response</span></span>

<span data-ttu-id="160f3-179">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="160f3-179">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="160f3-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="160f3-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="160f3-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="160f3-181">Request</span></span>

<span data-ttu-id="160f3-182">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="160f3-182">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="160f3-183">Esse `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="160f3-183">The `clientState` field is optional.</span></span>

<span data-ttu-id="160f3-184">Esta solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="160f3-184">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="160f3-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="160f3-185">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="160f3-186">C#</span><span class="sxs-lookup"><span data-stu-id="160f3-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="160f3-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="160f3-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="160f3-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="160f3-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="160f3-189">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="160f3-189">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="160f3-190">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="160f3-190">Resource type</span></span> | <span data-ttu-id="160f3-191">Exemplos</span><span class="sxs-lookup"><span data-stu-id="160f3-191">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="160f3-192">Email</span><span class="sxs-lookup"><span data-stu-id="160f3-192">Mail</span></span>|<span data-ttu-id="160f3-193">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="160f3-193">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="160f3-194">me/messages</span><span class="sxs-lookup"><span data-stu-id="160f3-194">me/messages</span></span>|
|<span data-ttu-id="160f3-195">Contatos</span><span class="sxs-lookup"><span data-stu-id="160f3-195">Contacts</span></span>|<span data-ttu-id="160f3-196">me/contacts</span><span class="sxs-lookup"><span data-stu-id="160f3-196">me/contacts</span></span>|
|<span data-ttu-id="160f3-197">Calendários</span><span class="sxs-lookup"><span data-stu-id="160f3-197">Calendars</span></span>|<span data-ttu-id="160f3-198">me/events</span><span class="sxs-lookup"><span data-stu-id="160f3-198">me/events</span></span>|
|<span data-ttu-id="160f3-199">Usuários</span><span class="sxs-lookup"><span data-stu-id="160f3-199">Users</span></span>|<span data-ttu-id="160f3-200">usuários</span><span class="sxs-lookup"><span data-stu-id="160f3-200">users</span></span>|
|<span data-ttu-id="160f3-201">Grupos</span><span class="sxs-lookup"><span data-stu-id="160f3-201">Groups</span></span>|<span data-ttu-id="160f3-202">grupos</span><span class="sxs-lookup"><span data-stu-id="160f3-202">groups</span></span>|
|<span data-ttu-id="160f3-203">Conversas</span><span class="sxs-lookup"><span data-stu-id="160f3-203">Conversations</span></span>|<span data-ttu-id="160f3-204">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="160f3-204">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="160f3-205">Unidades</span><span class="sxs-lookup"><span data-stu-id="160f3-205">Drives</span></span>|<span data-ttu-id="160f3-206">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="160f3-206">me/drive/root</span></span>|
|<span data-ttu-id="160f3-207">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="160f3-207">Security alert</span></span>|<span data-ttu-id="160f3-208">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="160f3-208">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="160f3-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="160f3-209">Response</span></span>

<span data-ttu-id="160f3-210">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="160f3-210">The following example shows the response.</span></span> 

><span data-ttu-id="160f3-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="160f3-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="160f3-213">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="160f3-213">Notification endpoint validation</span></span>

<span data-ttu-id="160f3-214">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="160f3-214">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="160f3-215">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="160f3-215">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
