---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 641345f403205c7babed381a393b715d44f5e3f9
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848212"
---
# <a name="create-subscription"></a><span data-ttu-id="a0366-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="a0366-103">Create subscription</span></span>

<span data-ttu-id="a0366-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0366-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0366-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a0366-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0366-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0366-106">Permissions</span></span>

<span data-ttu-id="a0366-107">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a0366-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="a0366-108">Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="a0366-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="a0366-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="a0366-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a0366-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0366-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0366-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-111">Supported resource</span></span> | <span data-ttu-id="a0366-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0366-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0366-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0366-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0366-114">Application</span><span class="sxs-lookup"><span data-stu-id="a0366-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="a0366-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="a0366-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="a0366-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="a0366-116">Not supported</span></span> | <span data-ttu-id="a0366-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="a0366-117">Not supported</span></span> | <span data-ttu-id="a0366-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="a0366-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a0366-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="a0366-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="a0366-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-121">Not supported</span></span> | <span data-ttu-id="a0366-122">ChannelMessage. Read. Group \*, ChannelMessage. Read. All</span><span class="sxs-lookup"><span data-stu-id="a0366-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a0366-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="a0366-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="a0366-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-124">Not supported</span></span> | <span data-ttu-id="a0366-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-125">Not supported</span></span> | <span data-ttu-id="a0366-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a0366-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a0366-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="a0366-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0366-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="a0366-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-129">Not supported</span></span> | <span data-ttu-id="a0366-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="a0366-131">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="a0366-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="a0366-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-132">Not supported</span></span> | <span data-ttu-id="a0366-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-133">Not supported</span></span> | <span data-ttu-id="a0366-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="a0366-135">contato</span><span class="sxs-lookup"><span data-stu-id="a0366-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a0366-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-136">Contacts.Read</span></span> | <span data-ttu-id="a0366-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-137">Contacts.Read</span></span> | <span data-ttu-id="a0366-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-138">Contacts.Read</span></span> |
|<span data-ttu-id="a0366-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="a0366-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a0366-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-140">Not supported</span></span> | <span data-ttu-id="a0366-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0366-141">Files.ReadWrite</span></span> | <span data-ttu-id="a0366-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-142">Not supported</span></span> |
|<span data-ttu-id="a0366-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a0366-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a0366-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="a0366-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-145">Not supported</span></span> | <span data-ttu-id="a0366-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a0366-147">evento</span><span class="sxs-lookup"><span data-stu-id="a0366-147">event</span></span>](../resources/event.md) | <span data-ttu-id="a0366-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-148">Calendars.Read</span></span> | <span data-ttu-id="a0366-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-149">Calendars.Read</span></span> | <span data-ttu-id="a0366-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-150">Calendars.Read</span></span> |
|[<span data-ttu-id="a0366-151">grupo</span><span class="sxs-lookup"><span data-stu-id="a0366-151">group</span></span>](../resources/group.md) | <span data-ttu-id="a0366-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-152">Group.Read.All</span></span> | <span data-ttu-id="a0366-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-153">Not supported</span></span> | <span data-ttu-id="a0366-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-154">Group.Read.All</span></span> |
|[<span data-ttu-id="a0366-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="a0366-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a0366-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-156">Group.Read.All</span></span> | <span data-ttu-id="a0366-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-157">Not supported</span></span> | <span data-ttu-id="a0366-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-158">Not supported</span></span> |
|[<span data-ttu-id="a0366-159">list</span><span class="sxs-lookup"><span data-stu-id="a0366-159">list</span></span>](../resources/list.md) | <span data-ttu-id="a0366-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="a0366-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-161">Not supported</span></span> | <span data-ttu-id="a0366-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="a0366-163">message</span><span class="sxs-lookup"><span data-stu-id="a0366-163">message</span></span>](../resources/message.md) | <span data-ttu-id="a0366-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a0366-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a0366-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a0366-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="a0366-167">presence</span><span class="sxs-lookup"><span data-stu-id="a0366-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="a0366-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-168">Presence.Read.All</span></span> | <span data-ttu-id="a0366-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-169">Not supported</span></span> | <span data-ttu-id="a0366-170">Incompatível</span><span class="sxs-lookup"><span data-stu-id="a0366-170">Not supported</span></span> |
|[<span data-ttu-id="a0366-171">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="a0366-171">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="a0366-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-172">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a0366-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0366-173">Not supported</span></span> | <span data-ttu-id="a0366-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0366-174">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a0366-175">Usuário</span><span class="sxs-lookup"><span data-stu-id="a0366-175">user</span></span>](../resources/user.md) | <span data-ttu-id="a0366-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-176">User.Read.All</span></span> | <span data-ttu-id="a0366-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-177">User.Read.All</span></span> | <span data-ttu-id="a0366-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0366-178">User.Read.All</span></span> |

> <span data-ttu-id="a0366-179">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a0366-179">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="a0366-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a0366-180">chatMessage</span></span>

<span data-ttu-id="a0366-181">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o **includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="a0366-181">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="a0366-182">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="a0366-182">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="a0366-183">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="a0366-183">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="a0366-184">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="a0366-184">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="a0366-185">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="a0366-185">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="a0366-186">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="a0366-186">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="a0366-187">**Observação:**`/chats/getAllMessages` retorna apenas mensagens de bate papo pertencentes ao locatário.</span><span class="sxs-lookup"><span data-stu-id="a0366-187">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="a0366-188">Se um thread de bate papo for iniciado por um usuário fora do locatário, esse thread de bate papo não será de propriedade do locatário e não criará notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="a0366-188">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="a0366-189">driveItem</span><span class="sxs-lookup"><span data-stu-id="a0366-189">driveItem</span></span>

<span data-ttu-id="a0366-190">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a0366-190">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="a0366-191">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="a0366-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="a0366-192">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="a0366-192">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a0366-193">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="a0366-193">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a0366-194">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="a0366-194">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="a0366-195">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="a0366-195">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="a0366-196">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="a0366-196">contact, event, and message</span></span>

<span data-ttu-id="a0366-197">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a0366-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="a0366-198">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="a0366-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="a0366-199">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a0366-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a0366-200">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="a0366-200">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a0366-201">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="a0366-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a0366-202">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="a0366-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a0366-203">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="a0366-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="a0366-204">presença</span><span class="sxs-lookup"><span data-stu-id="a0366-204">presence</span></span>

<span data-ttu-id="a0366-205">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="a0366-205">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="a0366-206">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="a0366-206">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0366-207">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0366-207">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="a0366-208">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0366-208">Request headers</span></span>

| <span data-ttu-id="a0366-209">Nome</span><span class="sxs-lookup"><span data-stu-id="a0366-209">Name</span></span>       | <span data-ttu-id="a0366-210">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0366-210">Type</span></span> | <span data-ttu-id="a0366-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0366-211">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a0366-212">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0366-212">Authorization</span></span>  | <span data-ttu-id="a0366-213">string</span><span class="sxs-lookup"><span data-stu-id="a0366-213">string</span></span>  | <span data-ttu-id="a0366-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0366-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a0366-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0366-216">Response</span></span>

<span data-ttu-id="a0366-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0366-217">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="a0366-218">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a0366-218">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="a0366-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0366-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0366-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0366-220">Request</span></span>

<span data-ttu-id="a0366-221">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="a0366-221">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="a0366-222">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="a0366-222">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="a0366-223">Esta solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="a0366-223">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0366-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0366-224">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a0366-225">C#</span><span class="sxs-lookup"><span data-stu-id="a0366-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0366-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0366-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0366-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0366-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a0366-228">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="a0366-228">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="a0366-229">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="a0366-229">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="a0366-230">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="a0366-230">Resources examples</span></span>

<span data-ttu-id="a0366-231">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="a0366-231">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="a0366-232">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="a0366-232">Resource type</span></span> | <span data-ttu-id="a0366-233">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0366-233">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="a0366-234">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="a0366-234">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="a0366-235">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="a0366-235">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a0366-236">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span><span class="sxs-lookup"><span data-stu-id="a0366-236">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span></span> |
|[<span data-ttu-id="a0366-237">Contatos</span><span class="sxs-lookup"><span data-stu-id="a0366-237">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="a0366-238">Conversas</span><span class="sxs-lookup"><span data-stu-id="a0366-238">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="a0366-239">Unidades</span><span class="sxs-lookup"><span data-stu-id="a0366-239">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="a0366-240">Eventos</span><span class="sxs-lookup"><span data-stu-id="a0366-240">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="a0366-241">Grupos</span><span class="sxs-lookup"><span data-stu-id="a0366-241">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="a0366-242">Lista</span><span class="sxs-lookup"><span data-stu-id="a0366-242">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="a0366-243">Email</span><span class="sxs-lookup"><span data-stu-id="a0366-243">Mail</span></span>](../resources/message.md)|<span data-ttu-id="a0366-244">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="a0366-244">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="a0366-245">Presença</span><span class="sxs-lookup"><span data-stu-id="a0366-245">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="a0366-246">`/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="a0366-246">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="a0366-247">Usuários</span><span class="sxs-lookup"><span data-stu-id="a0366-247">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="a0366-248">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="a0366-248">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="a0366-249">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="a0366-249">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="a0366-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0366-250">Response</span></span>

<span data-ttu-id="a0366-251">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0366-251">The following example shows the response.</span></span> 

><span data-ttu-id="a0366-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0366-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="a0366-254">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="a0366-254">Notification endpoint validation</span></span>

<span data-ttu-id="a0366-255">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="a0366-255">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="a0366-256">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="a0366-256">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


