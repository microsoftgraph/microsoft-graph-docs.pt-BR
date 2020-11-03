---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 857af6aff513582d4d0bfcf7bcad5b364b8518e2
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848721"
---
# <a name="get-subscription"></a><span data-ttu-id="bdc04-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="bdc04-103">Get subscription</span></span>

<span data-ttu-id="bdc04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdc04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdc04-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="bdc04-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdc04-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdc04-106">Permissions</span></span>

<span data-ttu-id="bdc04-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="bdc04-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="bdc04-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdc04-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdc04-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-109">Supported resource</span></span> | <span data-ttu-id="bdc04-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdc04-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdc04-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdc04-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdc04-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdc04-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="bdc04-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="bdc04-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="bdc04-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="bdc04-114">Not supported</span></span> | <span data-ttu-id="bdc04-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="bdc04-115">Not supported</span></span> | <span data-ttu-id="bdc04-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="bdc04-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="bdc04-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="bdc04-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="bdc04-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-119">Not supported</span></span> | <span data-ttu-id="bdc04-120">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="bdc04-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="bdc04-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="bdc04-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="bdc04-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-122">Not supported</span></span> | <span data-ttu-id="bdc04-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-123">Not supported</span></span> | <span data-ttu-id="bdc04-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="bdc04-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="bdc04-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="bdc04-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdc04-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="bdc04-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-127">Not supported</span></span> | <span data-ttu-id="bdc04-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="bdc04-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="bdc04-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="bdc04-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-130">Not supported</span></span> | <span data-ttu-id="bdc04-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-131">Not supported</span></span> | <span data-ttu-id="bdc04-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="bdc04-133">contato</span><span class="sxs-lookup"><span data-stu-id="bdc04-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="bdc04-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-134">Contacts.Read</span></span> | <span data-ttu-id="bdc04-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-135">Contacts.Read</span></span> | <span data-ttu-id="bdc04-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-136">Contacts.Read</span></span> |
|<span data-ttu-id="bdc04-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="bdc04-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="bdc04-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-138">Not supported</span></span> | <span data-ttu-id="bdc04-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdc04-139">Files.ReadWrite</span></span> | <span data-ttu-id="bdc04-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-140">Not supported</span></span> |
|<span data-ttu-id="bdc04-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="bdc04-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="bdc04-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="bdc04-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-143">Not supported</span></span> | <span data-ttu-id="bdc04-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="bdc04-145">evento</span><span class="sxs-lookup"><span data-stu-id="bdc04-145">event</span></span>](../resources/event.md) | <span data-ttu-id="bdc04-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-146">Calendars.Read</span></span> | <span data-ttu-id="bdc04-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-147">Calendars.Read</span></span> | <span data-ttu-id="bdc04-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-148">Calendars.Read</span></span> |
|[<span data-ttu-id="bdc04-149">grupo</span><span class="sxs-lookup"><span data-stu-id="bdc04-149">group</span></span>](../resources/group.md) | <span data-ttu-id="bdc04-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-150">Group.Read.All</span></span> | <span data-ttu-id="bdc04-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-151">Not supported</span></span> | <span data-ttu-id="bdc04-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-152">Group.Read.All</span></span> |
|[<span data-ttu-id="bdc04-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="bdc04-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="bdc04-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-154">Group.Read.All</span></span> | <span data-ttu-id="bdc04-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-155">Not supported</span></span> | <span data-ttu-id="bdc04-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-156">Not supported</span></span> |
|[<span data-ttu-id="bdc04-157">list</span><span class="sxs-lookup"><span data-stu-id="bdc04-157">list</span></span>](../resources/list.md) | <span data-ttu-id="bdc04-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="bdc04-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-159">Not supported</span></span> | <span data-ttu-id="bdc04-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="bdc04-161">message</span><span class="sxs-lookup"><span data-stu-id="bdc04-161">message</span></span>](../resources/message.md) | <span data-ttu-id="bdc04-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bdc04-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bdc04-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bdc04-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="bdc04-165">presence</span><span class="sxs-lookup"><span data-stu-id="bdc04-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="bdc04-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-166">Presence.Read.All</span></span> | <span data-ttu-id="bdc04-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-167">Not supported</span></span> | <span data-ttu-id="bdc04-168">Incompatível</span><span class="sxs-lookup"><span data-stu-id="bdc04-168">Not supported</span></span> |
|[<span data-ttu-id="bdc04-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="bdc04-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="bdc04-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="bdc04-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdc04-171">Not supported</span></span> | <span data-ttu-id="bdc04-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="bdc04-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="bdc04-173">user</span></span>](../resources/user.md) | <span data-ttu-id="bdc04-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-174">User.Read.All</span></span> | <span data-ttu-id="bdc04-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-175">User.Read.All</span></span> | <span data-ttu-id="bdc04-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdc04-176">User.Read.All</span></span> |

> <span data-ttu-id="bdc04-177">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bdc04-177">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="bdc04-178">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bdc04-178">chatMessage</span></span>

<span data-ttu-id="bdc04-179">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="bdc04-179">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="bdc04-180">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="bdc04-180">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="bdc04-181">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="bdc04-181">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="bdc04-182">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="bdc04-182">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="bdc04-183">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="bdc04-183">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="bdc04-184">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="bdc04-184">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="bdc04-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="bdc04-185">driveItem</span></span>

<span data-ttu-id="bdc04-186">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bdc04-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="bdc04-187">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="bdc04-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="bdc04-188">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="bdc04-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="bdc04-189">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="bdc04-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="bdc04-190">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="bdc04-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="bdc04-191">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="bdc04-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="bdc04-192">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="bdc04-192">contact, event, and message</span></span>

<span data-ttu-id="bdc04-193">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="bdc04-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="bdc04-194">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="bdc04-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="bdc04-195">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="bdc04-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="bdc04-196">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="bdc04-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="bdc04-197">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="bdc04-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="bdc04-198">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="bdc04-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="bdc04-199">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="bdc04-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="bdc04-200">presença</span><span class="sxs-lookup"><span data-stu-id="bdc04-200">presence</span></span>

<span data-ttu-id="bdc04-201">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="bdc04-201">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="bdc04-202">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="bdc04-202">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="bdc04-203">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdc04-203">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bdc04-204">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bdc04-204">Optional query parameters</span></span>

<span data-ttu-id="bdc04-205">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bdc04-205">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdc04-206">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc04-206">Request headers</span></span>

| <span data-ttu-id="bdc04-207">Nome</span><span class="sxs-lookup"><span data-stu-id="bdc04-207">Name</span></span>       | <span data-ttu-id="bdc04-208">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdc04-208">Type</span></span> | <span data-ttu-id="bdc04-209">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdc04-209">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="bdc04-210">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdc04-210">Authorization</span></span>  | <span data-ttu-id="bdc04-211">string</span><span class="sxs-lookup"><span data-stu-id="bdc04-211">string</span></span>  | <span data-ttu-id="bdc04-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdc04-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdc04-214">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc04-214">Request body</span></span>

<span data-ttu-id="bdc04-215">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bdc04-215">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdc04-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdc04-216">Response</span></span>

<span data-ttu-id="bdc04-217">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdc04-217">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdc04-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdc04-218">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bdc04-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc04-219">Request</span></span>

<span data-ttu-id="bdc04-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdc04-220">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdc04-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdc04-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="bdc04-222">C#</span><span class="sxs-lookup"><span data-stu-id="bdc04-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdc04-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdc04-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdc04-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdc04-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bdc04-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdc04-225">Response</span></span>

<span data-ttu-id="bdc04-226">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdc04-226">Here is an example of the response.</span></span>
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
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
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


