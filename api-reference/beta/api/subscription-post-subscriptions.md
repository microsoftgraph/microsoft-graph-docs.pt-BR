---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e5276d8cf4e0a096e1ce98c9247d0c46e9f515c9
ms.sourcegitcommit: 568909e47fb075264584e440fd0cad978abfab11
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/27/2020
ms.locfileid: "42287986"
---
# <a name="create-subscription"></a><span data-ttu-id="c4718-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="c4718-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4718-104">Assinar um aplicativo de escuta para receber notificações quando o tipo de alterações solicitadas ocorrer em recursos específicos no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c4718-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4718-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4718-105">Permissions</span></span>

<span data-ttu-id="c4718-106">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="c4718-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="c4718-107">Por exemplo, para obter notificações sobre mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="c4718-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="c4718-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="c4718-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c4718-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4718-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4718-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-110">Supported resource</span></span> | <span data-ttu-id="c4718-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4718-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4718-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4718-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4718-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4718-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="c4718-114">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="c4718-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="c4718-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-115">Not supported</span></span> | <span data-ttu-id="c4718-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-116">Not supported</span></span> | <span data-ttu-id="c4718-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c4718-118">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="c4718-118">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="c4718-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-119">Not supported</span></span> | <span data-ttu-id="c4718-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-120">Not supported</span></span> | <span data-ttu-id="c4718-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-121">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c4718-122">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="c4718-122">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="c4718-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-123">Not supported</span></span> | <span data-ttu-id="c4718-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-124">Not supported</span></span> | <span data-ttu-id="c4718-125">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-125">Chat.Read.All</span></span>  |
|<span data-ttu-id="c4718-126">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="c4718-126">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="c4718-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-127">Not supported</span></span> | <span data-ttu-id="c4718-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-128">Not supported</span></span> | <span data-ttu-id="c4718-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-129">Chat.Read.All</span></span>  |
|[<span data-ttu-id="c4718-130">contato</span><span class="sxs-lookup"><span data-stu-id="c4718-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c4718-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-131">Contacts.Read</span></span> | <span data-ttu-id="c4718-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-132">Contacts.Read</span></span> | <span data-ttu-id="c4718-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-133">Contacts.Read</span></span> |
|<span data-ttu-id="c4718-134">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="c4718-134">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c4718-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-135">Not supported</span></span> | <span data-ttu-id="c4718-136">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4718-136">Files.ReadWrite</span></span> | <span data-ttu-id="c4718-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-137">Not supported</span></span> |
|<span data-ttu-id="c4718-138">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="c4718-138">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c4718-139">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4718-139">Files.ReadWrite.All</span></span> | <span data-ttu-id="c4718-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-140">Not supported</span></span> | <span data-ttu-id="c4718-141">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4718-141">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c4718-142">evento</span><span class="sxs-lookup"><span data-stu-id="c4718-142">event</span></span>](../resources/event.md) | <span data-ttu-id="c4718-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-143">Calendars.Read</span></span> | <span data-ttu-id="c4718-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-144">Calendars.Read</span></span> | <span data-ttu-id="c4718-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-145">Calendars.Read</span></span> |
|[<span data-ttu-id="c4718-146">grupo</span><span class="sxs-lookup"><span data-stu-id="c4718-146">group</span></span>](../resources/group.md) | <span data-ttu-id="c4718-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-147">Group.Read.All</span></span> | <span data-ttu-id="c4718-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-148">Not supported</span></span> | <span data-ttu-id="c4718-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-149">Group.Read.All</span></span> |
|[<span data-ttu-id="c4718-150">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="c4718-150">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c4718-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-151">Group.Read.All</span></span> | <span data-ttu-id="c4718-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-152">Not supported</span></span> | <span data-ttu-id="c4718-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-153">Not supported</span></span> |
|[<span data-ttu-id="c4718-154">message</span><span class="sxs-lookup"><span data-stu-id="c4718-154">message</span></span>](../resources/message.md) | <span data-ttu-id="c4718-155">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-155">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c4718-156">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-156">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c4718-157">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c4718-157">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="c4718-158">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="c4718-158">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="c4718-159">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4718-159">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c4718-160">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c4718-160">Not supported</span></span> | <span data-ttu-id="c4718-161">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4718-161">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c4718-162">Usuário</span><span class="sxs-lookup"><span data-stu-id="c4718-162">user</span></span>](../resources/user.md) | <span data-ttu-id="c4718-163">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-163">User.Read.All</span></span> | <span data-ttu-id="c4718-164">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-164">User.Read.All</span></span> | <span data-ttu-id="c4718-165">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4718-165">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="c4718-166">Chat (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="c4718-166">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="c4718-167">as assinaturas do **chat** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c4718-167">**chatMessage** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="c4718-168">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="c4718-168">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="c4718-169">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="c4718-169">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="c4718-170">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c4718-170">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="c4718-171">**Observação:** `/teams/allMessages` e `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="c4718-171">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="c4718-172">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="c4718-172">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="c4718-173">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4718-173">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="c4718-174">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="c4718-174">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="c4718-175">driveItem (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="c4718-175">driveItem (OneDrive)</span></span>

<span data-ttu-id="c4718-176">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c4718-176">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="c4718-177">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="c4718-177">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="c4718-178">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="c4718-178">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c4718-179">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="c4718-179">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c4718-180">As notificações são enviadas pelos tipos de alterações solicitadas na pasta inscrita, ou qualquer arquivo, pasta ou outras instâncias **driveItem** na sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="c4718-180">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="c4718-181">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="c4718-181">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="c4718-182">contato, evento e mensagem (Outlook)</span><span class="sxs-lookup"><span data-stu-id="c4718-182">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="c4718-183">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4718-183">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="c4718-184">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="c4718-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="c4718-185">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c4718-185">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c4718-186">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="c4718-186">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="c4718-187">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="c4718-187">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c4718-188">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="c4718-188">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c4718-189">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="c4718-189">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="c4718-190">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4718-190">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="c4718-191">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4718-191">Request headers</span></span>

| <span data-ttu-id="c4718-192">Nome</span><span class="sxs-lookup"><span data-stu-id="c4718-192">Name</span></span>       | <span data-ttu-id="c4718-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4718-193">Type</span></span> | <span data-ttu-id="c4718-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4718-194">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c4718-195">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4718-195">Authorization</span></span>  | <span data-ttu-id="c4718-196">string</span><span class="sxs-lookup"><span data-stu-id="c4718-196">string</span></span>  | <span data-ttu-id="c4718-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4718-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4718-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4718-199">Response</span></span>

<span data-ttu-id="c4718-200">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4718-200">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4718-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4718-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4718-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4718-202">Request</span></span>

<span data-ttu-id="c4718-203">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="c4718-203">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="c4718-204">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="c4718-204">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="c4718-205">Esta solicitação cria uma assinatura para notificações sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="c4718-205">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4718-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4718-206">HTTP</span></span>](#tab/http)
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
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="c4718-207">C#</span><span class="sxs-lookup"><span data-stu-id="c4718-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4718-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4718-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4718-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4718-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c4718-210">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="c4718-210">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="c4718-211">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="c4718-211">Resource type</span></span> | <span data-ttu-id="c4718-212">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4718-212">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="c4718-213">Email</span><span class="sxs-lookup"><span data-stu-id="c4718-213">Mail</span></span>|<span data-ttu-id="c4718-214">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="c4718-214">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="c4718-215">me/messages</span><span class="sxs-lookup"><span data-stu-id="c4718-215">me/messages</span></span>|
|<span data-ttu-id="c4718-216">Contatos</span><span class="sxs-lookup"><span data-stu-id="c4718-216">Contacts</span></span>|<span data-ttu-id="c4718-217">me/contacts</span><span class="sxs-lookup"><span data-stu-id="c4718-217">me/contacts</span></span>|
|<span data-ttu-id="c4718-218">Calendários</span><span class="sxs-lookup"><span data-stu-id="c4718-218">Calendars</span></span>|<span data-ttu-id="c4718-219">me/events</span><span class="sxs-lookup"><span data-stu-id="c4718-219">me/events</span></span>|
|<span data-ttu-id="c4718-220">Usuários</span><span class="sxs-lookup"><span data-stu-id="c4718-220">Users</span></span>|<span data-ttu-id="c4718-221">usuários</span><span class="sxs-lookup"><span data-stu-id="c4718-221">users</span></span>|
|<span data-ttu-id="c4718-222">Grupos</span><span class="sxs-lookup"><span data-stu-id="c4718-222">Groups</span></span>|<span data-ttu-id="c4718-223">grupos</span><span class="sxs-lookup"><span data-stu-id="c4718-223">groups</span></span>|
|<span data-ttu-id="c4718-224">Conversas</span><span class="sxs-lookup"><span data-stu-id="c4718-224">Conversations</span></span>|<span data-ttu-id="c4718-225">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="c4718-225">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="c4718-226">Unidades</span><span class="sxs-lookup"><span data-stu-id="c4718-226">Drives</span></span>|<span data-ttu-id="c4718-227">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="c4718-227">me/drive/root</span></span>|
|<span data-ttu-id="c4718-228">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="c4718-228">Security alert</span></span>|<span data-ttu-id="c4718-229">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="c4718-229">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="c4718-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4718-230">Response</span></span>

<span data-ttu-id="c4718-231">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4718-231">The following example shows the response.</span></span> 

><span data-ttu-id="c4718-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4718-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="c4718-234">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="c4718-234">Notification endpoint validation</span></span>

<span data-ttu-id="c4718-235">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="c4718-235">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="c4718-236">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="c4718-236">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
