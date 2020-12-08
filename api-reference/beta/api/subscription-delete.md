---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c6e8b1d203b5a14a4d450b459dbadeb06d2cfe45
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597179"
---
# <a name="delete-subscription"></a><span data-ttu-id="25031-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="25031-103">Delete subscription</span></span>

<span data-ttu-id="25031-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="25031-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25031-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="25031-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="25031-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="25031-106">Permissions</span></span>

<span data-ttu-id="25031-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="25031-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="25031-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25031-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25031-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="25031-109">Supported resource</span></span> | <span data-ttu-id="25031-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25031-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25031-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25031-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25031-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25031-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="25031-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="25031-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="25031-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="25031-114">Not supported</span></span> | <span data-ttu-id="25031-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="25031-115">Not supported</span></span> | <span data-ttu-id="25031-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="25031-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="25031-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="25031-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="25031-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-119">Not supported</span></span> | <span data-ttu-id="25031-120">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="25031-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="25031-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="25031-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="25031-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-122">Not supported</span></span> | <span data-ttu-id="25031-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-123">Not supported</span></span> | <span data-ttu-id="25031-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="25031-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="25031-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="25031-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25031-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="25031-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-127">Not supported</span></span> | <span data-ttu-id="25031-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="25031-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="25031-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="25031-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-130">Not supported</span></span> | <span data-ttu-id="25031-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-131">Not supported</span></span> | <span data-ttu-id="25031-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="25031-133">contato</span><span class="sxs-lookup"><span data-stu-id="25031-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="25031-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="25031-134">Contacts.Read</span></span> | <span data-ttu-id="25031-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="25031-135">Contacts.Read</span></span> | <span data-ttu-id="25031-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="25031-136">Contacts.Read</span></span> |
|<span data-ttu-id="25031-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="25031-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="25031-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-138">Not supported</span></span> | <span data-ttu-id="25031-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25031-139">Files.ReadWrite</span></span> | <span data-ttu-id="25031-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-140">Not supported</span></span> |
|<span data-ttu-id="25031-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="25031-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="25031-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="25031-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-143">Not supported</span></span> | <span data-ttu-id="25031-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="25031-145">evento</span><span class="sxs-lookup"><span data-stu-id="25031-145">event</span></span>](../resources/event.md) | <span data-ttu-id="25031-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25031-146">Calendars.Read</span></span> | <span data-ttu-id="25031-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25031-147">Calendars.Read</span></span> | <span data-ttu-id="25031-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="25031-148">Calendars.Read</span></span> |
|[<span data-ttu-id="25031-149">grupo</span><span class="sxs-lookup"><span data-stu-id="25031-149">group</span></span>](../resources/group.md) | <span data-ttu-id="25031-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-150">Group.Read.All</span></span> | <span data-ttu-id="25031-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-151">Not supported</span></span> | <span data-ttu-id="25031-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-152">Group.Read.All</span></span> |
|[<span data-ttu-id="25031-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="25031-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="25031-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-154">Group.Read.All</span></span> | <span data-ttu-id="25031-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-155">Not supported</span></span> | <span data-ttu-id="25031-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-156">Not supported</span></span> |
|[<span data-ttu-id="25031-157">list</span><span class="sxs-lookup"><span data-stu-id="25031-157">list</span></span>](../resources/list.md) | <span data-ttu-id="25031-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="25031-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-159">Not supported</span></span> | <span data-ttu-id="25031-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="25031-161">message</span><span class="sxs-lookup"><span data-stu-id="25031-161">message</span></span>](../resources/message.md) | <span data-ttu-id="25031-162">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="25031-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="25031-163">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="25031-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="25031-164">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="25031-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="25031-165">presence</span><span class="sxs-lookup"><span data-stu-id="25031-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="25031-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-166">Presence.Read.All</span></span> | <span data-ttu-id="25031-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-167">Not supported</span></span> | <span data-ttu-id="25031-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-168">Not supported</span></span> |
|[<span data-ttu-id="25031-169">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="25031-169">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="25031-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-170">Not supported</span></span> | <span data-ttu-id="25031-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-171">Not supported</span></span> | <span data-ttu-id="25031-172">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-172">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="25031-173">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="25031-173">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="25031-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-174">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="25031-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-175">Not supported</span></span> | <span data-ttu-id="25031-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25031-176">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="25031-177">todoTask</span><span class="sxs-lookup"><span data-stu-id="25031-177">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="25031-178">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25031-178">Tasks.ReadWrite</span></span> | <span data-ttu-id="25031-179">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25031-179">Tasks.ReadWrite</span></span> | <span data-ttu-id="25031-180">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="25031-180">Not supported</span></span> |
|[<span data-ttu-id="25031-181">Usuário</span><span class="sxs-lookup"><span data-stu-id="25031-181">user</span></span>](../resources/user.md) | <span data-ttu-id="25031-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-182">User.Read.All</span></span> | <span data-ttu-id="25031-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-183">User.Read.All</span></span> | <span data-ttu-id="25031-184">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="25031-184">User.Read.All</span></span> |

> <span data-ttu-id="25031-185">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="25031-185">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="25031-186">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25031-186">chatMessage</span></span>

<span data-ttu-id="25031-187">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="25031-187">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="25031-188">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="25031-188">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="25031-189">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="25031-189">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="25031-190">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="25031-190">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="25031-191">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="25031-191">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="25031-192">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="25031-192">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="25031-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="25031-193">driveItem</span></span>

<span data-ttu-id="25031-194">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="25031-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="25031-195">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="25031-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="25031-196">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="25031-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="25031-197">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="25031-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="25031-198">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="25031-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="25031-199">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="25031-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="25031-200">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="25031-200">contact, event, and message</span></span>

<span data-ttu-id="25031-201">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="25031-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="25031-202">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="25031-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="25031-203">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="25031-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="25031-204">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="25031-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="25031-205">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="25031-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="25031-206">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="25031-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="25031-207">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="25031-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="25031-208">presença</span><span class="sxs-lookup"><span data-stu-id="25031-208">presence</span></span>

<span data-ttu-id="25031-209">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="25031-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="25031-210">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="25031-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="25031-211">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25031-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="25031-212">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25031-212">Request headers</span></span>

| <span data-ttu-id="25031-213">Nome</span><span class="sxs-lookup"><span data-stu-id="25031-213">Name</span></span>       | <span data-ttu-id="25031-214">Tipo</span><span class="sxs-lookup"><span data-stu-id="25031-214">Type</span></span> | <span data-ttu-id="25031-215">Descrição</span><span class="sxs-lookup"><span data-stu-id="25031-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="25031-216">Autorização</span><span class="sxs-lookup"><span data-stu-id="25031-216">Authorization</span></span>  | <span data-ttu-id="25031-217">string</span><span class="sxs-lookup"><span data-stu-id="25031-217">string</span></span>  | <span data-ttu-id="25031-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25031-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25031-220">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25031-220">Request body</span></span>

<span data-ttu-id="25031-221">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25031-221">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25031-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="25031-222">Response</span></span>

<span data-ttu-id="25031-223">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25031-223">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="25031-224">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="25031-224">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="25031-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25031-225">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25031-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25031-226">Request</span></span>

<span data-ttu-id="25031-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25031-227">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25031-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="25031-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="25031-229">C#</span><span class="sxs-lookup"><span data-stu-id="25031-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25031-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25031-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25031-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25031-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25031-232">Java</span><span class="sxs-lookup"><span data-stu-id="25031-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25031-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="25031-233">Response</span></span>

<span data-ttu-id="25031-234">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25031-234">Here is an example of the response.</span></span>
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


