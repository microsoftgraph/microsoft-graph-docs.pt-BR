---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 34a03b5e5305e62837e72559719995e2b6dae5e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013976"
---
# <a name="update-subscription"></a><span data-ttu-id="2f982-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="2f982-103">Update subscription</span></span>

<span data-ttu-id="2f982-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f982-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f982-105">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="2f982-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="2f982-106">As assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="2f982-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="2f982-107">Para evitar notificações de alteração ausentes, um aplicativo deve renovar as assinaturas bem antes da data de expiração.</span><span class="sxs-lookup"><span data-stu-id="2f982-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="2f982-108">Consulte [Subscription](../resources/subscription.md) para obter o tamanho máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="2f982-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f982-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f982-109">Permissions</span></span>

<span data-ttu-id="2f982-110">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="2f982-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2f982-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f982-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f982-112">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-112">Supported resource</span></span> | <span data-ttu-id="2f982-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f982-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2f982-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f982-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f982-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f982-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="2f982-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="2f982-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="2f982-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="2f982-117">Not supported</span></span> | <span data-ttu-id="2f982-118">Incompatível</span><span class="sxs-lookup"><span data-stu-id="2f982-118">Not supported</span></span> | <span data-ttu-id="2f982-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="2f982-120">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="2f982-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="2f982-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="2f982-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-122">Not supported</span></span> | <span data-ttu-id="2f982-123">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-123">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2f982-124">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="2f982-124">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="2f982-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-125">Not supported</span></span> | <span data-ttu-id="2f982-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-126">Not supported</span></span> | <span data-ttu-id="2f982-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2f982-128">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="2f982-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="2f982-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f982-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="2f982-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-130">Not supported</span></span> | <span data-ttu-id="2f982-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="2f982-132">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="2f982-132">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="2f982-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-133">Not supported</span></span> | <span data-ttu-id="2f982-134">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-134">Not supported</span></span> | <span data-ttu-id="2f982-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="2f982-136">contato</span><span class="sxs-lookup"><span data-stu-id="2f982-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2f982-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-137">Contacts.Read</span></span> | <span data-ttu-id="2f982-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-138">Contacts.Read</span></span> | <span data-ttu-id="2f982-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-139">Contacts.Read</span></span> |
|<span data-ttu-id="2f982-140">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="2f982-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2f982-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-141">Not supported</span></span> | <span data-ttu-id="2f982-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f982-142">Files.ReadWrite</span></span> | <span data-ttu-id="2f982-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-143">Not supported</span></span> |
|<span data-ttu-id="2f982-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="2f982-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2f982-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="2f982-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-146">Not supported</span></span> | <span data-ttu-id="2f982-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2f982-148">evento</span><span class="sxs-lookup"><span data-stu-id="2f982-148">event</span></span>](../resources/event.md) | <span data-ttu-id="2f982-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-149">Calendars.Read</span></span> | <span data-ttu-id="2f982-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-150">Calendars.Read</span></span> | <span data-ttu-id="2f982-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-151">Calendars.Read</span></span> |
|[<span data-ttu-id="2f982-152">grupo</span><span class="sxs-lookup"><span data-stu-id="2f982-152">group</span></span>](../resources/group.md) | <span data-ttu-id="2f982-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-153">Group.Read.All</span></span> | <span data-ttu-id="2f982-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-154">Not supported</span></span> | <span data-ttu-id="2f982-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-155">Group.Read.All</span></span> |
|[<span data-ttu-id="2f982-156">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="2f982-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2f982-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-157">Group.Read.All</span></span> | <span data-ttu-id="2f982-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-158">Not supported</span></span> | <span data-ttu-id="2f982-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-159">Not supported</span></span> |
|[<span data-ttu-id="2f982-160">list</span><span class="sxs-lookup"><span data-stu-id="2f982-160">list</span></span>](../resources/list.md) | <span data-ttu-id="2f982-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="2f982-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-162">Not supported</span></span> | <span data-ttu-id="2f982-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="2f982-164">message</span><span class="sxs-lookup"><span data-stu-id="2f982-164">message</span></span>](../resources/message.md) | <span data-ttu-id="2f982-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2f982-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2f982-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2f982-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2f982-168">presence</span><span class="sxs-lookup"><span data-stu-id="2f982-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="2f982-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-169">Presence.Read.All</span></span> | <span data-ttu-id="2f982-170">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-170">Not supported</span></span> | <span data-ttu-id="2f982-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-171">Not supported</span></span> |
|[<span data-ttu-id="2f982-172">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="2f982-172">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2f982-173">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-173">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2f982-174">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2f982-174">Not supported</span></span> | <span data-ttu-id="2f982-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f982-175">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2f982-176">Usuário</span><span class="sxs-lookup"><span data-stu-id="2f982-176">user</span></span>](../resources/user.md) | <span data-ttu-id="2f982-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-177">User.Read.All</span></span> | <span data-ttu-id="2f982-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-178">User.Read.All</span></span> | <span data-ttu-id="2f982-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f982-179">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="2f982-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f982-180">chatMessage</span></span>

<span data-ttu-id="2f982-181">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="2f982-181">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="2f982-182">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="2f982-182">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="2f982-183">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="2f982-183">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="2f982-184">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="2f982-184">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="2f982-185">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="2f982-185">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="2f982-186">**Observação:** `/teams/allMessages` e que `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="2f982-186">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="2f982-187">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="2f982-187">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="2f982-188">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2f982-188">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="2f982-189">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="2f982-189">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="2f982-190">driveItem</span><span class="sxs-lookup"><span data-stu-id="2f982-190">driveItem</span></span>

<span data-ttu-id="2f982-191">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2f982-191">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="2f982-192">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="2f982-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="2f982-193">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="2f982-193">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2f982-194">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="2f982-194">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2f982-195">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="2f982-195">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="2f982-196">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="2f982-196">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="2f982-197">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="2f982-197">contact, event, and message</span></span>

<span data-ttu-id="2f982-198">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2f982-198">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="2f982-199">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="2f982-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="2f982-200">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2f982-200">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2f982-201">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="2f982-201">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2f982-202">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="2f982-202">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2f982-203">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="2f982-203">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2f982-204">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="2f982-204">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="2f982-205">presença</span><span class="sxs-lookup"><span data-stu-id="2f982-205">presence</span></span>

<span data-ttu-id="2f982-206">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="2f982-206">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="2f982-207">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="2f982-207">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f982-208">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f982-208">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2f982-209">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f982-209">Request headers</span></span>

| <span data-ttu-id="2f982-210">Nome</span><span class="sxs-lookup"><span data-stu-id="2f982-210">Name</span></span>       | <span data-ttu-id="2f982-211">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f982-211">Type</span></span> | <span data-ttu-id="2f982-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f982-212">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f982-213">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f982-213">Authorization</span></span>  | <span data-ttu-id="2f982-214">string</span><span class="sxs-lookup"><span data-stu-id="2f982-214">string</span></span>  | <span data-ttu-id="2f982-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f982-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2f982-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f982-217">Response</span></span>

<span data-ttu-id="2f982-218">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f982-218">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="2f982-219">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="2f982-219">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="2f982-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f982-220">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f982-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f982-221">Request</span></span>

<span data-ttu-id="2f982-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f982-222">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f982-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f982-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2f982-224">C#</span><span class="sxs-lookup"><span data-stu-id="2f982-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f982-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f982-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f982-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f982-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f982-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f982-227">Response</span></span>

<span data-ttu-id="2f982-228">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f982-228">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
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


