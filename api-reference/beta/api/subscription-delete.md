---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fbf44321322d51bc237715f7b4555a68655ee10
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848686"
---
# <a name="delete-subscription"></a><span data-ttu-id="688a9-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="688a9-103">Delete subscription</span></span>

<span data-ttu-id="688a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="688a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="688a9-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="688a9-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="688a9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="688a9-106">Permissions</span></span>

<span data-ttu-id="688a9-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="688a9-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="688a9-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688a9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="688a9-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-109">Supported resource</span></span> | <span data-ttu-id="688a9-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="688a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="688a9-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="688a9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="688a9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="688a9-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="688a9-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="688a9-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="688a9-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="688a9-114">Not supported</span></span> | <span data-ttu-id="688a9-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="688a9-115">Not supported</span></span> | <span data-ttu-id="688a9-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="688a9-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="688a9-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="688a9-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="688a9-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="688a9-119">Not supported</span></span> | <span data-ttu-id="688a9-120">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="688a9-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="688a9-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="688a9-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="688a9-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-122">Not supported</span></span> | <span data-ttu-id="688a9-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-123">Not supported</span></span> | <span data-ttu-id="688a9-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="688a9-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="688a9-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="688a9-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="688a9-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="688a9-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-127">Not supported</span></span> | <span data-ttu-id="688a9-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="688a9-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="688a9-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="688a9-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-130">Not supported</span></span> | <span data-ttu-id="688a9-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-131">Not supported</span></span> | <span data-ttu-id="688a9-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="688a9-133">contato</span><span class="sxs-lookup"><span data-stu-id="688a9-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="688a9-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-134">Contacts.Read</span></span> | <span data-ttu-id="688a9-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-135">Contacts.Read</span></span> | <span data-ttu-id="688a9-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-136">Contacts.Read</span></span> |
|<span data-ttu-id="688a9-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="688a9-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="688a9-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-138">Not supported</span></span> | <span data-ttu-id="688a9-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="688a9-139">Files.ReadWrite</span></span> | <span data-ttu-id="688a9-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-140">Not supported</span></span> |
|<span data-ttu-id="688a9-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="688a9-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="688a9-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="688a9-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-143">Not supported</span></span> | <span data-ttu-id="688a9-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="688a9-145">evento</span><span class="sxs-lookup"><span data-stu-id="688a9-145">event</span></span>](../resources/event.md) | <span data-ttu-id="688a9-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-146">Calendars.Read</span></span> | <span data-ttu-id="688a9-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-147">Calendars.Read</span></span> | <span data-ttu-id="688a9-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-148">Calendars.Read</span></span> |
|[<span data-ttu-id="688a9-149">grupo</span><span class="sxs-lookup"><span data-stu-id="688a9-149">group</span></span>](../resources/group.md) | <span data-ttu-id="688a9-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-150">Group.Read.All</span></span> | <span data-ttu-id="688a9-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-151">Not supported</span></span> | <span data-ttu-id="688a9-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-152">Group.Read.All</span></span> |
|[<span data-ttu-id="688a9-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="688a9-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="688a9-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-154">Group.Read.All</span></span> | <span data-ttu-id="688a9-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-155">Not supported</span></span> | <span data-ttu-id="688a9-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-156">Not supported</span></span> |
|[<span data-ttu-id="688a9-157">list</span><span class="sxs-lookup"><span data-stu-id="688a9-157">list</span></span>](../resources/list.md) | <span data-ttu-id="688a9-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="688a9-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-159">Not supported</span></span> | <span data-ttu-id="688a9-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="688a9-161">message</span><span class="sxs-lookup"><span data-stu-id="688a9-161">message</span></span>](../resources/message.md) | <span data-ttu-id="688a9-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="688a9-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="688a9-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="688a9-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="688a9-165">presence</span><span class="sxs-lookup"><span data-stu-id="688a9-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="688a9-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-166">Presence.Read.All</span></span> | <span data-ttu-id="688a9-167">Incompatível</span><span class="sxs-lookup"><span data-stu-id="688a9-167">Not supported</span></span> | <span data-ttu-id="688a9-168">Incompatível</span><span class="sxs-lookup"><span data-stu-id="688a9-168">Not supported</span></span> |
|[<span data-ttu-id="688a9-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="688a9-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="688a9-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="688a9-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="688a9-171">Not supported</span></span> | <span data-ttu-id="688a9-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="688a9-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="688a9-173">user</span></span>](../resources/user.md) | <span data-ttu-id="688a9-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-174">User.Read.All</span></span> | <span data-ttu-id="688a9-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-175">User.Read.All</span></span> | <span data-ttu-id="688a9-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="688a9-176">User.Read.All</span></span> |

> <span data-ttu-id="688a9-177">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="688a9-177">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="688a9-178">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688a9-178">chatMessage</span></span>

<span data-ttu-id="688a9-179">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="688a9-179">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="688a9-180">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="688a9-180">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="688a9-181">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="688a9-181">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="688a9-182">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="688a9-182">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="688a9-183">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="688a9-183">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="688a9-184">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="688a9-184">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="688a9-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="688a9-185">driveItem</span></span>

<span data-ttu-id="688a9-186">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="688a9-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="688a9-187">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="688a9-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="688a9-188">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="688a9-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="688a9-189">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="688a9-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="688a9-190">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="688a9-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="688a9-191">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="688a9-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="688a9-192">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="688a9-192">contact, event, and message</span></span>

<span data-ttu-id="688a9-193">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="688a9-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="688a9-194">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="688a9-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="688a9-195">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="688a9-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="688a9-196">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="688a9-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="688a9-197">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="688a9-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="688a9-198">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="688a9-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="688a9-199">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="688a9-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="688a9-200">presença</span><span class="sxs-lookup"><span data-stu-id="688a9-200">presence</span></span>

<span data-ttu-id="688a9-201">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="688a9-201">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="688a9-202">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="688a9-202">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="688a9-203">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="688a9-203">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="688a9-204">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="688a9-204">Request headers</span></span>

| <span data-ttu-id="688a9-205">Nome</span><span class="sxs-lookup"><span data-stu-id="688a9-205">Name</span></span>       | <span data-ttu-id="688a9-206">Tipo</span><span class="sxs-lookup"><span data-stu-id="688a9-206">Type</span></span> | <span data-ttu-id="688a9-207">Descrição</span><span class="sxs-lookup"><span data-stu-id="688a9-207">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="688a9-208">Autorização</span><span class="sxs-lookup"><span data-stu-id="688a9-208">Authorization</span></span>  | <span data-ttu-id="688a9-209">string</span><span class="sxs-lookup"><span data-stu-id="688a9-209">string</span></span>  | <span data-ttu-id="688a9-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="688a9-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="688a9-212">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="688a9-212">Request body</span></span>

<span data-ttu-id="688a9-213">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="688a9-213">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="688a9-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="688a9-214">Response</span></span>

<span data-ttu-id="688a9-215">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="688a9-215">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="688a9-216">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="688a9-216">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="688a9-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="688a9-217">Example</span></span>

##### <a name="request"></a><span data-ttu-id="688a9-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="688a9-218">Request</span></span>

<span data-ttu-id="688a9-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="688a9-219">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="688a9-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="688a9-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="688a9-221">C#</span><span class="sxs-lookup"><span data-stu-id="688a9-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="688a9-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="688a9-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="688a9-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="688a9-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="688a9-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="688a9-224">Response</span></span>

<span data-ttu-id="688a9-225">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="688a9-225">Here is an example of the response.</span></span>
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


