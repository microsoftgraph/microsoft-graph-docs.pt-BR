---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 855c0463c75bd57e49b2de990a8de69965c34b48
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034261"
---
# <a name="update-subscription"></a><span data-ttu-id="4fb6c-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="4fb6c-103">Update subscription</span></span>

<span data-ttu-id="4fb6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fb6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fb6c-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="4fb6c-106">As assinaturas expiram após um período que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="4fb6c-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar suas assinaturas bem antes de sua data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="4fb6c-108">Consulte [a assinatura](../resources/subscription.md) para a duração máxima de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fb6c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fb6c-109">Permissions</span></span>

<span data-ttu-id="4fb6c-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4fb6c-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fb6c-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fb6c-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-112">Supported resource</span></span> | <span data-ttu-id="4fb6c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4fb6c-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fb6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fb6c-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4fb6c-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="4fb6c-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="4fb6c-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="4fb6c-117">Not supported</span></span> | <span data-ttu-id="4fb6c-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="4fb6c-118">Not supported</span></span> | <span data-ttu-id="4fb6c-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="4fb6c-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="4fb6c-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="4fb6c-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-122">Not supported</span></span> | <span data-ttu-id="4fb6c-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="4fb6c-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="4fb6c-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-125">Not supported</span></span> | <span data-ttu-id="4fb6c-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-126">Not supported</span></span> | <span data-ttu-id="4fb6c-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="4fb6c-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="4fb6c-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fb6c-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="4fb6c-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-130">Not supported</span></span> | <span data-ttu-id="4fb6c-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="4fb6c-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="4fb6c-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-133">Not supported</span></span> | <span data-ttu-id="4fb6c-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-134">Not supported</span></span> | <span data-ttu-id="4fb6c-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="4fb6c-136">contato</span><span class="sxs-lookup"><span data-stu-id="4fb6c-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4fb6c-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-137">Contacts.Read</span></span> | <span data-ttu-id="4fb6c-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-138">Contacts.Read</span></span> | <span data-ttu-id="4fb6c-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-139">Contacts.Read</span></span> |
|<span data-ttu-id="4fb6c-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4fb6c-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-141">Not supported</span></span> | <span data-ttu-id="4fb6c-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fb6c-142">Files.ReadWrite</span></span> | <span data-ttu-id="4fb6c-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-143">Not supported</span></span> |
|<span data-ttu-id="4fb6c-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4fb6c-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="4fb6c-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-146">Not supported</span></span> | <span data-ttu-id="4fb6c-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4fb6c-148">evento</span><span class="sxs-lookup"><span data-stu-id="4fb6c-148">event</span></span>](../resources/event.md) | <span data-ttu-id="4fb6c-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-149">Calendars.Read</span></span> | <span data-ttu-id="4fb6c-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-150">Calendars.Read</span></span> | <span data-ttu-id="4fb6c-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-151">Calendars.Read</span></span> |
|[<span data-ttu-id="4fb6c-152">grupo</span><span class="sxs-lookup"><span data-stu-id="4fb6c-152">group</span></span>](../resources/group.md) | <span data-ttu-id="4fb6c-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-153">Group.Read.All</span></span> | <span data-ttu-id="4fb6c-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-154">Not supported</span></span> | <span data-ttu-id="4fb6c-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-155">Group.Read.All</span></span> |
|[<span data-ttu-id="4fb6c-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="4fb6c-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4fb6c-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-157">Group.Read.All</span></span> | <span data-ttu-id="4fb6c-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-158">Not supported</span></span> | <span data-ttu-id="4fb6c-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-159">Not supported</span></span> |
|[<span data-ttu-id="4fb6c-160">list</span><span class="sxs-lookup"><span data-stu-id="4fb6c-160">list</span></span>](../resources/list.md) | <span data-ttu-id="4fb6c-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="4fb6c-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-162">Not supported</span></span> | <span data-ttu-id="4fb6c-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="4fb6c-164">message</span><span class="sxs-lookup"><span data-stu-id="4fb6c-164">message</span></span>](../resources/message.md) | <span data-ttu-id="4fb6c-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4fb6c-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4fb6c-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4fb6c-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="4fb6c-168">presence</span><span class="sxs-lookup"><span data-stu-id="4fb6c-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="4fb6c-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-169">Presence.Read.All</span></span> | <span data-ttu-id="4fb6c-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-170">Not supported</span></span> | <span data-ttu-id="4fb6c-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-171">Not supported</span></span> |
|[<span data-ttu-id="4fb6c-172">impressora</span><span class="sxs-lookup"><span data-stu-id="4fb6c-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="4fb6c-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-173">Not supported</span></span> | <span data-ttu-id="4fb6c-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-174">Not supported</span></span> | <span data-ttu-id="4fb6c-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="4fb6c-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="4fb6c-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="4fb6c-177">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-177">Not supported</span></span> | <span data-ttu-id="4fb6c-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-178">Not supported</span></span> | <span data-ttu-id="4fb6c-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="4fb6c-180">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="4fb6c-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="4fb6c-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4fb6c-182">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-182">Not supported</span></span> | <span data-ttu-id="4fb6c-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="4fb6c-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="4fb6c-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="4fb6c-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fb6c-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="4fb6c-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fb6c-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="4fb6c-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4fb6c-187">Not supported</span></span> |
|[<span data-ttu-id="4fb6c-188">Usuário</span><span class="sxs-lookup"><span data-stu-id="4fb6c-188">user</span></span>](../resources/user.md) | <span data-ttu-id="4fb6c-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-189">User.Read.All</span></span> | <span data-ttu-id="4fb6c-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-190">User.Read.All</span></span> | <span data-ttu-id="4fb6c-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb6c-191">User.Read.All</span></span> |

> <span data-ttu-id="4fb6c-192">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4fb6c-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="4fb6c-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="4fb6c-193">driveItem</span></span>

<span data-ttu-id="4fb6c-194">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="4fb6c-195">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="4fb6c-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="4fb6c-196">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4fb6c-197">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4fb6c-198">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="4fb6c-199">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="4fb6c-200">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="4fb6c-200">contact, event, and message</span></span>

<span data-ttu-id="4fb6c-201">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="4fb6c-202">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="4fb6c-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="4fb6c-203">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4fb6c-204">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="4fb6c-205">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="4fb6c-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4fb6c-206">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4fb6c-207">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="4fb6c-208">presença</span><span class="sxs-lookup"><span data-stu-id="4fb6c-208">presence</span></span>

<span data-ttu-id="4fb6c-209">**assinaturas** de presença exigem [criptografia.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="4fb6c-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="4fb6c-210">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="4fb6c-211">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fb6c-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4fb6c-212">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fb6c-212">Request headers</span></span>

| <span data-ttu-id="4fb6c-213">Nome</span><span class="sxs-lookup"><span data-stu-id="4fb6c-213">Name</span></span>       | <span data-ttu-id="4fb6c-214">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fb6c-214">Type</span></span> | <span data-ttu-id="4fb6c-215">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fb6c-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4fb6c-216">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fb6c-216">Authorization</span></span>  | <span data-ttu-id="4fb6c-217">string</span><span class="sxs-lookup"><span data-stu-id="4fb6c-217">string</span></span>  | <span data-ttu-id="4fb6c-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4fb6c-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fb6c-220">Response</span></span>

<span data-ttu-id="4fb6c-221">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-221">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="4fb6c-222">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="4fb6c-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="4fb6c-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fb6c-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4fb6c-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fb6c-224">Request</span></span>

<span data-ttu-id="4fb6c-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fb6c-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fb6c-226">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4fb6c-227">C#</span><span class="sxs-lookup"><span data-stu-id="4fb6c-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fb6c-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fb6c-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fb6c-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fb6c-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fb6c-230">Java</span><span class="sxs-lookup"><span data-stu-id="4fb6c-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4fb6c-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fb6c-231">Response</span></span>

<span data-ttu-id="4fb6c-232">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fb6c-232">Here is an example of the response.</span></span>
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


