---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 10e764bef772b6874f811048b9ec5cdc101f1807
ms.sourcegitcommit: 95c1cf4f70a9322d276dc84726457eeaf98169e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2020
ms.locfileid: "46531457"
---
# <a name="create-subscription"></a><span data-ttu-id="87184-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="87184-103">Create subscription</span></span>

<span data-ttu-id="87184-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87184-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87184-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="87184-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="87184-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87184-106">Permissions</span></span>

<span data-ttu-id="87184-107">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="87184-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="87184-108">Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="87184-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="87184-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="87184-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="87184-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87184-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87184-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="87184-111">Supported resource</span></span> | <span data-ttu-id="87184-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87184-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87184-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87184-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87184-114">Application</span><span class="sxs-lookup"><span data-stu-id="87184-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="87184-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="87184-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="87184-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-116">Not supported</span></span> | <span data-ttu-id="87184-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-117">Not supported</span></span> | <span data-ttu-id="87184-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="87184-119">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="87184-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="87184-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="87184-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-121">Not supported</span></span> | <span data-ttu-id="87184-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="87184-123">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="87184-123">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="87184-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-124">Not supported</span></span> | <span data-ttu-id="87184-125">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-125">Not supported</span></span> | <span data-ttu-id="87184-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="87184-127">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="87184-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="87184-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87184-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="87184-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-129">Not supported</span></span> | <span data-ttu-id="87184-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="87184-131">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="87184-131">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="87184-132">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-132">Not supported</span></span> | <span data-ttu-id="87184-133">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-133">Not supported</span></span> | <span data-ttu-id="87184-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="87184-135">contato</span><span class="sxs-lookup"><span data-stu-id="87184-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="87184-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="87184-136">Contacts.Read</span></span> | <span data-ttu-id="87184-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="87184-137">Contacts.Read</span></span> | <span data-ttu-id="87184-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="87184-138">Contacts.Read</span></span> |
|<span data-ttu-id="87184-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="87184-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="87184-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-140">Not supported</span></span> | <span data-ttu-id="87184-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87184-141">Files.ReadWrite</span></span> | <span data-ttu-id="87184-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-142">Not supported</span></span> |
|<span data-ttu-id="87184-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="87184-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="87184-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="87184-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-145">Not supported</span></span> | <span data-ttu-id="87184-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="87184-147">evento</span><span class="sxs-lookup"><span data-stu-id="87184-147">event</span></span>](../resources/event.md) | <span data-ttu-id="87184-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="87184-148">Calendars.Read</span></span> | <span data-ttu-id="87184-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="87184-149">Calendars.Read</span></span> | <span data-ttu-id="87184-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="87184-150">Calendars.Read</span></span> |
|[<span data-ttu-id="87184-151">grupo</span><span class="sxs-lookup"><span data-stu-id="87184-151">group</span></span>](../resources/group.md) | <span data-ttu-id="87184-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-152">Group.Read.All</span></span> | <span data-ttu-id="87184-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-153">Not supported</span></span> | <span data-ttu-id="87184-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-154">Group.Read.All</span></span> |
|[<span data-ttu-id="87184-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="87184-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="87184-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-156">Group.Read.All</span></span> | <span data-ttu-id="87184-157">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-157">Not supported</span></span> | <span data-ttu-id="87184-158">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-158">Not supported</span></span> |
|[<span data-ttu-id="87184-159">list</span><span class="sxs-lookup"><span data-stu-id="87184-159">list</span></span>](../resources/list.md) | <span data-ttu-id="87184-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="87184-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-161">Not supported</span></span> | <span data-ttu-id="87184-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="87184-163">message</span><span class="sxs-lookup"><span data-stu-id="87184-163">message</span></span>](../resources/message.md) | <span data-ttu-id="87184-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="87184-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="87184-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="87184-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="87184-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="87184-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="87184-167">presence</span><span class="sxs-lookup"><span data-stu-id="87184-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="87184-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-168">Presence.Read.All</span></span> | <span data-ttu-id="87184-169">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-169">Not supported</span></span> | <span data-ttu-id="87184-170">Incompatível</span><span class="sxs-lookup"><span data-stu-id="87184-170">Not supported</span></span> |
|[<span data-ttu-id="87184-171">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="87184-171">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="87184-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-172">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="87184-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="87184-173">Not supported</span></span> | <span data-ttu-id="87184-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87184-174">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="87184-175">Usuário</span><span class="sxs-lookup"><span data-stu-id="87184-175">user</span></span>](../resources/user.md) | <span data-ttu-id="87184-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-176">User.Read.All</span></span> | <span data-ttu-id="87184-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-177">User.Read.All</span></span> | <span data-ttu-id="87184-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="87184-178">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="87184-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="87184-179">chatMessage</span></span>

<span data-ttu-id="87184-180">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="87184-180">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="87184-181">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="87184-181">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="87184-182">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="87184-182">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="87184-183">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="87184-183">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="87184-184">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="87184-184">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="87184-185">**Observação:** `/teams/allMessages` e que `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="87184-185">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="87184-186">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="87184-186">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="87184-187">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="87184-187">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="87184-188">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="87184-188">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="87184-189">driveItem</span><span class="sxs-lookup"><span data-stu-id="87184-189">driveItem</span></span>

<span data-ttu-id="87184-190">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="87184-190">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="87184-191">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="87184-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="87184-192">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="87184-192">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="87184-193">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="87184-193">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="87184-194">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="87184-194">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="87184-195">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="87184-195">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="87184-196">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="87184-196">contact, event, and message</span></span>

<span data-ttu-id="87184-197">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="87184-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="87184-198">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="87184-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="87184-199">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="87184-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="87184-200">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="87184-200">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="87184-201">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="87184-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="87184-202">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="87184-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="87184-203">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="87184-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="87184-204">presença</span><span class="sxs-lookup"><span data-stu-id="87184-204">presence</span></span>

<span data-ttu-id="87184-205">as assinaturas de **presença** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="87184-205">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="87184-206">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="87184-206">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="87184-207">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87184-207">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="87184-208">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87184-208">Request headers</span></span>

| <span data-ttu-id="87184-209">Nome</span><span class="sxs-lookup"><span data-stu-id="87184-209">Name</span></span>       | <span data-ttu-id="87184-210">Tipo</span><span class="sxs-lookup"><span data-stu-id="87184-210">Type</span></span> | <span data-ttu-id="87184-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="87184-211">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="87184-212">Autorização</span><span class="sxs-lookup"><span data-stu-id="87184-212">Authorization</span></span>  | <span data-ttu-id="87184-213">string</span><span class="sxs-lookup"><span data-stu-id="87184-213">string</span></span>  | <span data-ttu-id="87184-p110">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87184-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="87184-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="87184-216">Response</span></span>

<span data-ttu-id="87184-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87184-217">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="87184-218">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="87184-218">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="87184-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87184-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="87184-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87184-220">Request</span></span>

<span data-ttu-id="87184-221">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="87184-221">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="87184-222">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="87184-222">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="87184-223">Esta solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="87184-223">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="87184-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="87184-224">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="87184-225">C#</span><span class="sxs-lookup"><span data-stu-id="87184-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87184-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87184-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87184-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87184-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="87184-228">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="87184-228">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="87184-229">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="87184-229">Resource type</span></span> | <span data-ttu-id="87184-230">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87184-230">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="87184-231">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="87184-231">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="87184-232">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="87184-232">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="87184-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span><span class="sxs-lookup"><span data-stu-id="87184-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span></span> |
|[<span data-ttu-id="87184-234">Contatos</span><span class="sxs-lookup"><span data-stu-id="87184-234">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="87184-235">Conversas</span><span class="sxs-lookup"><span data-stu-id="87184-235">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="87184-236">Unidades</span><span class="sxs-lookup"><span data-stu-id="87184-236">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="87184-237">Eventos</span><span class="sxs-lookup"><span data-stu-id="87184-237">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="87184-238">Grupos</span><span class="sxs-lookup"><span data-stu-id="87184-238">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="87184-239">List</span><span class="sxs-lookup"><span data-stu-id="87184-239">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="87184-240">Email</span><span class="sxs-lookup"><span data-stu-id="87184-240">Mail</span></span>](../resources/message.md)|<span data-ttu-id="87184-241">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="87184-241">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="87184-242">Presença</span><span class="sxs-lookup"><span data-stu-id="87184-242">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="87184-243">`/communications/presences/{id}`(usuário único), `/communications/presences?$filter=id in ({id},{id}…)` (vários usuários)</span><span class="sxs-lookup"><span data-stu-id="87184-243">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="87184-244">Usuários</span><span class="sxs-lookup"><span data-stu-id="87184-244">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="87184-245">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="87184-245">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="87184-246">**Observação:** Qualquer caminho iniciado com `me` também pode ser usado com `users/{id}` o ao invés de `me` direcionar um usuário específico, e não o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="87184-246">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="87184-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="87184-247">Response</span></span>

<span data-ttu-id="87184-248">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="87184-248">The following example shows the response.</span></span> 

><span data-ttu-id="87184-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87184-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="87184-251">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="87184-251">Notification endpoint validation</span></span>

<span data-ttu-id="87184-252">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="87184-252">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="87184-253">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="87184-253">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
