---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 850d0f893678ce51e502dcdeb560f816b5ff935c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597428"
---
# <a name="create-subscription"></a><span data-ttu-id="bf157-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="bf157-103">Create subscription</span></span>

<span data-ttu-id="bf157-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf157-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf157-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bf157-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf157-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf157-106">Permissions</span></span>

<span data-ttu-id="bf157-107">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="bf157-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="bf157-108">Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="bf157-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="bf157-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="bf157-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="bf157-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf157-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf157-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-111">Supported resource</span></span> | <span data-ttu-id="bf157-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf157-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf157-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf157-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf157-114">Application</span><span class="sxs-lookup"><span data-stu-id="bf157-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="bf157-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="bf157-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="bf157-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="bf157-116">Not supported</span></span> | <span data-ttu-id="bf157-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="bf157-117">Not supported</span></span> | <span data-ttu-id="bf157-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="bf157-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="bf157-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="bf157-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="bf157-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-121">Not supported</span></span> | <span data-ttu-id="bf157-122">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="bf157-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="bf157-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="bf157-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="bf157-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-124">Not supported</span></span> | <span data-ttu-id="bf157-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-125">Not supported</span></span> | <span data-ttu-id="bf157-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="bf157-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="bf157-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="bf157-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf157-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="bf157-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-129">Not supported</span></span> | <span data-ttu-id="bf157-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="bf157-131">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="bf157-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="bf157-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-132">Not supported</span></span> | <span data-ttu-id="bf157-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-133">Not supported</span></span> | <span data-ttu-id="bf157-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="bf157-135">contato</span><span class="sxs-lookup"><span data-stu-id="bf157-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="bf157-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-136">Contacts.Read</span></span> | <span data-ttu-id="bf157-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-137">Contacts.Read</span></span> | <span data-ttu-id="bf157-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-138">Contacts.Read</span></span> |
|<span data-ttu-id="bf157-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="bf157-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="bf157-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-140">Not supported</span></span> | <span data-ttu-id="bf157-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf157-141">Files.ReadWrite</span></span> | <span data-ttu-id="bf157-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-142">Not supported</span></span> |
|<span data-ttu-id="bf157-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="bf157-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="bf157-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="bf157-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-145">Not supported</span></span> | <span data-ttu-id="bf157-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf157-147">evento</span><span class="sxs-lookup"><span data-stu-id="bf157-147">event</span></span>](../resources/event.md) | <span data-ttu-id="bf157-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-148">Calendars.Read</span></span> | <span data-ttu-id="bf157-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-149">Calendars.Read</span></span> | <span data-ttu-id="bf157-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-150">Calendars.Read</span></span> |
|[<span data-ttu-id="bf157-151">grupo</span><span class="sxs-lookup"><span data-stu-id="bf157-151">group</span></span>](../resources/group.md) | <span data-ttu-id="bf157-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-152">Group.Read.All</span></span> | <span data-ttu-id="bf157-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-153">Not supported</span></span> | <span data-ttu-id="bf157-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-154">Group.Read.All</span></span> |
|[<span data-ttu-id="bf157-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="bf157-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="bf157-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-156">Group.Read.All</span></span> | <span data-ttu-id="bf157-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-157">Not supported</span></span> | <span data-ttu-id="bf157-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-158">Not supported</span></span> |
|[<span data-ttu-id="bf157-159">list</span><span class="sxs-lookup"><span data-stu-id="bf157-159">list</span></span>](../resources/list.md) | <span data-ttu-id="bf157-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="bf157-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-161">Not supported</span></span> | <span data-ttu-id="bf157-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf157-163">message</span><span class="sxs-lookup"><span data-stu-id="bf157-163">message</span></span>](../resources/message.md) | <span data-ttu-id="bf157-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bf157-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bf157-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf157-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="bf157-167">presence</span><span class="sxs-lookup"><span data-stu-id="bf157-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="bf157-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-168">Presence.Read.All</span></span> | <span data-ttu-id="bf157-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-169">Not supported</span></span> | <span data-ttu-id="bf157-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-170">Not supported</span></span> |
|[<span data-ttu-id="bf157-171">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="bf157-171">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="bf157-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-172">Not supported</span></span> | <span data-ttu-id="bf157-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-173">Not supported</span></span> | <span data-ttu-id="bf157-174">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-174">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf157-175">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="bf157-175">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="bf157-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-176">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="bf157-177">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-177">Not supported</span></span> | <span data-ttu-id="bf157-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf157-178">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf157-179">todoTask</span><span class="sxs-lookup"><span data-stu-id="bf157-179">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="bf157-180">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf157-180">Tasks.ReadWrite</span></span> | <span data-ttu-id="bf157-181">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf157-181">Tasks.ReadWrite</span></span> | <span data-ttu-id="bf157-182">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bf157-182">Not supported</span></span> |
|[<span data-ttu-id="bf157-183">Usuário</span><span class="sxs-lookup"><span data-stu-id="bf157-183">user</span></span>](../resources/user.md) | <span data-ttu-id="bf157-184">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-184">User.Read.All</span></span> | <span data-ttu-id="bf157-185">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-185">User.Read.All</span></span> | <span data-ttu-id="bf157-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf157-186">User.Read.All</span></span> |

> <span data-ttu-id="bf157-187">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bf157-187">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="bf157-188">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bf157-188">chatMessage</span></span>

<span data-ttu-id="bf157-189">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="bf157-189">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="bf157-190">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="bf157-190">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="bf157-191">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="bf157-191">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="bf157-192">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="bf157-192">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="bf157-193">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="bf157-193">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="bf157-194">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="bf157-194">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="bf157-195">**Observação:** `/chats/getAllMessages` retorna somente mensagens de chats pertencentes ao locatário.</span><span class="sxs-lookup"><span data-stu-id="bf157-195">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="bf157-196">Se um thread de chat é iniciado por um usuário fora do locatário, esse thread de chat não pertence ao locatário e não cria notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="bf157-196">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="bf157-197">driveItem</span><span class="sxs-lookup"><span data-stu-id="bf157-197">driveItem</span></span>

<span data-ttu-id="bf157-198">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bf157-198">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="bf157-199">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="bf157-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="bf157-200">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="bf157-200">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="bf157-201">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="bf157-201">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="bf157-202">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="bf157-202">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="bf157-203">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="bf157-203">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="bf157-204">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="bf157-204">contact, event, and message</span></span>

<span data-ttu-id="bf157-205">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="bf157-205">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="bf157-206">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="bf157-206">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="bf157-207">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="bf157-207">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="bf157-208">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="bf157-208">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="bf157-209">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="bf157-209">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="bf157-210">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="bf157-210">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="bf157-211">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="bf157-211">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="bf157-212">presença</span><span class="sxs-lookup"><span data-stu-id="bf157-212">presence</span></span>

<span data-ttu-id="bf157-213">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="bf157-213">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="bf157-214">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="bf157-214">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf157-215">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf157-215">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="bf157-216">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf157-216">Request headers</span></span>

| <span data-ttu-id="bf157-217">Nome</span><span class="sxs-lookup"><span data-stu-id="bf157-217">Name</span></span>       | <span data-ttu-id="bf157-218">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf157-218">Type</span></span> | <span data-ttu-id="bf157-219">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf157-219">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bf157-220">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf157-220">Authorization</span></span>  | <span data-ttu-id="bf157-221">string</span><span class="sxs-lookup"><span data-stu-id="bf157-221">string</span></span>  | <span data-ttu-id="bf157-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf157-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bf157-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf157-224">Response</span></span>

<span data-ttu-id="bf157-225">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf157-225">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="bf157-226">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="bf157-226">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="bf157-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf157-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf157-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf157-228">Request</span></span>

<span data-ttu-id="bf157-229">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="bf157-229">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="bf157-230">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="bf157-230">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="bf157-231">Esta solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="bf157-231">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf157-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf157-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="bf157-233">C#</span><span class="sxs-lookup"><span data-stu-id="bf157-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf157-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf157-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf157-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf157-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf157-236">Java</span><span class="sxs-lookup"><span data-stu-id="bf157-236">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bf157-237">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="bf157-237">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="bf157-238">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="bf157-238">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="bf157-239">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="bf157-239">Resources examples</span></span>

<span data-ttu-id="bf157-240">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="bf157-240">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="bf157-241">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="bf157-241">Resource type</span></span> | <span data-ttu-id="bf157-242">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bf157-242">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="bf157-243">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="bf157-243">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="bf157-244">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="bf157-244">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="bf157-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="bf157-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="bf157-246">Contatos</span><span class="sxs-lookup"><span data-stu-id="bf157-246">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="bf157-247">Conversas</span><span class="sxs-lookup"><span data-stu-id="bf157-247">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="bf157-248">Unidades</span><span class="sxs-lookup"><span data-stu-id="bf157-248">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="bf157-249">Eventos</span><span class="sxs-lookup"><span data-stu-id="bf157-249">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="bf157-250">Grupos</span><span class="sxs-lookup"><span data-stu-id="bf157-250">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="bf157-251">Lista</span><span class="sxs-lookup"><span data-stu-id="bf157-251">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="bf157-252">Email</span><span class="sxs-lookup"><span data-stu-id="bf157-252">Mail</span></span>](../resources/message.md)|<span data-ttu-id="bf157-253">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="bf157-253">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="bf157-254">Presença</span><span class="sxs-lookup"><span data-stu-id="bf157-254">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="bf157-255">`/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="bf157-255">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="bf157-256">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="bf157-256">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="bf157-257">Usuários</span><span class="sxs-lookup"><span data-stu-id="bf157-257">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="bf157-258">todoTask</span><span class="sxs-lookup"><span data-stu-id="bf157-258">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="bf157-259">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="bf157-259">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="bf157-260">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="bf157-260">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="bf157-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf157-261">Response</span></span>

<span data-ttu-id="bf157-262">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="bf157-262">The following example shows the response.</span></span> 

><span data-ttu-id="bf157-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf157-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="bf157-265">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="bf157-265">Notification endpoint validation</span></span>

<span data-ttu-id="bf157-266">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="bf157-266">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="bf157-267">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="bf157-267">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

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


