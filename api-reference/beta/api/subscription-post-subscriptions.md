---
title: Criar assinatura
description: Inscreve um aplicativo ouvinte para receber notificações de alteração quando os dados em um recurso microsoft Graph alterações.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 7fe6db48038b68d7d2bfe507af60a26846962832
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054872"
---
# <a name="create-subscription"></a><span data-ttu-id="48f4a-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="48f4a-103">Create subscription</span></span>

<span data-ttu-id="48f4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48f4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48f4a-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="48f4a-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="48f4a-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="48f4a-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f4a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="48f4a-107">Permissions</span></span>

<span data-ttu-id="48f4a-108">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="48f4a-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="48f4a-109">Por exemplo, para receber notificações de alteração em mensagens, seu aplicativo precisa da permissão Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="48f4a-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="48f4a-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="48f4a-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="48f4a-111">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f4a-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48f4a-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-112">Supported resource</span></span> | <span data-ttu-id="48f4a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48f4a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48f4a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48f4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f4a-115">Application</span><span class="sxs-lookup"><span data-stu-id="48f4a-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="48f4a-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="48f4a-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="48f4a-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="48f4a-117">Not supported</span></span> | <span data-ttu-id="48f4a-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="48f4a-118">Not supported</span></span> | <span data-ttu-id="48f4a-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="48f4a-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="48f4a-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="48f4a-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="48f4a-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-122">Not supported</span></span> | <span data-ttu-id="48f4a-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="48f4a-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="48f4a-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="48f4a-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-125">Not supported</span></span> | <span data-ttu-id="48f4a-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-126">Not supported</span></span> | <span data-ttu-id="48f4a-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="48f4a-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="48f4a-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="48f4a-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f4a-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="48f4a-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-130">Not supported</span></span> | <span data-ttu-id="48f4a-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="48f4a-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="48f4a-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="48f4a-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-133">Not supported</span></span> | <span data-ttu-id="48f4a-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-134">Not supported</span></span> | <span data-ttu-id="48f4a-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="48f4a-136">contato</span><span class="sxs-lookup"><span data-stu-id="48f4a-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="48f4a-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-137">Contacts.Read</span></span> | <span data-ttu-id="48f4a-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-138">Contacts.Read</span></span> | <span data-ttu-id="48f4a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-139">Contacts.Read</span></span> |
|<span data-ttu-id="48f4a-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="48f4a-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="48f4a-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-141">Not supported</span></span> | <span data-ttu-id="48f4a-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f4a-142">Files.ReadWrite</span></span> | <span data-ttu-id="48f4a-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-143">Not supported</span></span> |
|<span data-ttu-id="48f4a-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="48f4a-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="48f4a-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="48f4a-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-146">Not supported</span></span> | <span data-ttu-id="48f4a-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="48f4a-148">evento</span><span class="sxs-lookup"><span data-stu-id="48f4a-148">event</span></span>](../resources/event.md) | <span data-ttu-id="48f4a-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-149">Calendars.Read</span></span> | <span data-ttu-id="48f4a-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-150">Calendars.Read</span></span> | <span data-ttu-id="48f4a-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-151">Calendars.Read</span></span> |
|[<span data-ttu-id="48f4a-152">grupo</span><span class="sxs-lookup"><span data-stu-id="48f4a-152">group</span></span>](../resources/group.md) | <span data-ttu-id="48f4a-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-153">Group.Read.All</span></span> | <span data-ttu-id="48f4a-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-154">Not supported</span></span> | <span data-ttu-id="48f4a-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-155">Group.Read.All</span></span> |
|[<span data-ttu-id="48f4a-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="48f4a-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="48f4a-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-157">Group.Read.All</span></span> | <span data-ttu-id="48f4a-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-158">Not supported</span></span> | <span data-ttu-id="48f4a-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-159">Not supported</span></span> |
|[<span data-ttu-id="48f4a-160">list</span><span class="sxs-lookup"><span data-stu-id="48f4a-160">list</span></span>](../resources/list.md) | <span data-ttu-id="48f4a-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="48f4a-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-162">Not supported</span></span> | <span data-ttu-id="48f4a-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="48f4a-164">message</span><span class="sxs-lookup"><span data-stu-id="48f4a-164">message</span></span>](../resources/message.md) | <span data-ttu-id="48f4a-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="48f4a-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="48f4a-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48f4a-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="48f4a-168">presence</span><span class="sxs-lookup"><span data-stu-id="48f4a-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="48f4a-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-169">Presence.Read.All</span></span> | <span data-ttu-id="48f4a-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-170">Not supported</span></span> | <span data-ttu-id="48f4a-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-171">Not supported</span></span> |
|[<span data-ttu-id="48f4a-172">printer</span><span class="sxs-lookup"><span data-stu-id="48f4a-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="48f4a-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-173">Not supported</span></span> | <span data-ttu-id="48f4a-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-174">Not supported</span></span> | <span data-ttu-id="48f4a-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="48f4a-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="48f4a-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="48f4a-177">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-177">Not supported</span></span> | <span data-ttu-id="48f4a-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-178">Not supported</span></span> | <span data-ttu-id="48f4a-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="48f4a-180">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="48f4a-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="48f4a-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="48f4a-182">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-182">Not supported</span></span> | <span data-ttu-id="48f4a-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="48f4a-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="48f4a-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="48f4a-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f4a-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="48f4a-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48f4a-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="48f4a-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="48f4a-187">Not supported</span></span> |
|[<span data-ttu-id="48f4a-188">Usuário</span><span class="sxs-lookup"><span data-stu-id="48f4a-188">user</span></span>](../resources/user.md) | <span data-ttu-id="48f4a-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-189">User.Read.All</span></span> | <span data-ttu-id="48f4a-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-190">User.Read.All</span></span> | <span data-ttu-id="48f4a-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="48f4a-191">User.Read.All</span></span> |

> <span data-ttu-id="48f4a-192">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="48f4a-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="48f4a-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="48f4a-193">driveItem</span></span>

<span data-ttu-id="48f4a-194">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="48f4a-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="48f4a-195">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="48f4a-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="48f4a-196">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="48f4a-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="48f4a-197">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="48f4a-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="48f4a-198">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="48f4a-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="48f4a-199">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="48f4a-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="48f4a-200">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="48f4a-200">contact, event, and message</span></span>

<span data-ttu-id="48f4a-201">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="48f4a-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="48f4a-202">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="48f4a-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="48f4a-203">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="48f4a-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="48f4a-204">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="48f4a-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="48f4a-205">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="48f4a-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="48f4a-206">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="48f4a-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="48f4a-207">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="48f4a-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="48f4a-208">presença</span><span class="sxs-lookup"><span data-stu-id="48f4a-208">presence</span></span>

<span data-ttu-id="48f4a-209">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="48f4a-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="48f4a-210">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="48f4a-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="48f4a-211">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48f4a-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="48f4a-212">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48f4a-212">Request headers</span></span>

| <span data-ttu-id="48f4a-213">Nome</span><span class="sxs-lookup"><span data-stu-id="48f4a-213">Name</span></span>       | <span data-ttu-id="48f4a-214">Tipo</span><span class="sxs-lookup"><span data-stu-id="48f4a-214">Type</span></span> | <span data-ttu-id="48f4a-215">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f4a-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="48f4a-216">Autorização</span><span class="sxs-lookup"><span data-stu-id="48f4a-216">Authorization</span></span>  | <span data-ttu-id="48f4a-217">string</span><span class="sxs-lookup"><span data-stu-id="48f4a-217">string</span></span>  | <span data-ttu-id="48f4a-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48f4a-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="48f4a-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f4a-220">Response</span></span>

<span data-ttu-id="48f4a-221">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48f4a-221">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="48f4a-222">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="48f4a-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="48f4a-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48f4a-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="48f4a-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48f4a-224">Request</span></span>

<span data-ttu-id="48f4a-225">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="48f4a-225">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="48f4a-226">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="48f4a-226">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="48f4a-227">Essa solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário atualmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="48f4a-227">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="48f4a-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="48f4a-228">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="48f4a-229">C#</span><span class="sxs-lookup"><span data-stu-id="48f4a-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48f4a-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48f4a-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48f4a-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48f4a-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48f4a-232">Java</span><span class="sxs-lookup"><span data-stu-id="48f4a-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="48f4a-233">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="48f4a-233">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="48f4a-234">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="48f4a-234">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="48f4a-235">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="48f4a-235">Resources examples</span></span>

<span data-ttu-id="48f4a-236">Os valores a seguir são válidos para a propriedade resource.</span><span class="sxs-lookup"><span data-stu-id="48f4a-236">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="48f4a-237">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="48f4a-237">Resource type</span></span> | <span data-ttu-id="48f4a-238">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48f4a-238">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="48f4a-239">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="48f4a-239">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="48f4a-240">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="48f4a-240">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="48f4a-241">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="48f4a-241">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="48f4a-242">Contatos</span><span class="sxs-lookup"><span data-stu-id="48f4a-242">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="48f4a-243">Conversas</span><span class="sxs-lookup"><span data-stu-id="48f4a-243">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="48f4a-244">Unidades</span><span class="sxs-lookup"><span data-stu-id="48f4a-244">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="48f4a-245">Eventos</span><span class="sxs-lookup"><span data-stu-id="48f4a-245">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="48f4a-246">Grupos</span><span class="sxs-lookup"><span data-stu-id="48f4a-246">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="48f4a-247">Lista</span><span class="sxs-lookup"><span data-stu-id="48f4a-247">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="48f4a-248">Email</span><span class="sxs-lookup"><span data-stu-id="48f4a-248">Mail</span></span>](../resources/message.md)|<span data-ttu-id="48f4a-249">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="48f4a-249">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="48f4a-250">Presença</span><span class="sxs-lookup"><span data-stu-id="48f4a-250">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="48f4a-251">`/communications/presences/{id}` (usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="48f4a-251">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="48f4a-252">impressora</span><span class="sxs-lookup"><span data-stu-id="48f4a-252">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="48f4a-253">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="48f4a-253">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="48f4a-254">Usuários</span><span class="sxs-lookup"><span data-stu-id="48f4a-254">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="48f4a-255">todoTask</span><span class="sxs-lookup"><span data-stu-id="48f4a-255">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="48f4a-256">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="48f4a-256">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="48f4a-257">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="48f4a-257">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="48f4a-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f4a-258">Response</span></span>

<span data-ttu-id="48f4a-259">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="48f4a-259">The following example shows the response.</span></span> 

><span data-ttu-id="48f4a-260">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48f4a-260">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="48f4a-261">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="48f4a-261">Notification endpoint validation</span></span>

<span data-ttu-id="48f4a-262">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl)** deve ser capaz de responder a uma solicitação de validação conforme descrito em [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="48f4a-262">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="48f4a-263">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="48f4a-263">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


