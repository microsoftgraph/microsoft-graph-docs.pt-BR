---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5301b2817832738dba7563c063eb288686eab272
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932610"
---
# <a name="delete-subscription"></a><span data-ttu-id="07af1-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="07af1-103">Delete subscription</span></span>

<span data-ttu-id="07af1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07af1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07af1-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="07af1-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="07af1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="07af1-106">Permissions</span></span>

<span data-ttu-id="07af1-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="07af1-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="07af1-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07af1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07af1-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-109">Supported resource</span></span> | <span data-ttu-id="07af1-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07af1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07af1-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07af1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07af1-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07af1-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="07af1-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="07af1-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="07af1-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="07af1-114">Not supported</span></span> | <span data-ttu-id="07af1-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="07af1-115">Not supported</span></span> | <span data-ttu-id="07af1-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="07af1-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="07af1-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="07af1-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="07af1-119">Incompatível</span><span class="sxs-lookup"><span data-stu-id="07af1-119">Not supported</span></span> | <span data-ttu-id="07af1-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="07af1-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="07af1-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="07af1-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-122">Not supported</span></span> | <span data-ttu-id="07af1-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-123">Not supported</span></span> | <span data-ttu-id="07af1-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="07af1-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="07af1-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="07af1-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07af1-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="07af1-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-127">Not supported</span></span> | <span data-ttu-id="07af1-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="07af1-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="07af1-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="07af1-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-130">Not supported</span></span> | <span data-ttu-id="07af1-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-131">Not supported</span></span> | <span data-ttu-id="07af1-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="07af1-133">contato</span><span class="sxs-lookup"><span data-stu-id="07af1-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="07af1-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-134">Contacts.Read</span></span> | <span data-ttu-id="07af1-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-135">Contacts.Read</span></span> | <span data-ttu-id="07af1-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-136">Contacts.Read</span></span> |
|<span data-ttu-id="07af1-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="07af1-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="07af1-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-138">Not supported</span></span> | <span data-ttu-id="07af1-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07af1-139">Files.ReadWrite</span></span> | <span data-ttu-id="07af1-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-140">Not supported</span></span> |
|<span data-ttu-id="07af1-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="07af1-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="07af1-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="07af1-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-143">Not supported</span></span> | <span data-ttu-id="07af1-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="07af1-145">evento</span><span class="sxs-lookup"><span data-stu-id="07af1-145">event</span></span>](../resources/event.md) | <span data-ttu-id="07af1-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-146">Calendars.Read</span></span> | <span data-ttu-id="07af1-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-147">Calendars.Read</span></span> | <span data-ttu-id="07af1-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-148">Calendars.Read</span></span> |
|[<span data-ttu-id="07af1-149">grupo</span><span class="sxs-lookup"><span data-stu-id="07af1-149">group</span></span>](../resources/group.md) | <span data-ttu-id="07af1-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-150">Group.Read.All</span></span> | <span data-ttu-id="07af1-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-151">Not supported</span></span> | <span data-ttu-id="07af1-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-152">Group.Read.All</span></span> |
|[<span data-ttu-id="07af1-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="07af1-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="07af1-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-154">Group.Read.All</span></span> | <span data-ttu-id="07af1-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-155">Not supported</span></span> | <span data-ttu-id="07af1-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-156">Not supported</span></span> |
|[<span data-ttu-id="07af1-157">list</span><span class="sxs-lookup"><span data-stu-id="07af1-157">list</span></span>](../resources/list.md) | <span data-ttu-id="07af1-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="07af1-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-159">Not supported</span></span> | <span data-ttu-id="07af1-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="07af1-161">message</span><span class="sxs-lookup"><span data-stu-id="07af1-161">message</span></span>](../resources/message.md) | <span data-ttu-id="07af1-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="07af1-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="07af1-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07af1-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="07af1-165">presence</span><span class="sxs-lookup"><span data-stu-id="07af1-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="07af1-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-166">Presence.Read.All</span></span> | <span data-ttu-id="07af1-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-167">Not supported</span></span> | <span data-ttu-id="07af1-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-168">Not supported</span></span> |
|[<span data-ttu-id="07af1-169">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="07af1-169">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="07af1-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-170">Not supported</span></span> | <span data-ttu-id="07af1-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-171">Not supported</span></span> | <span data-ttu-id="07af1-172">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-172">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="07af1-173">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="07af1-173">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="07af1-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-174">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="07af1-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="07af1-175">Not supported</span></span> | <span data-ttu-id="07af1-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07af1-176">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="07af1-177">Usuário</span><span class="sxs-lookup"><span data-stu-id="07af1-177">user</span></span>](../resources/user.md) | <span data-ttu-id="07af1-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-178">User.Read.All</span></span> | <span data-ttu-id="07af1-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-179">User.Read.All</span></span> | <span data-ttu-id="07af1-180">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07af1-180">User.Read.All</span></span> |

> <span data-ttu-id="07af1-181">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="07af1-181">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="07af1-182">chatMessage</span><span class="sxs-lookup"><span data-stu-id="07af1-182">chatMessage</span></span>

<span data-ttu-id="07af1-183">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="07af1-183">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="07af1-184">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="07af1-184">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="07af1-185">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="07af1-185">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="07af1-186">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="07af1-186">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="07af1-187">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="07af1-187">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="07af1-188">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="07af1-188">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="07af1-189">driveItem</span><span class="sxs-lookup"><span data-stu-id="07af1-189">driveItem</span></span>

<span data-ttu-id="07af1-190">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="07af1-190">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="07af1-191">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="07af1-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="07af1-192">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="07af1-192">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="07af1-193">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="07af1-193">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="07af1-194">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="07af1-194">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="07af1-195">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="07af1-195">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="07af1-196">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="07af1-196">contact, event, and message</span></span>

<span data-ttu-id="07af1-197">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="07af1-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="07af1-198">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="07af1-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="07af1-199">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="07af1-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="07af1-200">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="07af1-200">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="07af1-201">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="07af1-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="07af1-202">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="07af1-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="07af1-203">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="07af1-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="07af1-204">presença</span><span class="sxs-lookup"><span data-stu-id="07af1-204">presence</span></span>

<span data-ttu-id="07af1-205">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="07af1-205">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="07af1-206">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="07af1-206">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="07af1-207">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07af1-207">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="07af1-208">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07af1-208">Request headers</span></span>

| <span data-ttu-id="07af1-209">Nome</span><span class="sxs-lookup"><span data-stu-id="07af1-209">Name</span></span>       | <span data-ttu-id="07af1-210">Tipo</span><span class="sxs-lookup"><span data-stu-id="07af1-210">Type</span></span> | <span data-ttu-id="07af1-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="07af1-211">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07af1-212">Autorização</span><span class="sxs-lookup"><span data-stu-id="07af1-212">Authorization</span></span>  | <span data-ttu-id="07af1-213">string</span><span class="sxs-lookup"><span data-stu-id="07af1-213">string</span></span>  | <span data-ttu-id="07af1-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07af1-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07af1-216">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07af1-216">Request body</span></span>

<span data-ttu-id="07af1-217">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07af1-217">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07af1-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="07af1-218">Response</span></span>

<span data-ttu-id="07af1-219">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07af1-219">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="07af1-220">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="07af1-220">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="07af1-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07af1-221">Example</span></span>

##### <a name="request"></a><span data-ttu-id="07af1-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07af1-222">Request</span></span>

<span data-ttu-id="07af1-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07af1-223">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07af1-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="07af1-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="07af1-225">C#</span><span class="sxs-lookup"><span data-stu-id="07af1-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07af1-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07af1-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07af1-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07af1-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="07af1-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="07af1-228">Response</span></span>

<span data-ttu-id="07af1-229">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07af1-229">Here is an example of the response.</span></span>
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


