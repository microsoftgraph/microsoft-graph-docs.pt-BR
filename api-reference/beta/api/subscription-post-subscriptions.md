---
title: Criar assinatura
description: Assina um aplicativo de escuta para receber notificações de alteração quando os dados de um recurso do Microsoft Graph são alterados.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: d9d20e934965485c9c6262ceacb86ca304bc134d
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408124"
---
# <a name="create-subscription"></a><span data-ttu-id="5da10-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="5da10-103">Create subscription</span></span>

<span data-ttu-id="5da10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5da10-105">Assina um aplicativo de escuta para receber notificações de alteração quando o tipo solicitado de alterações ocorrerem no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5da10-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="5da10-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5da10-106">Permissions</span></span>

<span data-ttu-id="5da10-107">A criação de uma assinatura requer permissão de leitura para o recurso.</span><span class="sxs-lookup"><span data-stu-id="5da10-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="5da10-108">Por exemplo, para obter notificações de alteração em mensagens, seu aplicativo precisa da permissão mail. Read.</span><span class="sxs-lookup"><span data-stu-id="5da10-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="5da10-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="5da10-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5da10-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5da10-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5da10-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-111">Supported resource</span></span> | <span data-ttu-id="5da10-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5da10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5da10-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5da10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5da10-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5da10-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="5da10-115">[callRecord](../resources/callrecords-callrecord.md) (/Communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="5da10-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="5da10-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-116">Not supported</span></span> | <span data-ttu-id="5da10-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-117">Not supported</span></span> | <span data-ttu-id="5da10-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="5da10-119">[chat](../resources/chatmessage.md) (/Teams/{ID}/Channels/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="5da10-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="5da10-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-120">Not supported</span></span> | <span data-ttu-id="5da10-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-121">Not supported</span></span> | <span data-ttu-id="5da10-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5da10-123">[chat](../resources/chatmessage.md) (/Teams/allMessages--todas as mensagens do canal na organização)</span><span class="sxs-lookup"><span data-stu-id="5da10-123">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="5da10-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-124">Not supported</span></span> | <span data-ttu-id="5da10-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-125">Not supported</span></span> | <span data-ttu-id="5da10-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5da10-127">[chat](../resources/chatmessage.md) (/chats/{ID}/Messages)</span><span class="sxs-lookup"><span data-stu-id="5da10-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="5da10-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-128">Not supported</span></span> | <span data-ttu-id="5da10-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-129">Not supported</span></span> | <span data-ttu-id="5da10-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="5da10-131">[chat](../resources/chatmessage.md) (/chats/allMessages--todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="5da10-131">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="5da10-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-132">Not supported</span></span> | <span data-ttu-id="5da10-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-133">Not supported</span></span> | <span data-ttu-id="5da10-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="5da10-135">contato</span><span class="sxs-lookup"><span data-stu-id="5da10-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5da10-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-136">Contacts.Read</span></span> | <span data-ttu-id="5da10-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-137">Contacts.Read</span></span> | <span data-ttu-id="5da10-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-138">Contacts.Read</span></span> |
|<span data-ttu-id="5da10-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="5da10-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5da10-140">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5da10-140">Not supported</span></span> | <span data-ttu-id="5da10-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5da10-141">Files.ReadWrite</span></span> | <span data-ttu-id="5da10-142">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5da10-142">Not supported</span></span> |
|<span data-ttu-id="5da10-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="5da10-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5da10-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da10-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="5da10-145">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5da10-145">Not supported</span></span> | <span data-ttu-id="5da10-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da10-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5da10-147">evento</span><span class="sxs-lookup"><span data-stu-id="5da10-147">event</span></span>](../resources/event.md) | <span data-ttu-id="5da10-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-148">Calendars.Read</span></span> | <span data-ttu-id="5da10-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-149">Calendars.Read</span></span> | <span data-ttu-id="5da10-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-150">Calendars.Read</span></span> |
|[<span data-ttu-id="5da10-151">grupo</span><span class="sxs-lookup"><span data-stu-id="5da10-151">group</span></span>](../resources/group.md) | <span data-ttu-id="5da10-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-152">Group.Read.All</span></span> | <span data-ttu-id="5da10-153">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5da10-153">Not supported</span></span> | <span data-ttu-id="5da10-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-154">Group.Read.All</span></span> |
|[<span data-ttu-id="5da10-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="5da10-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5da10-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-156">Group.Read.All</span></span> | <span data-ttu-id="5da10-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-157">Not supported</span></span> | <span data-ttu-id="5da10-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-158">Not supported</span></span> |
|[<span data-ttu-id="5da10-159">list</span><span class="sxs-lookup"><span data-stu-id="5da10-159">list</span></span>](../resources/list.md) | <span data-ttu-id="5da10-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da10-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="5da10-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5da10-161">Not supported</span></span> | <span data-ttu-id="5da10-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da10-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="5da10-163">message</span><span class="sxs-lookup"><span data-stu-id="5da10-163">message</span></span>](../resources/message.md) | <span data-ttu-id="5da10-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5da10-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5da10-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5da10-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="5da10-167">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="5da10-167">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="5da10-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da10-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5da10-169">Incompatível</span><span class="sxs-lookup"><span data-stu-id="5da10-169">Not supported</span></span> | <span data-ttu-id="5da10-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da10-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5da10-171">Usuário</span><span class="sxs-lookup"><span data-stu-id="5da10-171">user</span></span>](../resources/user.md) | <span data-ttu-id="5da10-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-172">User.Read.All</span></span> | <span data-ttu-id="5da10-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-173">User.Read.All</span></span> | <span data-ttu-id="5da10-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da10-174">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="5da10-175">Chat (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="5da10-175">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="5da10-176">as assinaturas do **chat** exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="5da10-176">**chatMessage** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="5da10-177">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="5da10-177">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="5da10-178">Antes de criar uma assinatura do **chat** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="5da10-178">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="5da10-179">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="5da10-179">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="5da10-180">**Observação:** `/teams/allMessages` e que `/chats/allMessages` estão atualmente em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="5da10-180">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="5da10-181">Durante a visualização, você pode usar essa API sem taxas, sujeita aos [termos de uso das APIs da Microsoft](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="5da10-181">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="5da10-182">No entanto, os usuários de aplicativos que usam a API podem ser solicitados a ter assinaturas para ofertas específicas do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5da10-182">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="5da10-183">Na disponibilidade geral, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.</span><span class="sxs-lookup"><span data-stu-id="5da10-183">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="5da10-184">driveItem (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="5da10-184">driveItem (OneDrive)</span></span>

<span data-ttu-id="5da10-185">Limitações adicionais se aplicam a assinaturas em itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5da10-185">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="5da10-186">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="5da10-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="5da10-187">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="5da10-187">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5da10-188">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="5da10-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5da10-189">As notificações de alteração são enviadas para os tipos solicitados de alterações na pasta inscrita ou qualquer arquivo, pasta ou outra instância do **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="5da10-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="5da10-190">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="5da10-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="5da10-191">contato, evento e mensagem (Outlook)</span><span class="sxs-lookup"><span data-stu-id="5da10-191">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="5da10-192">Limitações adicionais se aplicam a assinaturas em itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="5da10-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="5da10-193">As limitações se aplicam à criação e ao gerenciamento (obter, atualizar e excluir) assinaturas.</span><span class="sxs-lookup"><span data-stu-id="5da10-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="5da10-194">A permissão delegada oferece suporte à assinatura de itens em pastas somente na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5da10-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5da10-195">Isso significa que, por exemplo, não é possível usar a permissão delegada Calendars.Read para inscrever eventos na caixa de correio de terceiros.</span><span class="sxs-lookup"><span data-stu-id="5da10-195">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5da10-196">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="5da10-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5da10-197">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="5da10-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5da10-198">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="5da10-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="5da10-199">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5da10-199">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="5da10-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5da10-200">Request headers</span></span>

| <span data-ttu-id="5da10-201">Nome</span><span class="sxs-lookup"><span data-stu-id="5da10-201">Name</span></span>       | <span data-ttu-id="5da10-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="5da10-202">Type</span></span> | <span data-ttu-id="5da10-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="5da10-203">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5da10-204">Autorização</span><span class="sxs-lookup"><span data-stu-id="5da10-204">Authorization</span></span>  | <span data-ttu-id="5da10-205">string</span><span class="sxs-lookup"><span data-stu-id="5da10-205">string</span></span>  | <span data-ttu-id="5da10-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5da10-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5da10-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="5da10-208">Response</span></span>

<span data-ttu-id="5da10-209">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [Subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5da10-209">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="5da10-210">Para obter detalhes sobre como os erros são retornados, confira [respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="5da10-210">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="5da10-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5da10-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="5da10-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5da10-212">Request</span></span>

<span data-ttu-id="5da10-213">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="5da10-213">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="5da10-214">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="5da10-214">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="5da10-215">Esta solicitação cria uma assinatura para notificações de alteração sobre novos emails recebidos pelo usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="5da10-215">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="5da10-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="5da10-216">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5da10-217">C#</span><span class="sxs-lookup"><span data-stu-id="5da10-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5da10-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5da10-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5da10-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5da10-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5da10-220">Estes são os valores válidos para a Propriedade Resource.</span><span class="sxs-lookup"><span data-stu-id="5da10-220">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="5da10-221">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="5da10-221">Resource type</span></span> | <span data-ttu-id="5da10-222">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5da10-222">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="5da10-223">Email</span><span class="sxs-lookup"><span data-stu-id="5da10-223">Mail</span></span>|<span data-ttu-id="5da10-224">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="5da10-224">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="5da10-225">me/messages</span><span class="sxs-lookup"><span data-stu-id="5da10-225">me/messages</span></span>|
|<span data-ttu-id="5da10-226">Contatos</span><span class="sxs-lookup"><span data-stu-id="5da10-226">Contacts</span></span>|<span data-ttu-id="5da10-227">me/contacts</span><span class="sxs-lookup"><span data-stu-id="5da10-227">me/contacts</span></span>|
|<span data-ttu-id="5da10-228">Calendários</span><span class="sxs-lookup"><span data-stu-id="5da10-228">Calendars</span></span>|<span data-ttu-id="5da10-229">me/events</span><span class="sxs-lookup"><span data-stu-id="5da10-229">me/events</span></span>|
|<span data-ttu-id="5da10-230">Usuários</span><span class="sxs-lookup"><span data-stu-id="5da10-230">Users</span></span>|<span data-ttu-id="5da10-231">usuários</span><span class="sxs-lookup"><span data-stu-id="5da10-231">users</span></span>|
|<span data-ttu-id="5da10-232">Grupos</span><span class="sxs-lookup"><span data-stu-id="5da10-232">Groups</span></span>|<span data-ttu-id="5da10-233">grupos</span><span class="sxs-lookup"><span data-stu-id="5da10-233">groups</span></span>|
|<span data-ttu-id="5da10-234">Conversas</span><span class="sxs-lookup"><span data-stu-id="5da10-234">Conversations</span></span>|<span data-ttu-id="5da10-235">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="5da10-235">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="5da10-236">Unidades</span><span class="sxs-lookup"><span data-stu-id="5da10-236">Drives</span></span>|<span data-ttu-id="5da10-237">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="5da10-237">me/drive/root</span></span>|
|<span data-ttu-id="5da10-238">Listar</span><span class="sxs-lookup"><span data-stu-id="5da10-238">List</span></span>|<span data-ttu-id="5da10-239">sites/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="5da10-239">sites/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="5da10-240">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="5da10-240">Security alert</span></span>|<span data-ttu-id="5da10-241">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="5da10-241">security/alerts?$filter=status eq ‘New’</span></span>|
|<span data-ttu-id="5da10-242">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="5da10-242">Call records</span></span>|<span data-ttu-id="5da10-243">comunicações/callRecords</span><span class="sxs-lookup"><span data-stu-id="5da10-243">communications/callRecords</span></span>|
|[<span data-ttu-id="5da10-244">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="5da10-244">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="5da10-245">chats/{ID}/mensagens, chats/multimessages, Teams/{ID}/Channels/{ID}/mensagens, equipes/próprias mensagens</span><span class="sxs-lookup"><span data-stu-id="5da10-245">chats/{id}/messages, chats/allMessages, teams/{id}/channels/{id}/messages, teams/allMessages</span></span> |

### <a name="response"></a><span data-ttu-id="5da10-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="5da10-246">Response</span></span>

<span data-ttu-id="5da10-247">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="5da10-247">The following example shows the response.</span></span> 

><span data-ttu-id="5da10-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5da10-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="5da10-250">Validação de ponto de extremidade de notificação</span><span class="sxs-lookup"><span data-stu-id="5da10-250">Notification endpoint validation</span></span>

<span data-ttu-id="5da10-251">O ponto de extremidade de notificação de assinatura (especificado na propriedade **notificationUrl** ) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="5da10-251">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="5da10-252">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="5da10-252">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
