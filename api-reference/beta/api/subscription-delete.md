---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 4cc38673566bdff9114e0f94e0a8e27c3d9ad2eb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787573"
---
# <a name="delete-subscription"></a><span data-ttu-id="422f4-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="422f4-103">Delete subscription</span></span>

<span data-ttu-id="422f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="422f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="422f4-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="422f4-105">Delete a subscription.</span></span>

<span data-ttu-id="422f4-106">Consulte a tabela na seção [Permissões](#permissions) para obter a lista de recursos que oferecem suporte à inscrição para alterar notificações.</span><span class="sxs-lookup"><span data-stu-id="422f4-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="422f4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="422f4-107">Permissions</span></span>

<span data-ttu-id="422f4-108">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="422f4-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="422f4-109">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="422f4-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="422f4-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-110">Supported resource</span></span> | <span data-ttu-id="422f4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="422f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="422f4-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="422f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="422f4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="422f4-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="422f4-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="422f4-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="422f4-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="422f4-115">Not supported</span></span> | <span data-ttu-id="422f4-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="422f4-116">Not supported</span></span> | <span data-ttu-id="422f4-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="422f4-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="422f4-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="422f4-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="422f4-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-120">Not supported</span></span> | <span data-ttu-id="422f4-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="422f4-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="422f4-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="422f4-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-123">Not supported</span></span> | <span data-ttu-id="422f4-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-124">Not supported</span></span> | <span data-ttu-id="422f4-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="422f4-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="422f4-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="422f4-127">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="422f4-127">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="422f4-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-128">Not supported</span></span> | <span data-ttu-id="422f4-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="422f4-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="422f4-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="422f4-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-131">Not supported</span></span> | <span data-ttu-id="422f4-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-132">Not supported</span></span> | <span data-ttu-id="422f4-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="422f4-134">contato</span><span class="sxs-lookup"><span data-stu-id="422f4-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="422f4-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-135">Contacts.Read</span></span> | <span data-ttu-id="422f4-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-136">Contacts.Read</span></span> | <span data-ttu-id="422f4-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-137">Contacts.Read</span></span> |
|<span data-ttu-id="422f4-138">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="422f4-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="422f4-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-139">Not supported</span></span> | <span data-ttu-id="422f4-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="422f4-140">Files.ReadWrite</span></span> | <span data-ttu-id="422f4-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-141">Not supported</span></span> |
|<span data-ttu-id="422f4-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="422f4-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="422f4-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="422f4-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-144">Not supported</span></span> | <span data-ttu-id="422f4-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="422f4-146">evento</span><span class="sxs-lookup"><span data-stu-id="422f4-146">event</span></span>](../resources/event.md) | <span data-ttu-id="422f4-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-147">Calendars.Read</span></span> | <span data-ttu-id="422f4-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-148">Calendars.Read</span></span> | <span data-ttu-id="422f4-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-149">Calendars.Read</span></span> |
|[<span data-ttu-id="422f4-150">grupo</span><span class="sxs-lookup"><span data-stu-id="422f4-150">group</span></span>](../resources/group.md) | <span data-ttu-id="422f4-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-151">Group.Read.All</span></span> | <span data-ttu-id="422f4-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-152">Not supported</span></span> | <span data-ttu-id="422f4-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-153">Group.Read.All</span></span> |
|[<span data-ttu-id="422f4-154">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="422f4-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="422f4-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-155">Group.Read.All</span></span> | <span data-ttu-id="422f4-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-156">Not supported</span></span> | <span data-ttu-id="422f4-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-157">Not supported</span></span> |
|[<span data-ttu-id="422f4-158">list</span><span class="sxs-lookup"><span data-stu-id="422f4-158">list</span></span>](../resources/list.md) | <span data-ttu-id="422f4-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="422f4-160">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-160">Not supported</span></span> | <span data-ttu-id="422f4-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="422f4-162">message</span><span class="sxs-lookup"><span data-stu-id="422f4-162">message</span></span>](../resources/message.md) | <span data-ttu-id="422f4-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="422f4-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="422f4-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="422f4-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="422f4-166">presence</span><span class="sxs-lookup"><span data-stu-id="422f4-166">presence</span></span>](../resources/presence.md) | <span data-ttu-id="422f4-167">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-167">Presence.Read.All</span></span> | <span data-ttu-id="422f4-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-168">Not supported</span></span> | <span data-ttu-id="422f4-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-169">Not supported</span></span> |
|[<span data-ttu-id="422f4-170">printer</span><span class="sxs-lookup"><span data-stu-id="422f4-170">printer</span></span>](../resources/printer.md) | <span data-ttu-id="422f4-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-171">Not supported</span></span> | <span data-ttu-id="422f4-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-172">Not supported</span></span> | <span data-ttu-id="422f4-173">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-173">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="422f4-174">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="422f4-174">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="422f4-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-175">Not supported</span></span> | <span data-ttu-id="422f4-176">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-176">Not supported</span></span> | <span data-ttu-id="422f4-177">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-177">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="422f4-178">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="422f4-178">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="422f4-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-179">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="422f4-180">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-180">Not supported</span></span> | <span data-ttu-id="422f4-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422f4-181">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="422f4-182">todoTask</span><span class="sxs-lookup"><span data-stu-id="422f4-182">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="422f4-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="422f4-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="422f4-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="422f4-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="422f4-185">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="422f4-185">Not supported</span></span> |
|[<span data-ttu-id="422f4-186">Usuário</span><span class="sxs-lookup"><span data-stu-id="422f4-186">user</span></span>](../resources/user.md) | <span data-ttu-id="422f4-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-187">User.Read.All</span></span> | <span data-ttu-id="422f4-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-188">User.Read.All</span></span> | <span data-ttu-id="422f4-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="422f4-189">User.Read.All</span></span> |

> <span data-ttu-id="422f4-190">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="422f4-190">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="422f4-191">driveItem</span><span class="sxs-lookup"><span data-stu-id="422f4-191">driveItem</span></span>

<span data-ttu-id="422f4-192">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="422f4-192">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="422f4-193">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="422f4-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="422f4-194">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="422f4-194">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="422f4-195">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="422f4-195">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="422f4-196">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="422f4-196">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="422f4-197">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="422f4-197">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="422f4-198">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="422f4-198">contact, event, and message</span></span>

<span data-ttu-id="422f4-199">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="422f4-199">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="422f4-200">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="422f4-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="422f4-201">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="422f4-201">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="422f4-202">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="422f4-202">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="422f4-203">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="422f4-203">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="422f4-204">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="422f4-204">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="422f4-205">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="422f4-205">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="422f4-206">presença</span><span class="sxs-lookup"><span data-stu-id="422f4-206">presence</span></span>

<span data-ttu-id="422f4-207">**assinaturas** de presença exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="422f4-207">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="422f4-208">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="422f4-208">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="422f4-209">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="422f4-209">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="422f4-210">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="422f4-210">Request headers</span></span>

| <span data-ttu-id="422f4-211">Nome</span><span class="sxs-lookup"><span data-stu-id="422f4-211">Name</span></span>       | <span data-ttu-id="422f4-212">Tipo</span><span class="sxs-lookup"><span data-stu-id="422f4-212">Type</span></span> | <span data-ttu-id="422f4-213">Descrição</span><span class="sxs-lookup"><span data-stu-id="422f4-213">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="422f4-214">Autorização</span><span class="sxs-lookup"><span data-stu-id="422f4-214">Authorization</span></span>  | <span data-ttu-id="422f4-215">string</span><span class="sxs-lookup"><span data-stu-id="422f4-215">string</span></span>  | <span data-ttu-id="422f4-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="422f4-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="422f4-218">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="422f4-218">Request body</span></span>

<span data-ttu-id="422f4-219">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="422f4-219">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="422f4-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="422f4-220">Response</span></span>

<span data-ttu-id="422f4-221">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="422f4-221">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="422f4-222">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="422f4-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="422f4-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="422f4-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="422f4-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="422f4-224">Request</span></span>

<span data-ttu-id="422f4-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="422f4-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="422f4-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="422f4-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="422f4-227">C#</span><span class="sxs-lookup"><span data-stu-id="422f4-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="422f4-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="422f4-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="422f4-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="422f4-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="422f4-230">Java</span><span class="sxs-lookup"><span data-stu-id="422f4-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="422f4-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="422f4-231">Response</span></span>

<span data-ttu-id="422f4-232">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="422f4-232">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


