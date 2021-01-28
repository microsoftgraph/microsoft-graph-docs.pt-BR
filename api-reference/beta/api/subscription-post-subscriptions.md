---
title: Criar assinatura
description: Assina um aplicativo ouvinte para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterações.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 68e748a054812350c7aad029d604e87aa77b7345
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034272"
---
# <a name="create-subscription"></a><span data-ttu-id="72c11-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="72c11-103">Create subscription</span></span>

<span data-ttu-id="72c11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72c11-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="72c11-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="72c11-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72c11-106">Permissions</span></span>

<span data-ttu-id="72c11-107">Criar uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="72c11-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="72c11-108">Por exemplo, para receber notificações de alteração em mensagens, seu aplicativo precisa da permissão Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="72c11-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="72c11-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="72c11-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="72c11-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c11-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72c11-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-111">Supported resource</span></span> | <span data-ttu-id="72c11-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72c11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72c11-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72c11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72c11-114">Application</span><span class="sxs-lookup"><span data-stu-id="72c11-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="72c11-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="72c11-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="72c11-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="72c11-116">Not supported</span></span> | <span data-ttu-id="72c11-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="72c11-117">Not supported</span></span> | <span data-ttu-id="72c11-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="72c11-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="72c11-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="72c11-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="72c11-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-121">Not supported</span></span> | <span data-ttu-id="72c11-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="72c11-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="72c11-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="72c11-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-124">Not supported</span></span> | <span data-ttu-id="72c11-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-125">Not supported</span></span> | <span data-ttu-id="72c11-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="72c11-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="72c11-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="72c11-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72c11-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="72c11-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-129">Not supported</span></span> | <span data-ttu-id="72c11-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="72c11-131">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="72c11-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="72c11-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-132">Not supported</span></span> | <span data-ttu-id="72c11-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-133">Not supported</span></span> | <span data-ttu-id="72c11-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="72c11-135">contato</span><span class="sxs-lookup"><span data-stu-id="72c11-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="72c11-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-136">Contacts.Read</span></span> | <span data-ttu-id="72c11-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-137">Contacts.Read</span></span> | <span data-ttu-id="72c11-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-138">Contacts.Read</span></span> |
|<span data-ttu-id="72c11-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="72c11-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="72c11-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-140">Not supported</span></span> | <span data-ttu-id="72c11-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72c11-141">Files.ReadWrite</span></span> | <span data-ttu-id="72c11-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-142">Not supported</span></span> |
|<span data-ttu-id="72c11-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="72c11-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="72c11-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="72c11-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-145">Not supported</span></span> | <span data-ttu-id="72c11-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="72c11-147">evento</span><span class="sxs-lookup"><span data-stu-id="72c11-147">event</span></span>](../resources/event.md) | <span data-ttu-id="72c11-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-148">Calendars.Read</span></span> | <span data-ttu-id="72c11-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-149">Calendars.Read</span></span> | <span data-ttu-id="72c11-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-150">Calendars.Read</span></span> |
|[<span data-ttu-id="72c11-151">grupo</span><span class="sxs-lookup"><span data-stu-id="72c11-151">group</span></span>](../resources/group.md) | <span data-ttu-id="72c11-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-152">Group.Read.All</span></span> | <span data-ttu-id="72c11-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-153">Not supported</span></span> | <span data-ttu-id="72c11-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-154">Group.Read.All</span></span> |
|[<span data-ttu-id="72c11-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="72c11-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="72c11-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-156">Group.Read.All</span></span> | <span data-ttu-id="72c11-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-157">Not supported</span></span> | <span data-ttu-id="72c11-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-158">Not supported</span></span> |
|[<span data-ttu-id="72c11-159">list</span><span class="sxs-lookup"><span data-stu-id="72c11-159">list</span></span>](../resources/list.md) | <span data-ttu-id="72c11-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="72c11-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-161">Not supported</span></span> | <span data-ttu-id="72c11-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="72c11-163">message</span><span class="sxs-lookup"><span data-stu-id="72c11-163">message</span></span>](../resources/message.md) | <span data-ttu-id="72c11-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="72c11-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="72c11-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72c11-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="72c11-167">presence</span><span class="sxs-lookup"><span data-stu-id="72c11-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="72c11-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-168">Presence.Read.All</span></span> | <span data-ttu-id="72c11-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-169">Not supported</span></span> | <span data-ttu-id="72c11-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-170">Not supported</span></span> |
|[<span data-ttu-id="72c11-171">impressora</span><span class="sxs-lookup"><span data-stu-id="72c11-171">printer</span></span>](../resources/printer.md) | <span data-ttu-id="72c11-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-172">Not supported</span></span> | <span data-ttu-id="72c11-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-173">Not supported</span></span> | <span data-ttu-id="72c11-174">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-174">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="72c11-175">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="72c11-175">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="72c11-176">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-176">Not supported</span></span> | <span data-ttu-id="72c11-177">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-177">Not supported</span></span> | <span data-ttu-id="72c11-178">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-178">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="72c11-179">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="72c11-179">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="72c11-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-180">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="72c11-181">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-181">Not supported</span></span> | <span data-ttu-id="72c11-182">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c11-182">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="72c11-183">todoTask</span><span class="sxs-lookup"><span data-stu-id="72c11-183">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="72c11-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72c11-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="72c11-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72c11-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="72c11-186">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="72c11-186">Not supported</span></span> |
|[<span data-ttu-id="72c11-187">Usuário</span><span class="sxs-lookup"><span data-stu-id="72c11-187">user</span></span>](../resources/user.md) | <span data-ttu-id="72c11-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-188">User.Read.All</span></span> | <span data-ttu-id="72c11-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-189">User.Read.All</span></span> | <span data-ttu-id="72c11-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c11-190">User.Read.All</span></span> |

> <span data-ttu-id="72c11-191">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="72c11-191">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="72c11-192">driveItem</span><span class="sxs-lookup"><span data-stu-id="72c11-192">driveItem</span></span>

<span data-ttu-id="72c11-193">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="72c11-193">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="72c11-194">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="72c11-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="72c11-195">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="72c11-195">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="72c11-196">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="72c11-196">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="72c11-197">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="72c11-197">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="72c11-198">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="72c11-198">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="72c11-199">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="72c11-199">contact, event, and message</span></span>

<span data-ttu-id="72c11-200">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="72c11-200">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="72c11-201">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="72c11-201">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="72c11-202">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="72c11-202">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="72c11-203">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="72c11-203">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="72c11-204">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="72c11-204">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="72c11-205">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="72c11-205">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="72c11-206">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="72c11-206">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="72c11-207">presença</span><span class="sxs-lookup"><span data-stu-id="72c11-207">presence</span></span>

<span data-ttu-id="72c11-208">**assinaturas** de presença [exigem criptografia.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="72c11-208">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="72c11-209">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="72c11-209">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="72c11-210">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72c11-210">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="72c11-211">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72c11-211">Request headers</span></span>

| <span data-ttu-id="72c11-212">Nome</span><span class="sxs-lookup"><span data-stu-id="72c11-212">Name</span></span>       | <span data-ttu-id="72c11-213">Tipo</span><span class="sxs-lookup"><span data-stu-id="72c11-213">Type</span></span> | <span data-ttu-id="72c11-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="72c11-214">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="72c11-215">Autorização</span><span class="sxs-lookup"><span data-stu-id="72c11-215">Authorization</span></span>  | <span data-ttu-id="72c11-216">string</span><span class="sxs-lookup"><span data-stu-id="72c11-216">string</span></span>  | <span data-ttu-id="72c11-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72c11-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="72c11-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="72c11-219">Response</span></span>

<span data-ttu-id="72c11-220">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72c11-220">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="72c11-221">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="72c11-221">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="72c11-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72c11-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="72c11-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72c11-223">Request</span></span>

<span data-ttu-id="72c11-224">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="72c11-224">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="72c11-225">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="72c11-225">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="72c11-226">Essa solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário atualmente assinado.</span><span class="sxs-lookup"><span data-stu-id="72c11-226">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="72c11-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="72c11-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="72c11-228">C#</span><span class="sxs-lookup"><span data-stu-id="72c11-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72c11-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72c11-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72c11-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72c11-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72c11-231">Java</span><span class="sxs-lookup"><span data-stu-id="72c11-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="72c11-232">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="72c11-232">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="72c11-233">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="72c11-233">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="72c11-234">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="72c11-234">Resources examples</span></span>

<span data-ttu-id="72c11-235">A seguir estão os valores válidos para a propriedade de recurso.</span><span class="sxs-lookup"><span data-stu-id="72c11-235">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="72c11-236">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="72c11-236">Resource type</span></span> | <span data-ttu-id="72c11-237">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72c11-237">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="72c11-238">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="72c11-238">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="72c11-239">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="72c11-239">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="72c11-240">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="72c11-240">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="72c11-241">Contatos</span><span class="sxs-lookup"><span data-stu-id="72c11-241">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="72c11-242">Conversas</span><span class="sxs-lookup"><span data-stu-id="72c11-242">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="72c11-243">Unidades</span><span class="sxs-lookup"><span data-stu-id="72c11-243">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="72c11-244">Eventos</span><span class="sxs-lookup"><span data-stu-id="72c11-244">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="72c11-245">Grupos</span><span class="sxs-lookup"><span data-stu-id="72c11-245">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="72c11-246">Lista</span><span class="sxs-lookup"><span data-stu-id="72c11-246">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="72c11-247">Email</span><span class="sxs-lookup"><span data-stu-id="72c11-247">Mail</span></span>](../resources/message.md)|<span data-ttu-id="72c11-248">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="72c11-248">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="72c11-249">Presença</span><span class="sxs-lookup"><span data-stu-id="72c11-249">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="72c11-250">`/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="72c11-250">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="72c11-251">impressora</span><span class="sxs-lookup"><span data-stu-id="72c11-251">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="72c11-252">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="72c11-252">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="72c11-253">Usuários</span><span class="sxs-lookup"><span data-stu-id="72c11-253">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="72c11-254">todoTask</span><span class="sxs-lookup"><span data-stu-id="72c11-254">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="72c11-255">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="72c11-255">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="72c11-256">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="72c11-256">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="72c11-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="72c11-257">Response</span></span>

<span data-ttu-id="72c11-258">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="72c11-258">The following example shows the response.</span></span> 

><span data-ttu-id="72c11-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72c11-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="72c11-261">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="72c11-261">Notification endpoint validation</span></span>

<span data-ttu-id="72c11-262">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl)** deve ser capaz de responder a uma solicitação de validação conforme descrito em Configurar notificações para alterações nos dados [do usuário.](/graph/webhooks#notification-endpoint-validation)</span><span class="sxs-lookup"><span data-stu-id="72c11-262">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="72c11-263">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="72c11-263">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


