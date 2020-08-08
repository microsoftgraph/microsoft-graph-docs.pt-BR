---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 703af25923636ba8c47d7820971e0b464e12324a
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598203"
---
# <a name="delete-subscription"></a><span data-ttu-id="55cc9-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="55cc9-103">Delete subscription</span></span>

<span data-ttu-id="55cc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55cc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55cc9-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="55cc9-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="55cc9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55cc9-106">Permissions</span></span>

<span data-ttu-id="55cc9-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="55cc9-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="55cc9-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55cc9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55cc9-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-109">Supported resource</span></span> | <span data-ttu-id="55cc9-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55cc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55cc9-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55cc9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55cc9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55cc9-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="55cc9-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="55cc9-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="55cc9-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-114">Not supported</span></span> | <span data-ttu-id="55cc9-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="55cc9-115">Not supported</span></span> | <span data-ttu-id="55cc9-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="55cc9-117">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="55cc9-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="55cc9-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="55cc9-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-119">Not supported</span></span> | <span data-ttu-id="55cc9-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="55cc9-121">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="55cc9-121">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="55cc9-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-122">Not supported</span></span> | <span data-ttu-id="55cc9-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-123">Not supported</span></span> | <span data-ttu-id="55cc9-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="55cc9-125">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="55cc9-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="55cc9-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55cc9-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="55cc9-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-127">Not supported</span></span> | <span data-ttu-id="55cc9-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="55cc9-129">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="55cc9-129">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="55cc9-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-130">Not supported</span></span> | <span data-ttu-id="55cc9-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-131">Not supported</span></span> | <span data-ttu-id="55cc9-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="55cc9-133">contato</span><span class="sxs-lookup"><span data-stu-id="55cc9-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="55cc9-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-134">Contacts.Read</span></span> | <span data-ttu-id="55cc9-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-135">Contacts.Read</span></span> | <span data-ttu-id="55cc9-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-136">Contacts.Read</span></span> |
|<span data-ttu-id="55cc9-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="55cc9-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="55cc9-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-138">Not supported</span></span> | <span data-ttu-id="55cc9-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55cc9-139">Files.ReadWrite</span></span> | <span data-ttu-id="55cc9-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-140">Not supported</span></span> |
|<span data-ttu-id="55cc9-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="55cc9-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="55cc9-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="55cc9-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-143">Not supported</span></span> | <span data-ttu-id="55cc9-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="55cc9-145">evento</span><span class="sxs-lookup"><span data-stu-id="55cc9-145">event</span></span>](../resources/event.md) | <span data-ttu-id="55cc9-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-146">Calendars.Read</span></span> | <span data-ttu-id="55cc9-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-147">Calendars.Read</span></span> | <span data-ttu-id="55cc9-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-148">Calendars.Read</span></span> |
|[<span data-ttu-id="55cc9-149">grupo</span><span class="sxs-lookup"><span data-stu-id="55cc9-149">group</span></span>](../resources/group.md) | <span data-ttu-id="55cc9-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-150">Group.Read.All</span></span> | <span data-ttu-id="55cc9-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-151">Not supported</span></span> | <span data-ttu-id="55cc9-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-152">Group.Read.All</span></span> |
|[<span data-ttu-id="55cc9-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="55cc9-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="55cc9-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-154">Group.Read.All</span></span> | <span data-ttu-id="55cc9-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-155">Not supported</span></span> | <span data-ttu-id="55cc9-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-156">Not supported</span></span> |
|[<span data-ttu-id="55cc9-157">list</span><span class="sxs-lookup"><span data-stu-id="55cc9-157">list</span></span>](../resources/list.md) | <span data-ttu-id="55cc9-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="55cc9-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-159">Not supported</span></span> | <span data-ttu-id="55cc9-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="55cc9-161">message</span><span class="sxs-lookup"><span data-stu-id="55cc9-161">message</span></span>](../resources/message.md) | <span data-ttu-id="55cc9-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="55cc9-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="55cc9-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="55cc9-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="55cc9-165">presence</span><span class="sxs-lookup"><span data-stu-id="55cc9-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="55cc9-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-166">Presence.Read.All</span></span> | <span data-ttu-id="55cc9-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-167">Not supported</span></span> | <span data-ttu-id="55cc9-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-168">Not supported</span></span> |
|[<span data-ttu-id="55cc9-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="55cc9-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="55cc9-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="55cc9-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="55cc9-171">Not supported</span></span> | <span data-ttu-id="55cc9-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="55cc9-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="55cc9-173">user</span></span>](../resources/user.md) | <span data-ttu-id="55cc9-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-174">User.Read.All</span></span> | <span data-ttu-id="55cc9-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-175">User.Read.All</span></span> | <span data-ttu-id="55cc9-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cc9-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="55cc9-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55cc9-177">chatMessage</span></span>

<span data-ttu-id="55cc9-178">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="55cc9-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="55cc9-179">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="55cc9-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="55cc9-180">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="55cc9-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="55cc9-181">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="55cc9-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="55cc9-182">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="55cc9-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="55cc9-183">**Observação:** `/teams/allMessages` e que `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="55cc9-183">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="55cc9-184">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="55cc9-184">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="55cc9-185">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55cc9-185">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="55cc9-186">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="55cc9-186">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="55cc9-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="55cc9-187">driveItem</span></span>

<span data-ttu-id="55cc9-188">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="55cc9-188">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="55cc9-189">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="55cc9-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="55cc9-190">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="55cc9-190">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="55cc9-191">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="55cc9-191">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="55cc9-192">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="55cc9-192">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="55cc9-193">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="55cc9-193">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="55cc9-194">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="55cc9-194">contact, event, and message</span></span>

<span data-ttu-id="55cc9-195">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55cc9-195">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="55cc9-196">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="55cc9-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="55cc9-197">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="55cc9-197">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="55cc9-198">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="55cc9-198">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="55cc9-199">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="55cc9-199">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="55cc9-200">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="55cc9-200">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="55cc9-201">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="55cc9-201">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="55cc9-202">presença</span><span class="sxs-lookup"><span data-stu-id="55cc9-202">presence</span></span>

<span data-ttu-id="55cc9-203">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="55cc9-203">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="55cc9-204">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="55cc9-204">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="55cc9-205">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55cc9-205">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55cc9-206">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55cc9-206">Request headers</span></span>

| <span data-ttu-id="55cc9-207">Nome</span><span class="sxs-lookup"><span data-stu-id="55cc9-207">Name</span></span>       | <span data-ttu-id="55cc9-208">Tipo</span><span class="sxs-lookup"><span data-stu-id="55cc9-208">Type</span></span> | <span data-ttu-id="55cc9-209">Descrição</span><span class="sxs-lookup"><span data-stu-id="55cc9-209">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="55cc9-210">Autorização</span><span class="sxs-lookup"><span data-stu-id="55cc9-210">Authorization</span></span>  | <span data-ttu-id="55cc9-211">string</span><span class="sxs-lookup"><span data-stu-id="55cc9-211">string</span></span>  | <span data-ttu-id="55cc9-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55cc9-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55cc9-214">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55cc9-214">Request body</span></span>

<span data-ttu-id="55cc9-215">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55cc9-215">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55cc9-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="55cc9-216">Response</span></span>

<span data-ttu-id="55cc9-217">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="55cc9-217">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="55cc9-218">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="55cc9-218">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="55cc9-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55cc9-219">Example</span></span>

##### <a name="request"></a><span data-ttu-id="55cc9-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55cc9-220">Request</span></span>

<span data-ttu-id="55cc9-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55cc9-221">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55cc9-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="55cc9-222">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="55cc9-223">C#</span><span class="sxs-lookup"><span data-stu-id="55cc9-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55cc9-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55cc9-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55cc9-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55cc9-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55cc9-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="55cc9-226">Response</span></span>

<span data-ttu-id="55cc9-227">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55cc9-227">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
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
