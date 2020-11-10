---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 4d3aea1ae5b8a56cdc4cf39fb97110a8766bde3d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972009"
---
# <a name="update-subscription"></a><span data-ttu-id="59fec-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="59fec-103">Update subscription</span></span>

<span data-ttu-id="59fec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59fec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59fec-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="59fec-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="59fec-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="59fec-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="59fec-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="59fec-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="59fec-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="59fec-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="59fec-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="59fec-109">Permissions</span></span>

<span data-ttu-id="59fec-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="59fec-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="59fec-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59fec-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59fec-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-112">Supported resource</span></span> | <span data-ttu-id="59fec-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59fec-113">Delegated (work or school account)</span></span> | <span data-ttu-id="59fec-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59fec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59fec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59fec-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="59fec-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="59fec-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="59fec-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="59fec-117">Not supported</span></span> | <span data-ttu-id="59fec-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="59fec-118">Not supported</span></span> | <span data-ttu-id="59fec-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="59fec-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="59fec-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="59fec-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="59fec-122">Incompatível</span><span class="sxs-lookup"><span data-stu-id="59fec-122">Not supported</span></span> | <span data-ttu-id="59fec-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="59fec-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="59fec-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="59fec-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-125">Not supported</span></span> | <span data-ttu-id="59fec-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-126">Not supported</span></span> | <span data-ttu-id="59fec-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="59fec-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="59fec-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="59fec-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59fec-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="59fec-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-130">Not supported</span></span> | <span data-ttu-id="59fec-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="59fec-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="59fec-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="59fec-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-133">Not supported</span></span> | <span data-ttu-id="59fec-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-134">Not supported</span></span> | <span data-ttu-id="59fec-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="59fec-136">contato</span><span class="sxs-lookup"><span data-stu-id="59fec-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="59fec-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-137">Contacts.Read</span></span> | <span data-ttu-id="59fec-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-138">Contacts.Read</span></span> | <span data-ttu-id="59fec-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-139">Contacts.Read</span></span> |
|<span data-ttu-id="59fec-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="59fec-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="59fec-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-141">Not supported</span></span> | <span data-ttu-id="59fec-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59fec-142">Files.ReadWrite</span></span> | <span data-ttu-id="59fec-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-143">Not supported</span></span> |
|<span data-ttu-id="59fec-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="59fec-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="59fec-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="59fec-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-146">Not supported</span></span> | <span data-ttu-id="59fec-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="59fec-148">evento</span><span class="sxs-lookup"><span data-stu-id="59fec-148">event</span></span>](../resources/event.md) | <span data-ttu-id="59fec-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-149">Calendars.Read</span></span> | <span data-ttu-id="59fec-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-150">Calendars.Read</span></span> | <span data-ttu-id="59fec-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-151">Calendars.Read</span></span> |
|[<span data-ttu-id="59fec-152">grupo</span><span class="sxs-lookup"><span data-stu-id="59fec-152">group</span></span>](../resources/group.md) | <span data-ttu-id="59fec-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-153">Group.Read.All</span></span> | <span data-ttu-id="59fec-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-154">Not supported</span></span> | <span data-ttu-id="59fec-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-155">Group.Read.All</span></span> |
|[<span data-ttu-id="59fec-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="59fec-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="59fec-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-157">Group.Read.All</span></span> | <span data-ttu-id="59fec-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-158">Not supported</span></span> | <span data-ttu-id="59fec-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-159">Not supported</span></span> |
|[<span data-ttu-id="59fec-160">list</span><span class="sxs-lookup"><span data-stu-id="59fec-160">list</span></span>](../resources/list.md) | <span data-ttu-id="59fec-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="59fec-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-162">Not supported</span></span> | <span data-ttu-id="59fec-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="59fec-164">message</span><span class="sxs-lookup"><span data-stu-id="59fec-164">message</span></span>](../resources/message.md) | <span data-ttu-id="59fec-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="59fec-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="59fec-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="59fec-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="59fec-168">presence</span><span class="sxs-lookup"><span data-stu-id="59fec-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="59fec-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-169">Presence.Read.All</span></span> | <span data-ttu-id="59fec-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-170">Not supported</span></span> | <span data-ttu-id="59fec-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-171">Not supported</span></span> |
|[<span data-ttu-id="59fec-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="59fec-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="59fec-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-173">Not supported</span></span> | <span data-ttu-id="59fec-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-174">Not supported</span></span> | <span data-ttu-id="59fec-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="59fec-176">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="59fec-176">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="59fec-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="59fec-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="59fec-178">Not supported</span></span> | <span data-ttu-id="59fec-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fec-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="59fec-180">Usuário</span><span class="sxs-lookup"><span data-stu-id="59fec-180">user</span></span>](../resources/user.md) | <span data-ttu-id="59fec-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-181">User.Read.All</span></span> | <span data-ttu-id="59fec-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-182">User.Read.All</span></span> | <span data-ttu-id="59fec-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="59fec-183">User.Read.All</span></span> |

> <span data-ttu-id="59fec-184">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="59fec-184">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="59fec-185">chatMessage</span><span class="sxs-lookup"><span data-stu-id="59fec-185">chatMessage</span></span>

<span data-ttu-id="59fec-186">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="59fec-186">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="59fec-187">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="59fec-187">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="59fec-188">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="59fec-188">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="59fec-189">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="59fec-189">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="59fec-190">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="59fec-190">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="59fec-191">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="59fec-191">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="59fec-192">driveItem</span><span class="sxs-lookup"><span data-stu-id="59fec-192">driveItem</span></span>

<span data-ttu-id="59fec-193">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="59fec-193">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="59fec-194">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="59fec-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="59fec-195">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="59fec-195">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="59fec-196">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="59fec-196">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="59fec-197">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="59fec-197">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="59fec-198">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="59fec-198">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="59fec-199">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="59fec-199">contact, event, and message</span></span>

<span data-ttu-id="59fec-200">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="59fec-200">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="59fec-201">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="59fec-201">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="59fec-202">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="59fec-202">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="59fec-203">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="59fec-203">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="59fec-204">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="59fec-204">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="59fec-205">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="59fec-205">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="59fec-206">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="59fec-206">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="59fec-207">presença</span><span class="sxs-lookup"><span data-stu-id="59fec-207">presence</span></span>

<span data-ttu-id="59fec-208">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="59fec-208">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="59fec-209">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="59fec-209">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="59fec-210">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59fec-210">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="59fec-211">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59fec-211">Request headers</span></span>

| <span data-ttu-id="59fec-212">Nome</span><span class="sxs-lookup"><span data-stu-id="59fec-212">Name</span></span>       | <span data-ttu-id="59fec-213">Tipo</span><span class="sxs-lookup"><span data-stu-id="59fec-213">Type</span></span> | <span data-ttu-id="59fec-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="59fec-214">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59fec-215">Autorização</span><span class="sxs-lookup"><span data-stu-id="59fec-215">Authorization</span></span>  | <span data-ttu-id="59fec-216">string</span><span class="sxs-lookup"><span data-stu-id="59fec-216">string</span></span>  | <span data-ttu-id="59fec-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59fec-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="59fec-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="59fec-219">Response</span></span>

<span data-ttu-id="59fec-220">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59fec-220">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="59fec-221">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="59fec-221">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="59fec-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59fec-222">Example</span></span>

##### <a name="request"></a><span data-ttu-id="59fec-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59fec-223">Request</span></span>

<span data-ttu-id="59fec-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59fec-224">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59fec-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="59fec-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="59fec-226">C#</span><span class="sxs-lookup"><span data-stu-id="59fec-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59fec-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59fec-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59fec-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59fec-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59fec-229">Java</span><span class="sxs-lookup"><span data-stu-id="59fec-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59fec-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="59fec-230">Response</span></span>

<span data-ttu-id="59fec-231">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59fec-231">Here is an example of the response.</span></span>
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


