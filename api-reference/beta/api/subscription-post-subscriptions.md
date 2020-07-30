---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: bae074c7599119063053069765c0653ce405e231
ms.sourcegitcommit: ff3fd4ead2b864ce6abb79915a0488d0562347f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46524335"
---
# <a name="create-subscription"></a><span data-ttu-id="0da40-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="0da40-103">Create subscription</span></span>

<span data-ttu-id="0da40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0da40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0da40-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0da40-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="0da40-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0da40-106">Permissions</span></span>

<span data-ttu-id="0da40-107">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="0da40-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="0da40-108">Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="0da40-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="0da40-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="0da40-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="0da40-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0da40-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0da40-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-111">Supported resource</span></span> | <span data-ttu-id="0da40-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0da40-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0da40-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0da40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da40-114">Application</span><span class="sxs-lookup"><span data-stu-id="0da40-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="0da40-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="0da40-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="0da40-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-116">Not supported</span></span> | <span data-ttu-id="0da40-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-117">Not supported</span></span> | <span data-ttu-id="0da40-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="0da40-119">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="0da40-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="0da40-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="0da40-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-121">Not supported</span></span> | <span data-ttu-id="0da40-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0da40-123">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="0da40-123">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="0da40-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-124">Not supported</span></span> | <span data-ttu-id="0da40-125">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-125">Not supported</span></span> | <span data-ttu-id="0da40-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0da40-127">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="0da40-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="0da40-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0da40-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="0da40-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-129">Not supported</span></span> | <span data-ttu-id="0da40-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="0da40-131">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="0da40-131">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="0da40-132">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-132">Not supported</span></span> | <span data-ttu-id="0da40-133">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-133">Not supported</span></span> | <span data-ttu-id="0da40-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="0da40-135">contato</span><span class="sxs-lookup"><span data-stu-id="0da40-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="0da40-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-136">Contacts.Read</span></span> | <span data-ttu-id="0da40-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-137">Contacts.Read</span></span> | <span data-ttu-id="0da40-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-138">Contacts.Read</span></span> |
|<span data-ttu-id="0da40-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="0da40-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="0da40-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-140">Not supported</span></span> | <span data-ttu-id="0da40-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0da40-141">Files.ReadWrite</span></span> | <span data-ttu-id="0da40-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-142">Not supported</span></span> |
|<span data-ttu-id="0da40-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="0da40-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="0da40-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="0da40-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-145">Not supported</span></span> | <span data-ttu-id="0da40-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="0da40-147">evento</span><span class="sxs-lookup"><span data-stu-id="0da40-147">event</span></span>](../resources/event.md) | <span data-ttu-id="0da40-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-148">Calendars.Read</span></span> | <span data-ttu-id="0da40-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-149">Calendars.Read</span></span> | <span data-ttu-id="0da40-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-150">Calendars.Read</span></span> |
|[<span data-ttu-id="0da40-151">grupo</span><span class="sxs-lookup"><span data-stu-id="0da40-151">group</span></span>](../resources/group.md) | <span data-ttu-id="0da40-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-152">Group.Read.All</span></span> | <span data-ttu-id="0da40-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-153">Not supported</span></span> | <span data-ttu-id="0da40-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-154">Group.Read.All</span></span> |
|[<span data-ttu-id="0da40-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="0da40-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="0da40-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-156">Group.Read.All</span></span> | <span data-ttu-id="0da40-157">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-157">Not supported</span></span> | <span data-ttu-id="0da40-158">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0da40-158">Not supported</span></span> |
|[<span data-ttu-id="0da40-159">list</span><span class="sxs-lookup"><span data-stu-id="0da40-159">list</span></span>](../resources/list.md) | <span data-ttu-id="0da40-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="0da40-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-161">Not supported</span></span> | <span data-ttu-id="0da40-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="0da40-163">message</span><span class="sxs-lookup"><span data-stu-id="0da40-163">message</span></span>](../resources/message.md) | <span data-ttu-id="0da40-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0da40-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0da40-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0da40-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="0da40-167">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="0da40-167">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="0da40-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="0da40-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0da40-169">Not supported</span></span> | <span data-ttu-id="0da40-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0da40-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="0da40-171">Usuário</span><span class="sxs-lookup"><span data-stu-id="0da40-171">user</span></span>](../resources/user.md) | <span data-ttu-id="0da40-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-172">User.Read.All</span></span> | <span data-ttu-id="0da40-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-173">User.Read.All</span></span> | <span data-ttu-id="0da40-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da40-174">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="0da40-175">Chat (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="0da40-175">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="0da40-176">as assinaturas do **chat** com permissões delegadas não dão suporte a dados de recurso (o**includeResourceData** deve ser `false` ) e não precisam de [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="0da40-176">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="0da40-177">as assinaturas do **chat** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="0da40-177">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="0da40-178">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="0da40-178">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="0da40-179">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="0da40-179">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="0da40-180">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="0da40-180">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

> <span data-ttu-id="0da40-181">**Observação:** `/teams/allMessages` e que `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="0da40-181">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="0da40-182">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="0da40-182">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="0da40-183">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0da40-183">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="0da40-184">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="0da40-184">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="0da40-185">driveItem (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="0da40-185">driveItem (OneDrive)</span></span>

<span data-ttu-id="0da40-186">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0da40-186">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="0da40-187">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0da40-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="0da40-188">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="0da40-188">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="0da40-189">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="0da40-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="0da40-190">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="0da40-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="0da40-191">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="0da40-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="0da40-192">contato, evento e mensagem (Outlook)</span><span class="sxs-lookup"><span data-stu-id="0da40-192">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="0da40-193">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="0da40-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="0da40-194">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0da40-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="0da40-195">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="0da40-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="0da40-196">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="0da40-196">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="0da40-197">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="0da40-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="0da40-198">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="0da40-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="0da40-199">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="0da40-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="0da40-200">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0da40-200">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="0da40-201">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0da40-201">Request headers</span></span>

| <span data-ttu-id="0da40-202">Nome</span><span class="sxs-lookup"><span data-stu-id="0da40-202">Name</span></span>       | <span data-ttu-id="0da40-203">Tipo</span><span class="sxs-lookup"><span data-stu-id="0da40-203">Type</span></span> | <span data-ttu-id="0da40-204">Descrição</span><span class="sxs-lookup"><span data-stu-id="0da40-204">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0da40-205">Autorização</span><span class="sxs-lookup"><span data-stu-id="0da40-205">Authorization</span></span>  | <span data-ttu-id="0da40-206">string</span><span class="sxs-lookup"><span data-stu-id="0da40-206">string</span></span>  | <span data-ttu-id="0da40-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0da40-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0da40-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="0da40-209">Response</span></span>

<span data-ttu-id="0da40-210">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0da40-210">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="0da40-211">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="0da40-211">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="0da40-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0da40-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="0da40-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0da40-213">Request</span></span>

<span data-ttu-id="0da40-214">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="0da40-214">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="0da40-215">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="0da40-215">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="0da40-216">Esta solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="0da40-216">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="0da40-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="0da40-217">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0da40-218">C#</span><span class="sxs-lookup"><span data-stu-id="0da40-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0da40-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0da40-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0da40-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0da40-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0da40-221">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="0da40-221">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="0da40-222">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="0da40-222">Resource type</span></span> | <span data-ttu-id="0da40-223">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0da40-223">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="0da40-224">Email</span><span class="sxs-lookup"><span data-stu-id="0da40-224">Mail</span></span>|<span data-ttu-id="0da40-225">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="0da40-225">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="0da40-226">me/messages</span><span class="sxs-lookup"><span data-stu-id="0da40-226">me/messages</span></span>|
|<span data-ttu-id="0da40-227">Contatos</span><span class="sxs-lookup"><span data-stu-id="0da40-227">Contacts</span></span>|<span data-ttu-id="0da40-228">me/contacts</span><span class="sxs-lookup"><span data-stu-id="0da40-228">me/contacts</span></span>|
|<span data-ttu-id="0da40-229">Calendários</span><span class="sxs-lookup"><span data-stu-id="0da40-229">Calendars</span></span>|<span data-ttu-id="0da40-230">me/events</span><span class="sxs-lookup"><span data-stu-id="0da40-230">me/events</span></span>|
|<span data-ttu-id="0da40-231">Usuários</span><span class="sxs-lookup"><span data-stu-id="0da40-231">Users</span></span>|<span data-ttu-id="0da40-232">usuários</span><span class="sxs-lookup"><span data-stu-id="0da40-232">users</span></span>|
|<span data-ttu-id="0da40-233">Grupos</span><span class="sxs-lookup"><span data-stu-id="0da40-233">Groups</span></span>|<span data-ttu-id="0da40-234">grupos</span><span class="sxs-lookup"><span data-stu-id="0da40-234">groups</span></span>|
|<span data-ttu-id="0da40-235">Conversas</span><span class="sxs-lookup"><span data-stu-id="0da40-235">Conversations</span></span>|<span data-ttu-id="0da40-236">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="0da40-236">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="0da40-237">Unidades</span><span class="sxs-lookup"><span data-stu-id="0da40-237">Drives</span></span>|<span data-ttu-id="0da40-238">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="0da40-238">me/drive/root</span></span>|
|<span data-ttu-id="0da40-239">Listar</span><span class="sxs-lookup"><span data-stu-id="0da40-239">List</span></span>|<span data-ttu-id="0da40-240">sites/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="0da40-240">sites/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="0da40-241">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="0da40-241">Security alert</span></span>|<span data-ttu-id="0da40-242">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="0da40-242">security/alerts?$filter=status eq ‘New’</span></span>|
|<span data-ttu-id="0da40-243">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="0da40-243">Call records</span></span>|<span data-ttu-id="0da40-244">communications/callRecords</span><span class="sxs-lookup"><span data-stu-id="0da40-244">communications/callRecords</span></span>|
|[<span data-ttu-id="0da40-245">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="0da40-245">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0da40-246">chats/{ID}/mensagens, chats/multimessages, Teams/{ID}/Channels/{ID}/mensagens, equipes/próprias mensagens</span><span class="sxs-lookup"><span data-stu-id="0da40-246">chats/{id}/messages, chats/allMessages, teams/{id}/channels/{id}/messages, teams/allMessages</span></span> |

### <a name="response"></a><span data-ttu-id="0da40-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="0da40-247">Response</span></span>

<span data-ttu-id="0da40-248">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0da40-248">The following example shows the response.</span></span> 

><span data-ttu-id="0da40-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0da40-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="0da40-251">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="0da40-251">Notification endpoint validation</span></span>

<span data-ttu-id="0da40-252">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="0da40-252">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="0da40-253">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="0da40-253">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
