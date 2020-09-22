---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: a8308d702f786f51375953268b9e9403864645aa
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193516"
---
# <a name="get-subscription"></a><span data-ttu-id="88c10-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="88c10-103">Get subscription</span></span>

<span data-ttu-id="88c10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88c10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88c10-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="88c10-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="88c10-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88c10-106">Permissions</span></span>

<span data-ttu-id="88c10-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="88c10-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="88c10-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88c10-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88c10-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-109">Supported resource</span></span> | <span data-ttu-id="88c10-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88c10-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88c10-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88c10-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88c10-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88c10-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="88c10-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="88c10-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="88c10-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-114">Not supported</span></span> | <span data-ttu-id="88c10-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-115">Not supported</span></span> | <span data-ttu-id="88c10-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="88c10-117">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="88c10-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="88c10-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="88c10-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-119">Not supported</span></span> | <span data-ttu-id="88c10-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="88c10-121">[chat](../resources/chatmessage.md) (/Teams/getAllMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="88c10-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="88c10-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-122">Not supported</span></span> | <span data-ttu-id="88c10-123">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-123">Not supported</span></span> | <span data-ttu-id="88c10-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="88c10-125">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="88c10-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="88c10-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88c10-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="88c10-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-127">Not supported</span></span> | <span data-ttu-id="88c10-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="88c10-129">[chat](../resources/chatmessage.md) (/chats/getAllMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="88c10-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="88c10-130">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-130">Not supported</span></span> | <span data-ttu-id="88c10-131">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-131">Not supported</span></span> | <span data-ttu-id="88c10-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="88c10-133">contato</span><span class="sxs-lookup"><span data-stu-id="88c10-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="88c10-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-134">Contacts.Read</span></span> | <span data-ttu-id="88c10-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-135">Contacts.Read</span></span> | <span data-ttu-id="88c10-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-136">Contacts.Read</span></span> |
|<span data-ttu-id="88c10-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="88c10-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="88c10-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-138">Not supported</span></span> | <span data-ttu-id="88c10-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88c10-139">Files.ReadWrite</span></span> | <span data-ttu-id="88c10-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-140">Not supported</span></span> |
|<span data-ttu-id="88c10-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="88c10-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="88c10-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="88c10-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-143">Not supported</span></span> | <span data-ttu-id="88c10-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="88c10-145">evento</span><span class="sxs-lookup"><span data-stu-id="88c10-145">event</span></span>](../resources/event.md) | <span data-ttu-id="88c10-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-146">Calendars.Read</span></span> | <span data-ttu-id="88c10-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-147">Calendars.Read</span></span> | <span data-ttu-id="88c10-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-148">Calendars.Read</span></span> |
|[<span data-ttu-id="88c10-149">grupo</span><span class="sxs-lookup"><span data-stu-id="88c10-149">group</span></span>](../resources/group.md) | <span data-ttu-id="88c10-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-150">Group.Read.All</span></span> | <span data-ttu-id="88c10-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-151">Not supported</span></span> | <span data-ttu-id="88c10-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-152">Group.Read.All</span></span> |
|[<span data-ttu-id="88c10-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="88c10-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="88c10-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-154">Group.Read.All</span></span> | <span data-ttu-id="88c10-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-155">Not supported</span></span> | <span data-ttu-id="88c10-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-156">Not supported</span></span> |
|[<span data-ttu-id="88c10-157">list</span><span class="sxs-lookup"><span data-stu-id="88c10-157">list</span></span>](../resources/list.md) | <span data-ttu-id="88c10-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="88c10-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-159">Not supported</span></span> | <span data-ttu-id="88c10-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="88c10-161">message</span><span class="sxs-lookup"><span data-stu-id="88c10-161">message</span></span>](../resources/message.md) | <span data-ttu-id="88c10-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="88c10-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="88c10-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="88c10-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="88c10-165">presença</span><span class="sxs-lookup"><span data-stu-id="88c10-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="88c10-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-166">Presence.Read.All</span></span> | <span data-ttu-id="88c10-167">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-167">Not supported</span></span> | <span data-ttu-id="88c10-168">Incompatível</span><span class="sxs-lookup"><span data-stu-id="88c10-168">Not supported</span></span> |
|[<span data-ttu-id="88c10-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="88c10-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="88c10-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="88c10-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88c10-171">Not supported</span></span> | <span data-ttu-id="88c10-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c10-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="88c10-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="88c10-173">user</span></span>](../resources/user.md) | <span data-ttu-id="88c10-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-174">User.Read.All</span></span> | <span data-ttu-id="88c10-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-175">User.Read.All</span></span> | <span data-ttu-id="88c10-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c10-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="88c10-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="88c10-177">chatMessage</span></span>

<span data-ttu-id="88c10-178">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="88c10-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="88c10-179">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="88c10-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="88c10-180">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="88c10-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="88c10-181">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="88c10-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="88c10-182">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="88c10-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="88c10-183">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para usuários que têm as  
 [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="88c10-183">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="88c10-184">driveItem</span><span class="sxs-lookup"><span data-stu-id="88c10-184">driveItem</span></span>

<span data-ttu-id="88c10-185">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="88c10-185">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="88c10-186">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="88c10-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="88c10-187">Em um OneDrive pessoal, você pode inscrever-se na pasta raiz ou em qualquer subpasta nessa unidade.</span><span class="sxs-lookup"><span data-stu-id="88c10-187">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="88c10-188">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="88c10-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="88c10-189">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="88c10-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="88c10-190">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="88c10-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="88c10-191">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="88c10-191">contact, event, and message</span></span>

<span data-ttu-id="88c10-192">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="88c10-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="88c10-193">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="88c10-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="88c10-194">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="88c10-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="88c10-195">Por exemplo, você não pode usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="88c10-195">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="88c10-196">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="88c10-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="88c10-197">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="88c10-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="88c10-198">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="88c10-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="88c10-199">presença</span><span class="sxs-lookup"><span data-stu-id="88c10-199">presence</span></span>

<span data-ttu-id="88c10-200">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="88c10-200">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="88c10-201">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="88c10-201">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="88c10-202">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88c10-202">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88c10-203">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88c10-203">Optional query parameters</span></span>

<span data-ttu-id="88c10-204">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88c10-204">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88c10-205">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88c10-205">Request headers</span></span>

| <span data-ttu-id="88c10-206">Nome</span><span class="sxs-lookup"><span data-stu-id="88c10-206">Name</span></span>       | <span data-ttu-id="88c10-207">Tipo</span><span class="sxs-lookup"><span data-stu-id="88c10-207">Type</span></span> | <span data-ttu-id="88c10-208">Descrição</span><span class="sxs-lookup"><span data-stu-id="88c10-208">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="88c10-209">Autorização</span><span class="sxs-lookup"><span data-stu-id="88c10-209">Authorization</span></span>  | <span data-ttu-id="88c10-210">string</span><span class="sxs-lookup"><span data-stu-id="88c10-210">string</span></span>  | <span data-ttu-id="88c10-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88c10-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88c10-213">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88c10-213">Request body</span></span>

<span data-ttu-id="88c10-214">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88c10-214">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88c10-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="88c10-215">Response</span></span>

<span data-ttu-id="88c10-216">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88c10-216">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88c10-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88c10-217">Example</span></span>

##### <a name="request"></a><span data-ttu-id="88c10-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88c10-218">Request</span></span>

<span data-ttu-id="88c10-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88c10-219">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88c10-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="88c10-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="88c10-221">C#</span><span class="sxs-lookup"><span data-stu-id="88c10-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88c10-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88c10-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88c10-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88c10-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88c10-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="88c10-224">Response</span></span>

<span data-ttu-id="88c10-225">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88c10-225">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


