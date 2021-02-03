---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 058d4e918b629d0ff1572dffb2a38228de56afdf
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092726"
---
# <a name="get-subscription"></a><span data-ttu-id="3f622-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="3f622-103">Get subscription</span></span>

<span data-ttu-id="3f622-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f622-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f622-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3f622-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="3f622-106">Consulte a tabela na [seção Permissões para](#permissions) ver a lista de recursos que suportam a assinatura para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="3f622-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f622-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f622-107">Permissions</span></span>

<span data-ttu-id="3f622-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="3f622-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3f622-109">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher permissões mais privilegiadas, procure as seguintes permissões em [Permissões.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="3f622-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f622-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-110">Supported resource</span></span> | <span data-ttu-id="3f622-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f622-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f622-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f622-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f622-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f622-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="3f622-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="3f622-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="3f622-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="3f622-115">Not supported</span></span> | <span data-ttu-id="3f622-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="3f622-116">Not supported</span></span> | <span data-ttu-id="3f622-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="3f622-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="3f622-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="3f622-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="3f622-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-120">Not supported</span></span> | <span data-ttu-id="3f622-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="3f622-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="3f622-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="3f622-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-123">Not supported</span></span> | <span data-ttu-id="3f622-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-124">Not supported</span></span> | <span data-ttu-id="3f622-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="3f622-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="3f622-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="3f622-127">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f622-127">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="3f622-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-128">Not supported</span></span> | <span data-ttu-id="3f622-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="3f622-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="3f622-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="3f622-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-131">Not supported</span></span> | <span data-ttu-id="3f622-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-132">Not supported</span></span> | <span data-ttu-id="3f622-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="3f622-134">contato</span><span class="sxs-lookup"><span data-stu-id="3f622-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="3f622-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-135">Contacts.Read</span></span> | <span data-ttu-id="3f622-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-136">Contacts.Read</span></span> | <span data-ttu-id="3f622-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-137">Contacts.Read</span></span> |
|<span data-ttu-id="3f622-138">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="3f622-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="3f622-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-139">Not supported</span></span> | <span data-ttu-id="3f622-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f622-140">Files.ReadWrite</span></span> | <span data-ttu-id="3f622-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-141">Not supported</span></span> |
|<span data-ttu-id="3f622-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="3f622-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="3f622-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="3f622-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-144">Not supported</span></span> | <span data-ttu-id="3f622-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="3f622-146">evento</span><span class="sxs-lookup"><span data-stu-id="3f622-146">event</span></span>](../resources/event.md) | <span data-ttu-id="3f622-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-147">Calendars.Read</span></span> | <span data-ttu-id="3f622-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-148">Calendars.Read</span></span> | <span data-ttu-id="3f622-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-149">Calendars.Read</span></span> |
|[<span data-ttu-id="3f622-150">grupo</span><span class="sxs-lookup"><span data-stu-id="3f622-150">group</span></span>](../resources/group.md) | <span data-ttu-id="3f622-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-151">Group.Read.All</span></span> | <span data-ttu-id="3f622-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-152">Not supported</span></span> | <span data-ttu-id="3f622-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-153">Group.Read.All</span></span> |
|[<span data-ttu-id="3f622-154">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="3f622-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="3f622-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-155">Group.Read.All</span></span> | <span data-ttu-id="3f622-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-156">Not supported</span></span> | <span data-ttu-id="3f622-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-157">Not supported</span></span> |
|[<span data-ttu-id="3f622-158">list</span><span class="sxs-lookup"><span data-stu-id="3f622-158">list</span></span>](../resources/list.md) | <span data-ttu-id="3f622-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="3f622-160">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-160">Not supported</span></span> | <span data-ttu-id="3f622-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="3f622-162">message</span><span class="sxs-lookup"><span data-stu-id="3f622-162">message</span></span>](../resources/message.md) | <span data-ttu-id="3f622-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="3f622-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="3f622-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3f622-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="3f622-166">presence</span><span class="sxs-lookup"><span data-stu-id="3f622-166">presence</span></span>](../resources/presence.md) | <span data-ttu-id="3f622-167">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-167">Presence.Read.All</span></span> | <span data-ttu-id="3f622-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-168">Not supported</span></span> | <span data-ttu-id="3f622-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-169">Not supported</span></span> |
|[<span data-ttu-id="3f622-170">impressora</span><span class="sxs-lookup"><span data-stu-id="3f622-170">printer</span></span>](../resources/printer.md) | <span data-ttu-id="3f622-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-171">Not supported</span></span> | <span data-ttu-id="3f622-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-172">Not supported</span></span> | <span data-ttu-id="3f622-173">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-173">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="3f622-174">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="3f622-174">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="3f622-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-175">Not supported</span></span> | <span data-ttu-id="3f622-176">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-176">Not supported</span></span> | <span data-ttu-id="3f622-177">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-177">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="3f622-178">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="3f622-178">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="3f622-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-179">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="3f622-180">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-180">Not supported</span></span> | <span data-ttu-id="3f622-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f622-181">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="3f622-182">todoTask</span><span class="sxs-lookup"><span data-stu-id="3f622-182">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="3f622-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f622-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="3f622-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f622-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="3f622-185">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3f622-185">Not supported</span></span> |
|[<span data-ttu-id="3f622-186">Usuário</span><span class="sxs-lookup"><span data-stu-id="3f622-186">user</span></span>](../resources/user.md) | <span data-ttu-id="3f622-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-187">User.Read.All</span></span> | <span data-ttu-id="3f622-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-188">User.Read.All</span></span> | <span data-ttu-id="3f622-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f622-189">User.Read.All</span></span> |

> <span data-ttu-id="3f622-190">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3f622-190">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="3f622-191">driveItem</span><span class="sxs-lookup"><span data-stu-id="3f622-191">driveItem</span></span>

<span data-ttu-id="3f622-192">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3f622-192">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="3f622-193">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="3f622-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="3f622-194">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="3f622-194">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="3f622-195">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="3f622-195">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="3f622-196">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="3f622-196">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="3f622-197">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="3f622-197">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="3f622-198">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="3f622-198">contact, event, and message</span></span>

<span data-ttu-id="3f622-199">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="3f622-199">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="3f622-200">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="3f622-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="3f622-201">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3f622-201">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="3f622-202">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="3f622-202">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="3f622-203">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="3f622-203">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="3f622-204">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="3f622-204">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="3f622-205">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="3f622-205">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="3f622-206">presença</span><span class="sxs-lookup"><span data-stu-id="3f622-206">presence</span></span>

<span data-ttu-id="3f622-207">**assinaturas** de presença [exigem criptografia.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="3f622-207">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="3f622-208">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="3f622-208">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="3f622-209">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f622-209">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3f622-210">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f622-210">Optional query parameters</span></span>

<span data-ttu-id="3f622-211">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f622-211">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f622-212">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f622-212">Request headers</span></span>

| <span data-ttu-id="3f622-213">Nome</span><span class="sxs-lookup"><span data-stu-id="3f622-213">Name</span></span>       | <span data-ttu-id="3f622-214">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f622-214">Type</span></span> | <span data-ttu-id="3f622-215">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f622-215">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="3f622-216">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f622-216">Authorization</span></span>  | <span data-ttu-id="3f622-217">string</span><span class="sxs-lookup"><span data-stu-id="3f622-217">string</span></span>  | <span data-ttu-id="3f622-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f622-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f622-220">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f622-220">Request body</span></span>

<span data-ttu-id="3f622-221">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f622-221">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f622-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f622-222">Response</span></span>

<span data-ttu-id="3f622-223">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f622-223">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f622-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f622-224">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3f622-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f622-225">Request</span></span>

<span data-ttu-id="3f622-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f622-226">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f622-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f622-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="3f622-228">C#</span><span class="sxs-lookup"><span data-stu-id="3f622-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f622-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f622-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f622-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f622-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f622-231">Java</span><span class="sxs-lookup"><span data-stu-id="3f622-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f622-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f622-232">Response</span></span>

<span data-ttu-id="3f622-233">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f622-233">Here is an example of the response.</span></span>
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


