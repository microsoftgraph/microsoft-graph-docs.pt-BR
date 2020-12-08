---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f8b9bcae9c9e23b852a94c7700094dccbff1cf75
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597176"
---
# <a name="update-subscription"></a><span data-ttu-id="7f093-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="7f093-103">Update subscription</span></span>

<span data-ttu-id="7f093-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7f093-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f093-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="7f093-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="7f093-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="7f093-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="7f093-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="7f093-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="7f093-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="7f093-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f093-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f093-109">Permissions</span></span>

<span data-ttu-id="7f093-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="7f093-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7f093-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f093-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f093-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-112">Supported resource</span></span> | <span data-ttu-id="7f093-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f093-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7f093-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f093-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f093-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f093-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="7f093-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="7f093-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="7f093-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="7f093-117">Not supported</span></span> | <span data-ttu-id="7f093-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="7f093-118">Not supported</span></span> | <span data-ttu-id="7f093-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="7f093-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7f093-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="7f093-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="7f093-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-122">Not supported</span></span> | <span data-ttu-id="7f093-123">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="7f093-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7f093-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="7f093-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="7f093-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-125">Not supported</span></span> | <span data-ttu-id="7f093-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-126">Not supported</span></span> | <span data-ttu-id="7f093-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7f093-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7f093-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="7f093-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f093-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="7f093-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-130">Not supported</span></span> | <span data-ttu-id="7f093-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="7f093-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="7f093-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="7f093-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-133">Not supported</span></span> | <span data-ttu-id="7f093-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-134">Not supported</span></span> | <span data-ttu-id="7f093-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="7f093-136">contato</span><span class="sxs-lookup"><span data-stu-id="7f093-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="7f093-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7f093-137">Contacts.Read</span></span> | <span data-ttu-id="7f093-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7f093-138">Contacts.Read</span></span> | <span data-ttu-id="7f093-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7f093-139">Contacts.Read</span></span> |
|<span data-ttu-id="7f093-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="7f093-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="7f093-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-141">Not supported</span></span> | <span data-ttu-id="7f093-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f093-142">Files.ReadWrite</span></span> | <span data-ttu-id="7f093-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-143">Not supported</span></span> |
|<span data-ttu-id="7f093-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="7f093-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="7f093-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="7f093-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-146">Not supported</span></span> | <span data-ttu-id="7f093-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f093-148">evento</span><span class="sxs-lookup"><span data-stu-id="7f093-148">event</span></span>](../resources/event.md) | <span data-ttu-id="7f093-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f093-149">Calendars.Read</span></span> | <span data-ttu-id="7f093-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f093-150">Calendars.Read</span></span> | <span data-ttu-id="7f093-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7f093-151">Calendars.Read</span></span> |
|[<span data-ttu-id="7f093-152">grupo</span><span class="sxs-lookup"><span data-stu-id="7f093-152">group</span></span>](../resources/group.md) | <span data-ttu-id="7f093-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-153">Group.Read.All</span></span> | <span data-ttu-id="7f093-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-154">Not supported</span></span> | <span data-ttu-id="7f093-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-155">Group.Read.All</span></span> |
|[<span data-ttu-id="7f093-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="7f093-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="7f093-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-157">Group.Read.All</span></span> | <span data-ttu-id="7f093-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-158">Not supported</span></span> | <span data-ttu-id="7f093-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-159">Not supported</span></span> |
|[<span data-ttu-id="7f093-160">list</span><span class="sxs-lookup"><span data-stu-id="7f093-160">list</span></span>](../resources/list.md) | <span data-ttu-id="7f093-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="7f093-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-162">Not supported</span></span> | <span data-ttu-id="7f093-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f093-164">message</span><span class="sxs-lookup"><span data-stu-id="7f093-164">message</span></span>](../resources/message.md) | <span data-ttu-id="7f093-165">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="7f093-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7f093-166">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="7f093-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7f093-167">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="7f093-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="7f093-168">presence</span><span class="sxs-lookup"><span data-stu-id="7f093-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="7f093-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-169">Presence.Read.All</span></span> | <span data-ttu-id="7f093-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-170">Not supported</span></span> | <span data-ttu-id="7f093-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-171">Not supported</span></span> |
|[<span data-ttu-id="7f093-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7f093-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="7f093-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-173">Not supported</span></span> | <span data-ttu-id="7f093-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-174">Not supported</span></span> | <span data-ttu-id="7f093-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f093-176">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="7f093-176">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="7f093-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="7f093-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-178">Not supported</span></span> | <span data-ttu-id="7f093-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f093-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="7f093-180">todoTask</span><span class="sxs-lookup"><span data-stu-id="7f093-180">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="7f093-181">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f093-181">Tasks.ReadWrite</span></span> | <span data-ttu-id="7f093-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f093-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="7f093-183">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7f093-183">Not supported</span></span> |
|[<span data-ttu-id="7f093-184">Usuário</span><span class="sxs-lookup"><span data-stu-id="7f093-184">user</span></span>](../resources/user.md) | <span data-ttu-id="7f093-185">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-185">User.Read.All</span></span> | <span data-ttu-id="7f093-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-186">User.Read.All</span></span> | <span data-ttu-id="7f093-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f093-187">User.Read.All</span></span> |

> <span data-ttu-id="7f093-188">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="7f093-188">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="7f093-189">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7f093-189">chatMessage</span></span>

<span data-ttu-id="7f093-190">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="7f093-190">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="7f093-191">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="7f093-191">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="7f093-192">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="7f093-192">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="7f093-193">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="7f093-193">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="7f093-194">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="7f093-194">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="7f093-195">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="7f093-195">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="7f093-196">driveItem</span><span class="sxs-lookup"><span data-stu-id="7f093-196">driveItem</span></span>

<span data-ttu-id="7f093-197">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7f093-197">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="7f093-198">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="7f093-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="7f093-199">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="7f093-199">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="7f093-200">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="7f093-200">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="7f093-201">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="7f093-201">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="7f093-202">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="7f093-202">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="7f093-203">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="7f093-203">contact, event, and message</span></span>

<span data-ttu-id="7f093-204">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f093-204">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="7f093-205">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="7f093-205">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="7f093-206">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="7f093-206">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="7f093-207">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="7f093-207">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="7f093-208">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="7f093-208">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="7f093-209">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="7f093-209">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="7f093-210">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="7f093-210">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="7f093-211">presença</span><span class="sxs-lookup"><span data-stu-id="7f093-211">presence</span></span>

<span data-ttu-id="7f093-212">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="7f093-212">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="7f093-213">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="7f093-213">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f093-214">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f093-214">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7f093-215">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f093-215">Request headers</span></span>

| <span data-ttu-id="7f093-216">Nome</span><span class="sxs-lookup"><span data-stu-id="7f093-216">Name</span></span>       | <span data-ttu-id="7f093-217">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f093-217">Type</span></span> | <span data-ttu-id="7f093-218">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f093-218">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f093-219">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f093-219">Authorization</span></span>  | <span data-ttu-id="7f093-220">string</span><span class="sxs-lookup"><span data-stu-id="7f093-220">string</span></span>  | <span data-ttu-id="7f093-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f093-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f093-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f093-223">Response</span></span>

<span data-ttu-id="7f093-224">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f093-224">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="7f093-225">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="7f093-225">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="7f093-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f093-226">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f093-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f093-227">Request</span></span>

<span data-ttu-id="7f093-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f093-228">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f093-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f093-229">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7f093-230">C#</span><span class="sxs-lookup"><span data-stu-id="7f093-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f093-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f093-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f093-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f093-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f093-233">Java</span><span class="sxs-lookup"><span data-stu-id="7f093-233">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f093-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f093-234">Response</span></span>

<span data-ttu-id="7f093-235">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f093-235">Here is an example of the response.</span></span>
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


