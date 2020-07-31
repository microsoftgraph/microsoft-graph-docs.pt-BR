---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e0915b6a7e458f7a192b4dfc44a1eb562898ff5b
ms.sourcegitcommit: 95c1cf4f70a9322d276dc84726457eeaf98169e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2020
ms.locfileid: "46531461"
---
# <a name="get-subscription"></a><span data-ttu-id="49069-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="49069-103">Get subscription</span></span>

<span data-ttu-id="49069-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49069-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49069-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="49069-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="49069-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49069-106">Permissions</span></span>

<span data-ttu-id="49069-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="49069-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="49069-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49069-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49069-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="49069-109">Supported resource</span></span> | <span data-ttu-id="49069-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49069-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49069-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49069-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49069-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49069-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="49069-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="49069-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="49069-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-114">Not supported</span></span> | <span data-ttu-id="49069-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="49069-115">Not supported</span></span> | <span data-ttu-id="49069-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="49069-117">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="49069-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="49069-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="49069-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-119">Not supported</span></span> | <span data-ttu-id="49069-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="49069-121">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="49069-121">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="49069-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-122">Not supported</span></span> | <span data-ttu-id="49069-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-123">Not supported</span></span> | <span data-ttu-id="49069-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="49069-125">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="49069-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="49069-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49069-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="49069-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-127">Not supported</span></span> | <span data-ttu-id="49069-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="49069-129">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="49069-129">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="49069-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-130">Not supported</span></span> | <span data-ttu-id="49069-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-131">Not supported</span></span> | <span data-ttu-id="49069-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="49069-133">contato</span><span class="sxs-lookup"><span data-stu-id="49069-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="49069-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49069-134">Contacts.Read</span></span> | <span data-ttu-id="49069-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49069-135">Contacts.Read</span></span> | <span data-ttu-id="49069-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="49069-136">Contacts.Read</span></span> |
|<span data-ttu-id="49069-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="49069-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="49069-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-138">Not supported</span></span> | <span data-ttu-id="49069-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49069-139">Files.ReadWrite</span></span> | <span data-ttu-id="49069-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-140">Not supported</span></span> |
|<span data-ttu-id="49069-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="49069-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="49069-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="49069-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-143">Not supported</span></span> | <span data-ttu-id="49069-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="49069-145">evento</span><span class="sxs-lookup"><span data-stu-id="49069-145">event</span></span>](../resources/event.md) | <span data-ttu-id="49069-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49069-146">Calendars.Read</span></span> | <span data-ttu-id="49069-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49069-147">Calendars.Read</span></span> | <span data-ttu-id="49069-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="49069-148">Calendars.Read</span></span> |
|[<span data-ttu-id="49069-149">grupo</span><span class="sxs-lookup"><span data-stu-id="49069-149">group</span></span>](../resources/group.md) | <span data-ttu-id="49069-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-150">Group.Read.All</span></span> | <span data-ttu-id="49069-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-151">Not supported</span></span> | <span data-ttu-id="49069-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-152">Group.Read.All</span></span> |
|[<span data-ttu-id="49069-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="49069-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="49069-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-154">Group.Read.All</span></span> | <span data-ttu-id="49069-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-155">Not supported</span></span> | <span data-ttu-id="49069-156">Incompatível</span><span class="sxs-lookup"><span data-stu-id="49069-156">Not supported</span></span> |
|[<span data-ttu-id="49069-157">list</span><span class="sxs-lookup"><span data-stu-id="49069-157">list</span></span>](../resources/list.md) | <span data-ttu-id="49069-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="49069-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-159">Not supported</span></span> | <span data-ttu-id="49069-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="49069-161">message</span><span class="sxs-lookup"><span data-stu-id="49069-161">message</span></span>](../resources/message.md) | <span data-ttu-id="49069-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49069-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="49069-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49069-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="49069-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="49069-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="49069-165">presence</span><span class="sxs-lookup"><span data-stu-id="49069-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="49069-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-166">Presence.Read.All</span></span> | <span data-ttu-id="49069-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-167">Not supported</span></span> | <span data-ttu-id="49069-168">Incompatível</span><span class="sxs-lookup"><span data-stu-id="49069-168">Not supported</span></span> |
|[<span data-ttu-id="49069-169">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="49069-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="49069-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="49069-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="49069-171">Not supported</span></span> | <span data-ttu-id="49069-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49069-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="49069-173">Usuário</span><span class="sxs-lookup"><span data-stu-id="49069-173">user</span></span>](../resources/user.md) | <span data-ttu-id="49069-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-174">User.Read.All</span></span> | <span data-ttu-id="49069-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-175">User.Read.All</span></span> | <span data-ttu-id="49069-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="49069-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="49069-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="49069-177">chatMessage</span></span>

<span data-ttu-id="49069-178">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="49069-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="49069-179">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="49069-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="49069-180">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="49069-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="49069-181">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="49069-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="49069-182">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="49069-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="49069-183">**Observação:** `/teams/allMessages` e que `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="49069-183">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="49069-184">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="49069-184">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="49069-185">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="49069-185">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="49069-186">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="49069-186">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="49069-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="49069-187">driveItem</span></span>

<span data-ttu-id="49069-188">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="49069-188">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="49069-189">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="49069-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="49069-190">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="49069-190">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="49069-191">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="49069-191">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="49069-192">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="49069-192">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="49069-193">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="49069-193">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="49069-194">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="49069-194">contact, event, and message</span></span>

<span data-ttu-id="49069-195">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="49069-195">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="49069-196">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="49069-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="49069-197">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="49069-197">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="49069-198">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="49069-198">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="49069-199">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="49069-199">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="49069-200">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="49069-200">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="49069-201">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="49069-201">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="49069-202">presença</span><span class="sxs-lookup"><span data-stu-id="49069-202">presence</span></span>

<span data-ttu-id="49069-203">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="49069-203">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="49069-204">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="49069-204">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="49069-205">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49069-205">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49069-206">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49069-206">Optional query parameters</span></span>

<span data-ttu-id="49069-207">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="49069-207">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49069-208">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49069-208">Request headers</span></span>

| <span data-ttu-id="49069-209">Nome</span><span class="sxs-lookup"><span data-stu-id="49069-209">Name</span></span>       | <span data-ttu-id="49069-210">Tipo</span><span class="sxs-lookup"><span data-stu-id="49069-210">Type</span></span> | <span data-ttu-id="49069-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="49069-211">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="49069-212">Autorização</span><span class="sxs-lookup"><span data-stu-id="49069-212">Authorization</span></span>  | <span data-ttu-id="49069-213">string</span><span class="sxs-lookup"><span data-stu-id="49069-213">string</span></span>  | <span data-ttu-id="49069-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49069-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49069-216">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49069-216">Request body</span></span>

<span data-ttu-id="49069-217">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49069-217">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49069-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="49069-218">Response</span></span>

<span data-ttu-id="49069-219">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49069-219">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49069-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49069-220">Example</span></span>

##### <a name="request"></a><span data-ttu-id="49069-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49069-221">Request</span></span>

<span data-ttu-id="49069-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49069-222">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49069-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="49069-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="49069-224">C#</span><span class="sxs-lookup"><span data-stu-id="49069-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49069-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49069-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49069-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49069-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49069-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="49069-227">Response</span></span>

<span data-ttu-id="49069-228">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49069-228">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2"
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
