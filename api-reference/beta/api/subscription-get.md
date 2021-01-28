---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 61860c0ca82fa5f116a52d9ba789807230426741
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034188"
---
# <a name="get-subscription"></a><span data-ttu-id="8a7d7-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="8a7d7-103">Get subscription</span></span>

<span data-ttu-id="8a7d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a7d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a7d7-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a7d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a7d7-106">Permissions</span></span>

<span data-ttu-id="8a7d7-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8a7d7-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a7d7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a7d7-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-109">Supported resource</span></span> | <span data-ttu-id="8a7d7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a7d7-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a7d7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a7d7-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="8a7d7-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="8a7d7-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="8a7d7-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="8a7d7-114">Not supported</span></span> | <span data-ttu-id="8a7d7-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="8a7d7-115">Not supported</span></span> | <span data-ttu-id="8a7d7-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8a7d7-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8a7d7-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="8a7d7-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-119">Not supported</span></span> | <span data-ttu-id="8a7d7-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8a7d7-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8a7d7-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-122">Not supported</span></span> | <span data-ttu-id="8a7d7-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-123">Not supported</span></span> | <span data-ttu-id="8a7d7-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8a7d7-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8a7d7-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7d7-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8a7d7-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-127">Not supported</span></span> | <span data-ttu-id="8a7d7-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="8a7d7-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8a7d7-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-130">Not supported</span></span> | <span data-ttu-id="8a7d7-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-131">Not supported</span></span> | <span data-ttu-id="8a7d7-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8a7d7-133">contato</span><span class="sxs-lookup"><span data-stu-id="8a7d7-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8a7d7-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-134">Contacts.Read</span></span> | <span data-ttu-id="8a7d7-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-135">Contacts.Read</span></span> | <span data-ttu-id="8a7d7-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-136">Contacts.Read</span></span> |
|<span data-ttu-id="8a7d7-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8a7d7-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-138">Not supported</span></span> | <span data-ttu-id="8a7d7-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7d7-139">Files.ReadWrite</span></span> | <span data-ttu-id="8a7d7-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-140">Not supported</span></span> |
|<span data-ttu-id="8a7d7-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8a7d7-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="8a7d7-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-143">Not supported</span></span> | <span data-ttu-id="8a7d7-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8a7d7-145">evento</span><span class="sxs-lookup"><span data-stu-id="8a7d7-145">event</span></span>](../resources/event.md) | <span data-ttu-id="8a7d7-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-146">Calendars.Read</span></span> | <span data-ttu-id="8a7d7-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-147">Calendars.Read</span></span> | <span data-ttu-id="8a7d7-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-148">Calendars.Read</span></span> |
|[<span data-ttu-id="8a7d7-149">grupo</span><span class="sxs-lookup"><span data-stu-id="8a7d7-149">group</span></span>](../resources/group.md) | <span data-ttu-id="8a7d7-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-150">Group.Read.All</span></span> | <span data-ttu-id="8a7d7-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-151">Not supported</span></span> | <span data-ttu-id="8a7d7-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-152">Group.Read.All</span></span> |
|[<span data-ttu-id="8a7d7-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="8a7d7-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8a7d7-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-154">Group.Read.All</span></span> | <span data-ttu-id="8a7d7-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-155">Not supported</span></span> | <span data-ttu-id="8a7d7-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-156">Not supported</span></span> |
|[<span data-ttu-id="8a7d7-157">list</span><span class="sxs-lookup"><span data-stu-id="8a7d7-157">list</span></span>](../resources/list.md) | <span data-ttu-id="8a7d7-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8a7d7-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-159">Not supported</span></span> | <span data-ttu-id="8a7d7-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8a7d7-161">message</span><span class="sxs-lookup"><span data-stu-id="8a7d7-161">message</span></span>](../resources/message.md) | <span data-ttu-id="8a7d7-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8a7d7-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8a7d7-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8a7d7-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8a7d7-165">presence</span><span class="sxs-lookup"><span data-stu-id="8a7d7-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="8a7d7-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-166">Presence.Read.All</span></span> | <span data-ttu-id="8a7d7-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-167">Not supported</span></span> | <span data-ttu-id="8a7d7-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-168">Not supported</span></span> |
|[<span data-ttu-id="8a7d7-169">impressora</span><span class="sxs-lookup"><span data-stu-id="8a7d7-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="8a7d7-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-170">Not supported</span></span> | <span data-ttu-id="8a7d7-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-171">Not supported</span></span> | <span data-ttu-id="8a7d7-172">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="8a7d7-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8a7d7-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="8a7d7-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-174">Not supported</span></span> | <span data-ttu-id="8a7d7-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-175">Not supported</span></span> | <span data-ttu-id="8a7d7-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="8a7d7-177">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="8a7d7-177">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="8a7d7-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8a7d7-179">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-179">Not supported</span></span> | <span data-ttu-id="8a7d7-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="8a7d7-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="8a7d7-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="8a7d7-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7d7-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="8a7d7-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a7d7-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="8a7d7-184">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8a7d7-184">Not supported</span></span> |
|[<span data-ttu-id="8a7d7-185">Usuário</span><span class="sxs-lookup"><span data-stu-id="8a7d7-185">user</span></span>](../resources/user.md) | <span data-ttu-id="8a7d7-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-186">User.Read.All</span></span> | <span data-ttu-id="8a7d7-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-187">User.Read.All</span></span> | <span data-ttu-id="8a7d7-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a7d7-188">User.Read.All</span></span> |

> <span data-ttu-id="8a7d7-189">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8a7d7-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="8a7d7-190">driveItem</span><span class="sxs-lookup"><span data-stu-id="8a7d7-190">driveItem</span></span>

<span data-ttu-id="8a7d7-191">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-191">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="8a7d7-192">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="8a7d7-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8a7d7-193">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-193">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8a7d7-194">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-194">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8a7d7-195">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-195">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8a7d7-196">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-196">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="8a7d7-197">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="8a7d7-197">contact, event, and message</span></span>

<span data-ttu-id="8a7d7-198">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-198">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8a7d7-199">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="8a7d7-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8a7d7-200">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-200">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8a7d7-201">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-201">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8a7d7-202">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="8a7d7-202">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8a7d7-203">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-203">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8a7d7-204">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-204">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="8a7d7-205">presença</span><span class="sxs-lookup"><span data-stu-id="8a7d7-205">presence</span></span>

<span data-ttu-id="8a7d7-206">**assinaturas** de presença [exigem criptografia.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="8a7d7-206">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8a7d7-207">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-207">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a7d7-208">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a7d7-208">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a7d7-209">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8a7d7-209">Optional query parameters</span></span>

<span data-ttu-id="8a7d7-210">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-210">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a7d7-211">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a7d7-211">Request headers</span></span>

| <span data-ttu-id="8a7d7-212">Nome</span><span class="sxs-lookup"><span data-stu-id="8a7d7-212">Name</span></span>       | <span data-ttu-id="8a7d7-213">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a7d7-213">Type</span></span> | <span data-ttu-id="8a7d7-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a7d7-214">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="8a7d7-215">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a7d7-215">Authorization</span></span>  | <span data-ttu-id="8a7d7-216">string</span><span class="sxs-lookup"><span data-stu-id="8a7d7-216">string</span></span>  | <span data-ttu-id="8a7d7-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a7d7-219">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a7d7-219">Request body</span></span>

<span data-ttu-id="8a7d7-220">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-220">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a7d7-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a7d7-221">Response</span></span>

<span data-ttu-id="8a7d7-222">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-222">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a7d7-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a7d7-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a7d7-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a7d7-224">Request</span></span>

<span data-ttu-id="8a7d7-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a7d7-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a7d7-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="8a7d7-227">C#</span><span class="sxs-lookup"><span data-stu-id="8a7d7-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a7d7-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a7d7-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a7d7-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a7d7-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a7d7-230">Java</span><span class="sxs-lookup"><span data-stu-id="8a7d7-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a7d7-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a7d7-231">Response</span></span>

<span data-ttu-id="8a7d7-232">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a7d7-232">Here is an example of the response.</span></span>
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


