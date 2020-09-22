---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 08166c2570c6c73fbb412a4713b5669b36e57736
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193313"
---
# <a name="delete-subscription"></a><span data-ttu-id="f1320-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="f1320-103">Delete subscription</span></span>

<span data-ttu-id="f1320-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1320-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1320-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="f1320-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1320-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1320-106">Permissions</span></span>

<span data-ttu-id="f1320-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="f1320-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f1320-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1320-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1320-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-109">Supported resource</span></span> | <span data-ttu-id="f1320-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1320-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1320-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1320-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1320-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1320-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="f1320-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="f1320-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="f1320-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-114">Not supported</span></span> | <span data-ttu-id="f1320-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-115">Not supported</span></span> | <span data-ttu-id="f1320-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="f1320-117">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="f1320-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="f1320-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="f1320-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-119">Not supported</span></span> | <span data-ttu-id="f1320-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="f1320-121">[chat](../resources/chatmessage.md) (/Teams/getAllMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="f1320-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="f1320-122">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-122">Not supported</span></span> | <span data-ttu-id="f1320-123">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-123">Not supported</span></span> | <span data-ttu-id="f1320-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="f1320-125">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="f1320-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="f1320-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1320-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="f1320-127">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-127">Not supported</span></span> | <span data-ttu-id="f1320-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="f1320-129">[chat](../resources/chatmessage.md) (/chats/getAllMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="f1320-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="f1320-130">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-130">Not supported</span></span> | <span data-ttu-id="f1320-131">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-131">Not supported</span></span> | <span data-ttu-id="f1320-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="f1320-133">contato</span><span class="sxs-lookup"><span data-stu-id="f1320-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f1320-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-134">Contacts.Read</span></span> | <span data-ttu-id="f1320-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-135">Contacts.Read</span></span> | <span data-ttu-id="f1320-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-136">Contacts.Read</span></span> |
|<span data-ttu-id="f1320-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="f1320-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="f1320-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-138">Not supported</span></span> | <span data-ttu-id="f1320-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1320-139">Files.ReadWrite</span></span> | <span data-ttu-id="f1320-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-140">Not supported</span></span> |
|<span data-ttu-id="f1320-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="f1320-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="f1320-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="f1320-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-143">Not supported</span></span> | <span data-ttu-id="f1320-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="f1320-145">evento</span><span class="sxs-lookup"><span data-stu-id="f1320-145">event</span></span>](../resources/event.md) | <span data-ttu-id="f1320-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-146">Calendars.Read</span></span> | <span data-ttu-id="f1320-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-147">Calendars.Read</span></span> | <span data-ttu-id="f1320-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-148">Calendars.Read</span></span> |
|[<span data-ttu-id="f1320-149">grupo</span><span class="sxs-lookup"><span data-stu-id="f1320-149">group</span></span>](../resources/group.md) | <span data-ttu-id="f1320-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-150">Group.Read.All</span></span> | <span data-ttu-id="f1320-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-151">Not supported</span></span> | <span data-ttu-id="f1320-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-152">Group.Read.All</span></span> |
|[<span data-ttu-id="f1320-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="f1320-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="f1320-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-154">Group.Read.All</span></span> | <span data-ttu-id="f1320-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-155">Not supported</span></span> | <span data-ttu-id="f1320-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-156">Not supported</span></span> |
|[<span data-ttu-id="f1320-157">list</span><span class="sxs-lookup"><span data-stu-id="f1320-157">list</span></span>](../resources/list.md) | <span data-ttu-id="f1320-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="f1320-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-159">Not supported</span></span> | <span data-ttu-id="f1320-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="f1320-161">message</span><span class="sxs-lookup"><span data-stu-id="f1320-161">message</span></span>](../resources/message.md) | <span data-ttu-id="f1320-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="f1320-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="f1320-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f1320-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="f1320-165">presença</span><span class="sxs-lookup"><span data-stu-id="f1320-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="f1320-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-166">Presence.Read.All</span></span> | <span data-ttu-id="f1320-167">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-167">Not supported</span></span> | <span data-ttu-id="f1320-168">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f1320-168">Not supported</span></span> |
|[<span data-ttu-id="f1320-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="f1320-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="f1320-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="f1320-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f1320-171">Not supported</span></span> | <span data-ttu-id="f1320-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1320-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="f1320-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="f1320-173">user</span></span>](../resources/user.md) | <span data-ttu-id="f1320-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-174">User.Read.All</span></span> | <span data-ttu-id="f1320-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-175">User.Read.All</span></span> | <span data-ttu-id="f1320-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1320-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="f1320-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f1320-177">chatMessage</span></span>

<span data-ttu-id="f1320-178">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f1320-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="f1320-179">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f1320-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f1320-180">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="f1320-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="f1320-181">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="f1320-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="f1320-182">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="f1320-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="f1320-183">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para usuários que têm as  
 [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="f1320-183">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="f1320-184">driveItem</span><span class="sxs-lookup"><span data-stu-id="f1320-184">driveItem</span></span>

<span data-ttu-id="f1320-185">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f1320-185">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="f1320-186">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="f1320-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="f1320-187">Em um OneDrive pessoal, você pode inscrever-se na pasta raiz ou em qualquer subpasta nessa unidade.</span><span class="sxs-lookup"><span data-stu-id="f1320-187">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="f1320-188">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="f1320-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="f1320-189">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="f1320-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="f1320-190">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="f1320-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="f1320-191">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="f1320-191">contact, event, and message</span></span>

<span data-ttu-id="f1320-192">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f1320-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="f1320-193">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="f1320-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="f1320-194">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f1320-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="f1320-195">Por exemplo, você não pode usar os calendários de permissão delegada. Leia para inscrever-se em eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="f1320-195">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="f1320-196">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="f1320-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="f1320-197">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="f1320-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="f1320-198">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="f1320-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="f1320-199">presença</span><span class="sxs-lookup"><span data-stu-id="f1320-199">presence</span></span>

<span data-ttu-id="f1320-200">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f1320-200">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f1320-201">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="f1320-201">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1320-202">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1320-202">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1320-203">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1320-203">Request headers</span></span>

| <span data-ttu-id="f1320-204">Nome</span><span class="sxs-lookup"><span data-stu-id="f1320-204">Name</span></span>       | <span data-ttu-id="f1320-205">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1320-205">Type</span></span> | <span data-ttu-id="f1320-206">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1320-206">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1320-207">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1320-207">Authorization</span></span>  | <span data-ttu-id="f1320-208">string</span><span class="sxs-lookup"><span data-stu-id="f1320-208">string</span></span>  | <span data-ttu-id="f1320-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1320-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1320-211">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1320-211">Request body</span></span>

<span data-ttu-id="f1320-212">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1320-212">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1320-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1320-213">Response</span></span>

<span data-ttu-id="f1320-214">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1320-214">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f1320-215">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="f1320-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="f1320-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1320-216">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f1320-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1320-217">Request</span></span>

<span data-ttu-id="f1320-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1320-218">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1320-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1320-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="f1320-220">C#</span><span class="sxs-lookup"><span data-stu-id="f1320-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1320-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1320-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1320-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1320-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f1320-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1320-223">Response</span></span>

<span data-ttu-id="f1320-224">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1320-224">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


