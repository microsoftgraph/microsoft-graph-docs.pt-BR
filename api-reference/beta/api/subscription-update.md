---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: ae66d6267914b25a101a84b96ed339dc68d8f867
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934700"
---
# <a name="update-subscription"></a><span data-ttu-id="f411e-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="f411e-103">Update subscription</span></span>

<span data-ttu-id="f411e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f411e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f411e-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="f411e-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="f411e-106">As assinaturas expiram após um período que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="f411e-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="f411e-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar suas assinaturas bem antes da data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="f411e-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="f411e-108">Consulte [a assinatura](../resources/subscription.md) para a duração máxima de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="f411e-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="f411e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f411e-109">Permissions</span></span>

<span data-ttu-id="f411e-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="f411e-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f411e-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f411e-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f411e-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-112">Supported resource</span></span> | <span data-ttu-id="f411e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f411e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f411e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f411e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f411e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f411e-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="f411e-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="f411e-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="f411e-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f411e-117">Not supported</span></span> | <span data-ttu-id="f411e-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f411e-118">Not supported</span></span> | <span data-ttu-id="f411e-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="f411e-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="f411e-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="f411e-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="f411e-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-122">Not supported</span></span> | <span data-ttu-id="f411e-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="f411e-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="f411e-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="f411e-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-125">Not supported</span></span> | <span data-ttu-id="f411e-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-126">Not supported</span></span> | <span data-ttu-id="f411e-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="f411e-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="f411e-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="f411e-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f411e-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="f411e-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-130">Not supported</span></span> | <span data-ttu-id="f411e-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="f411e-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="f411e-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="f411e-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-133">Not supported</span></span> | <span data-ttu-id="f411e-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-134">Not supported</span></span> | <span data-ttu-id="f411e-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="f411e-136">contato</span><span class="sxs-lookup"><span data-stu-id="f411e-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f411e-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-137">Contacts.Read</span></span> | <span data-ttu-id="f411e-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-138">Contacts.Read</span></span> | <span data-ttu-id="f411e-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-139">Contacts.Read</span></span> |
|<span data-ttu-id="f411e-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="f411e-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="f411e-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-141">Not supported</span></span> | <span data-ttu-id="f411e-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f411e-142">Files.ReadWrite</span></span> | <span data-ttu-id="f411e-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-143">Not supported</span></span> |
|<span data-ttu-id="f411e-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="f411e-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="f411e-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="f411e-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-146">Not supported</span></span> | <span data-ttu-id="f411e-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="f411e-148">evento</span><span class="sxs-lookup"><span data-stu-id="f411e-148">event</span></span>](../resources/event.md) | <span data-ttu-id="f411e-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-149">Calendars.Read</span></span> | <span data-ttu-id="f411e-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-150">Calendars.Read</span></span> | <span data-ttu-id="f411e-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-151">Calendars.Read</span></span> |
|[<span data-ttu-id="f411e-152">grupo</span><span class="sxs-lookup"><span data-stu-id="f411e-152">group</span></span>](../resources/group.md) | <span data-ttu-id="f411e-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-153">Group.Read.All</span></span> | <span data-ttu-id="f411e-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-154">Not supported</span></span> | <span data-ttu-id="f411e-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-155">Group.Read.All</span></span> |
|[<span data-ttu-id="f411e-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="f411e-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="f411e-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-157">Group.Read.All</span></span> | <span data-ttu-id="f411e-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-158">Not supported</span></span> | <span data-ttu-id="f411e-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-159">Not supported</span></span> |
|[<span data-ttu-id="f411e-160">list</span><span class="sxs-lookup"><span data-stu-id="f411e-160">list</span></span>](../resources/list.md) | <span data-ttu-id="f411e-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="f411e-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-162">Not supported</span></span> | <span data-ttu-id="f411e-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="f411e-164">message</span><span class="sxs-lookup"><span data-stu-id="f411e-164">message</span></span>](../resources/message.md) | <span data-ttu-id="f411e-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="f411e-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="f411e-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f411e-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="f411e-168">presence</span><span class="sxs-lookup"><span data-stu-id="f411e-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="f411e-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-169">Presence.Read.All</span></span> | <span data-ttu-id="f411e-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-170">Not supported</span></span> | <span data-ttu-id="f411e-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-171">Not supported</span></span> |
|[<span data-ttu-id="f411e-172">impressora</span><span class="sxs-lookup"><span data-stu-id="f411e-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="f411e-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-173">Not supported</span></span> | <span data-ttu-id="f411e-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-174">Not supported</span></span> | <span data-ttu-id="f411e-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="f411e-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="f411e-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="f411e-177">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-177">Not supported</span></span> | <span data-ttu-id="f411e-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-178">Not supported</span></span> | <span data-ttu-id="f411e-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="f411e-180">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="f411e-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="f411e-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="f411e-182">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-182">Not supported</span></span> | <span data-ttu-id="f411e-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f411e-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="f411e-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="f411e-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="f411e-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f411e-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="f411e-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f411e-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="f411e-187">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f411e-187">Not supported</span></span> |
|[<span data-ttu-id="f411e-188">Usuário</span><span class="sxs-lookup"><span data-stu-id="f411e-188">user</span></span>](../resources/user.md) | <span data-ttu-id="f411e-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-189">User.Read.All</span></span> | <span data-ttu-id="f411e-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-190">User.Read.All</span></span> | <span data-ttu-id="f411e-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f411e-191">User.Read.All</span></span> |

> <span data-ttu-id="f411e-192">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f411e-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="f411e-193">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f411e-193">chatMessage</span></span>

<span data-ttu-id="f411e-194">**Assinaturas chatMessage** com permissões delegadas não suportam dados de recurso (**includeResourceData** deve ser ), e `false` não [exigem criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f411e-194">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="f411e-195">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f411e-195">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f411e-196">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="f411e-196">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="f411e-197">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="f411e-197">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="f411e-198">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="f411e-198">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="f411e-199">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="f411e-199">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="f411e-200">No futuro, a Microsoft poderá exigir que você ou seus clientes pagarão taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="f411e-200">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="f411e-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="f411e-201">driveItem</span></span>

<span data-ttu-id="f411e-202">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f411e-202">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="f411e-203">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="f411e-203">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="f411e-204">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="f411e-204">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="f411e-205">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="f411e-205">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="f411e-206">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="f411e-206">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="f411e-207">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="f411e-207">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="f411e-208">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="f411e-208">contact, event, and message</span></span>

<span data-ttu-id="f411e-209">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f411e-209">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="f411e-210">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="f411e-210">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="f411e-211">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f411e-211">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="f411e-212">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="f411e-212">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="f411e-213">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="f411e-213">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="f411e-214">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="f411e-214">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="f411e-215">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="f411e-215">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="f411e-216">presença</span><span class="sxs-lookup"><span data-stu-id="f411e-216">presence</span></span>

<span data-ttu-id="f411e-217">**assinaturas** de presença [exigem criptografia.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="f411e-217">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f411e-218">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="f411e-218">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="f411e-219">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f411e-219">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f411e-220">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f411e-220">Request headers</span></span>

| <span data-ttu-id="f411e-221">Nome</span><span class="sxs-lookup"><span data-stu-id="f411e-221">Name</span></span>       | <span data-ttu-id="f411e-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="f411e-222">Type</span></span> | <span data-ttu-id="f411e-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="f411e-223">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f411e-224">Autorização</span><span class="sxs-lookup"><span data-stu-id="f411e-224">Authorization</span></span>  | <span data-ttu-id="f411e-225">string</span><span class="sxs-lookup"><span data-stu-id="f411e-225">string</span></span>  | <span data-ttu-id="f411e-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f411e-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f411e-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="f411e-228">Response</span></span>

<span data-ttu-id="f411e-229">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f411e-229">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="f411e-230">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="f411e-230">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="f411e-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f411e-231">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f411e-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f411e-232">Request</span></span>

<span data-ttu-id="f411e-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f411e-233">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f411e-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="f411e-234">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f411e-235">C#</span><span class="sxs-lookup"><span data-stu-id="f411e-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f411e-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f411e-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f411e-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f411e-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f411e-238">Java</span><span class="sxs-lookup"><span data-stu-id="f411e-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f411e-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="f411e-239">Response</span></span>

<span data-ttu-id="f411e-240">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f411e-240">Here is an example of the response.</span></span>
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


