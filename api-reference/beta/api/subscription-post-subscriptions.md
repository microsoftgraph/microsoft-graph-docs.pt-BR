---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 487be3c7a50dcd5b09ece599f69b74248965eacf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870820"
---
# <a name="create-subscription"></a><span data-ttu-id="a98b0-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="a98b0-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a98b0-104">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a98b0-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="a98b0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a98b0-105">Permissions</span></span>

<span data-ttu-id="a98b0-106">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a98b0-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="a98b0-107">Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="a98b0-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="a98b0-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="a98b0-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a98b0-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a98b0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a98b0-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-110">Supported resource</span></span> | <span data-ttu-id="a98b0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a98b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a98b0-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a98b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a98b0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a98b0-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="a98b0-114">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="a98b0-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="a98b0-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-115">Not supported</span></span> | <span data-ttu-id="a98b0-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-116">Not supported</span></span> | <span data-ttu-id="a98b0-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a98b0-118">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="a98b0-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="a98b0-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-119">Not supported</span></span> | <span data-ttu-id="a98b0-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-120">Not supported</span></span> | <span data-ttu-id="a98b0-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="a98b0-122">contato</span><span class="sxs-lookup"><span data-stu-id="a98b0-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a98b0-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-123">Contacts.Read</span></span> | <span data-ttu-id="a98b0-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-124">Contacts.Read</span></span> | <span data-ttu-id="a98b0-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-125">Contacts.Read</span></span> |
|<span data-ttu-id="a98b0-126">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="a98b0-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a98b0-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-127">Not supported</span></span> | <span data-ttu-id="a98b0-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a98b0-128">Files.ReadWrite</span></span> | <span data-ttu-id="a98b0-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-129">Not supported</span></span> |
|<span data-ttu-id="a98b0-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a98b0-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a98b0-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="a98b0-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-132">Not supported</span></span> | <span data-ttu-id="a98b0-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a98b0-134">evento</span><span class="sxs-lookup"><span data-stu-id="a98b0-134">event</span></span>](../resources/event.md) | <span data-ttu-id="a98b0-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-135">Calendars.Read</span></span> | <span data-ttu-id="a98b0-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-136">Calendars.Read</span></span> | <span data-ttu-id="a98b0-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-137">Calendars.Read</span></span> |
|[<span data-ttu-id="a98b0-138">grupo</span><span class="sxs-lookup"><span data-stu-id="a98b0-138">group</span></span>](../resources/group.md) | <span data-ttu-id="a98b0-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-139">Group.Read.All</span></span> | <span data-ttu-id="a98b0-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-140">Not supported</span></span> | <span data-ttu-id="a98b0-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-141">Group.Read.All</span></span> |
|[<span data-ttu-id="a98b0-142">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="a98b0-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a98b0-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-143">Group.Read.All</span></span> | <span data-ttu-id="a98b0-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-144">Not supported</span></span> | <span data-ttu-id="a98b0-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-145">Not supported</span></span> |
|[<span data-ttu-id="a98b0-146">message</span><span class="sxs-lookup"><span data-stu-id="a98b0-146">message</span></span>](../resources/message.md) | <span data-ttu-id="a98b0-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a98b0-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a98b0-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a98b0-149">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="a98b0-150">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="a98b0-150">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="a98b0-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a98b0-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a98b0-152">Not supported</span></span> | <span data-ttu-id="a98b0-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a98b0-154">Usuário</span><span class="sxs-lookup"><span data-stu-id="a98b0-154">user</span></span>](../resources/user.md) | <span data-ttu-id="a98b0-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-155">User.Read.All</span></span> | <span data-ttu-id="a98b0-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-156">User.Read.All</span></span> | <span data-ttu-id="a98b0-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a98b0-157">User.Read.All</span></span> |

> <span data-ttu-id="a98b0-158">**Observação:** Em janeiro de 2020, as assinaturas do chat exigem [criptografia](/graph/webhooks-with-resource-data), e a criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="a98b0-158">**Note:** In January 2020, chatMessage subscriptions will require [encryption](/graph/webhooks-with-resource-data), and subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

> <span data-ttu-id="a98b0-159">**Observação:** Limitações adicionais se aplicam a assinaturas em itens do OneDrive e do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a98b0-159">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="a98b0-160">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="a98b0-160">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="a98b0-161">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="a98b0-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a98b0-162">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="a98b0-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a98b0-163">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="a98b0-163">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="a98b0-164">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="a98b0-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="a98b0-165">No Outlook, a permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a98b0-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a98b0-166">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="a98b0-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a98b0-167">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="a98b0-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a98b0-168">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="a98b0-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a98b0-169">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="a98b0-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="a98b0-170">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a98b0-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="a98b0-171">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a98b0-171">Request headers</span></span>

| <span data-ttu-id="a98b0-172">Nome</span><span class="sxs-lookup"><span data-stu-id="a98b0-172">Name</span></span>       | <span data-ttu-id="a98b0-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="a98b0-173">Type</span></span> | <span data-ttu-id="a98b0-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="a98b0-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a98b0-175">Autorização</span><span class="sxs-lookup"><span data-stu-id="a98b0-175">Authorization</span></span>  | <span data-ttu-id="a98b0-176">string</span><span class="sxs-lookup"><span data-stu-id="a98b0-176">string</span></span>  | <span data-ttu-id="a98b0-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a98b0-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a98b0-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="a98b0-179">Response</span></span>

<span data-ttu-id="a98b0-180">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a98b0-180">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a98b0-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a98b0-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="a98b0-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a98b0-182">Request</span></span>

<span data-ttu-id="a98b0-183">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="a98b0-183">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="a98b0-184">Esse `clientState` campo é opcional.</span><span class="sxs-lookup"><span data-stu-id="a98b0-184">The `clientState` field is optional.</span></span>

<span data-ttu-id="a98b0-185">Esta solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="a98b0-185">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a98b0-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="a98b0-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a98b0-187">C#</span><span class="sxs-lookup"><span data-stu-id="a98b0-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a98b0-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a98b0-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a98b0-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98b0-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a98b0-190">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="a98b0-190">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="a98b0-191">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="a98b0-191">Resource type</span></span> | <span data-ttu-id="a98b0-192">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a98b0-192">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="a98b0-193">Email</span><span class="sxs-lookup"><span data-stu-id="a98b0-193">Mail</span></span>|<span data-ttu-id="a98b0-194">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="a98b0-194">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="a98b0-195">me/messages</span><span class="sxs-lookup"><span data-stu-id="a98b0-195">me/messages</span></span>|
|<span data-ttu-id="a98b0-196">Contatos</span><span class="sxs-lookup"><span data-stu-id="a98b0-196">Contacts</span></span>|<span data-ttu-id="a98b0-197">me/contacts</span><span class="sxs-lookup"><span data-stu-id="a98b0-197">me/contacts</span></span>|
|<span data-ttu-id="a98b0-198">Calendários</span><span class="sxs-lookup"><span data-stu-id="a98b0-198">Calendars</span></span>|<span data-ttu-id="a98b0-199">me/events</span><span class="sxs-lookup"><span data-stu-id="a98b0-199">me/events</span></span>|
|<span data-ttu-id="a98b0-200">Usuários</span><span class="sxs-lookup"><span data-stu-id="a98b0-200">Users</span></span>|<span data-ttu-id="a98b0-201">usuários</span><span class="sxs-lookup"><span data-stu-id="a98b0-201">users</span></span>|
|<span data-ttu-id="a98b0-202">Grupos</span><span class="sxs-lookup"><span data-stu-id="a98b0-202">Groups</span></span>|<span data-ttu-id="a98b0-203">grupos</span><span class="sxs-lookup"><span data-stu-id="a98b0-203">groups</span></span>|
|<span data-ttu-id="a98b0-204">Conversas</span><span class="sxs-lookup"><span data-stu-id="a98b0-204">Conversations</span></span>|<span data-ttu-id="a98b0-205">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="a98b0-205">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="a98b0-206">Unidades</span><span class="sxs-lookup"><span data-stu-id="a98b0-206">Drives</span></span>|<span data-ttu-id="a98b0-207">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="a98b0-207">me/drive/root</span></span>|
|<span data-ttu-id="a98b0-208">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="a98b0-208">Security alert</span></span>|<span data-ttu-id="a98b0-209">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="a98b0-209">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="a98b0-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="a98b0-210">Response</span></span>

<span data-ttu-id="a98b0-211">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a98b0-211">The following example shows the response.</span></span> 

><span data-ttu-id="a98b0-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a98b0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="a98b0-214">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="a98b0-214">Notification endpoint validation</span></span>

<span data-ttu-id="a98b0-215">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="a98b0-215">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="a98b0-216">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="a98b0-216">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
