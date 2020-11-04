---
title: Criar assinatura
description: Inscreve um aplicativo de ouvinte para receber notificações de alterações quando os dados no Microsoft Graph forem alterados.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d751cd722bcbf69ac00dae4200424ed9ba0e25f2
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848181"
---
# <a name="create-subscription"></a><span data-ttu-id="0c7a5-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="0c7a5-103">Create subscription</span></span>

<span data-ttu-id="0c7a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c7a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c7a5-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c7a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c7a5-106">Permissions</span></span>

 <span data-ttu-id="0c7a5-107">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="0c7a5-108">Por exemplo, para receber notificações de alterações por mensagens, seu aplicativo precisa da permissão`Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="0c7a5-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="0c7a5-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c7a5-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-111">Supported resource</span></span> | <span data-ttu-id="0c7a5-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c7a5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c7a5-114">Application</span><span class="sxs-lookup"><span data-stu-id="0c7a5-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="0c7a5-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="0c7a5-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0c7a5-116">Not supported</span></span> | <span data-ttu-id="0c7a5-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0c7a5-117">Not supported</span></span> | <span data-ttu-id="0c7a5-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="0c7a5-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="0c7a5-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-120">Not supported</span></span> | <span data-ttu-id="0c7a5-121">Incompatível</span><span class="sxs-lookup"><span data-stu-id="0c7a5-121">Not supported</span></span> |  <span data-ttu-id="0c7a5-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0c7a5-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="0c7a5-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-124">Not supported</span></span> | <span data-ttu-id="0c7a5-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-125">Not supported</span></span> | <span data-ttu-id="0c7a5-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0c7a5-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="0c7a5-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-128">Not supported</span></span> | <span data-ttu-id="0c7a5-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-129">Not supported</span></span> | <span data-ttu-id="0c7a5-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="0c7a5-131">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="0c7a5-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-132">Not supported</span></span> | <span data-ttu-id="0c7a5-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-133">Not supported</span></span> | <span data-ttu-id="0c7a5-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="0c7a5-135">contato</span><span class="sxs-lookup"><span data-stu-id="0c7a5-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="0c7a5-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-136">Contacts.Read</span></span> | <span data-ttu-id="0c7a5-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-137">Contacts.Read</span></span> | <span data-ttu-id="0c7a5-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-138">Contacts.Read</span></span> |
|<span data-ttu-id="0c7a5-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="0c7a5-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-140">Not supported</span></span> | <span data-ttu-id="0c7a5-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c7a5-141">Files.ReadWrite</span></span> | <span data-ttu-id="0c7a5-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-142">Not supported</span></span> |
|<span data-ttu-id="0c7a5-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="0c7a5-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="0c7a5-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="0c7a5-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-145">Not supported</span></span> | <span data-ttu-id="0c7a5-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="0c7a5-147">evento</span><span class="sxs-lookup"><span data-stu-id="0c7a5-147">event</span></span>](../resources/event.md) | <span data-ttu-id="0c7a5-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-148">Calendars.Read</span></span> | <span data-ttu-id="0c7a5-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-149">Calendars.Read</span></span> | <span data-ttu-id="0c7a5-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-150">Calendars.Read</span></span> |
|[<span data-ttu-id="0c7a5-151">grupo</span><span class="sxs-lookup"><span data-stu-id="0c7a5-151">group</span></span>](../resources/group.md) | <span data-ttu-id="0c7a5-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-152">Group.Read.All</span></span> | <span data-ttu-id="0c7a5-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-153">Not supported</span></span> | <span data-ttu-id="0c7a5-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-154">Group.Read.All</span></span> |
|[<span data-ttu-id="0c7a5-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="0c7a5-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="0c7a5-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-156">Group.Read.All</span></span> | <span data-ttu-id="0c7a5-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-157">Not supported</span></span> | <span data-ttu-id="0c7a5-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-158">Not supported</span></span> |
|[<span data-ttu-id="0c7a5-159">list</span><span class="sxs-lookup"><span data-stu-id="0c7a5-159">list</span></span>](../resources/list.md) | <span data-ttu-id="0c7a5-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="0c7a5-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-161">Not supported</span></span> | <span data-ttu-id="0c7a5-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="0c7a5-163">message</span><span class="sxs-lookup"><span data-stu-id="0c7a5-163">message</span></span>](../resources/message.md) | <span data-ttu-id="0c7a5-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0c7a5-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0c7a5-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0c7a5-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="0c7a5-167">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="0c7a5-167">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="0c7a5-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="0c7a5-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0c7a5-169">Not supported</span></span> | <span data-ttu-id="0c7a5-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="0c7a5-171">Usuário</span><span class="sxs-lookup"><span data-stu-id="0c7a5-171">user</span></span>](../resources/user.md) | <span data-ttu-id="0c7a5-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-172">User.Read.All</span></span> | <span data-ttu-id="0c7a5-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-173">User.Read.All</span></span> | <span data-ttu-id="0c7a5-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7a5-174">User.Read.All</span></span> |

> <span data-ttu-id="0c7a5-175">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-175">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="0c7a5-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0c7a5-176">chatMessage</span></span>

<span data-ttu-id="0c7a5-177">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-177">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="0c7a5-178">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-178">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="0c7a5-179">Antes de criar uma assinatura **chatMessage** , você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-179">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="0c7a5-180">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-180">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="0c7a5-181">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-181">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="0c7a5-182">**Observação:**`/chats/getAllMessages` retorna apenas mensagens de bate papo pertencentes ao locatário.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-182">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="0c7a5-183">Se um thread de bate papo for iniciado por um usuário fora do locatário, esse thread de bate papo não será de propriedade do locatário e não criará notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-183">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="0c7a5-184">driveItem</span><span class="sxs-lookup"><span data-stu-id="0c7a5-184">driveItem</span></span>

<span data-ttu-id="0c7a5-185">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-185">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="0c7a5-186">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="0c7a5-187">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-187">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="0c7a5-188">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="0c7a5-189">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="0c7a5-190">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="0c7a5-191">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="0c7a5-191">contact, event, and message</span></span>

<span data-ttu-id="0c7a5-192">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="0c7a5-193">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="0c7a5-194">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="0c7a5-195">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-195">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="0c7a5-196">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_ :</span><span class="sxs-lookup"><span data-stu-id="0c7a5-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="0c7a5-197">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="0c7a5-198">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c7a5-199">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c7a5-199">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="0c7a5-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7a5-200">Request headers</span></span>

| <span data-ttu-id="0c7a5-201">Nome</span><span class="sxs-lookup"><span data-stu-id="0c7a5-201">Name</span></span>       | <span data-ttu-id="0c7a5-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c7a5-202">Type</span></span> | <span data-ttu-id="0c7a5-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7a5-203">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c7a5-204">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c7a5-204">Authorization</span></span>  | <span data-ttu-id="0c7a5-205">string</span><span class="sxs-lookup"><span data-stu-id="0c7a5-205">string</span></span>  | <span data-ttu-id="0c7a5-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0c7a5-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c7a5-208">Response</span></span>

<span data-ttu-id="0c7a5-209">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-209">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="0c7a5-210">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="0c7a5-210">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="0c7a5-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c7a5-211">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0c7a5-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7a5-212">Request</span></span>

<span data-ttu-id="0c7a5-213">Veja a seguir um exemplo da solicitação de envio de uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-213">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c7a5-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c7a5-214">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
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
# <a name="c"></a>[<span data-ttu-id="0c7a5-215">C#</span><span class="sxs-lookup"><span data-stu-id="0c7a5-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c7a5-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c7a5-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c7a5-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c7a5-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c7a5-218">Java</span><span class="sxs-lookup"><span data-stu-id="0c7a5-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0c7a5-219">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-219">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="0c7a5-220">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-220">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="0c7a5-221">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="0c7a5-221">Resources examples</span></span>

<span data-ttu-id="0c7a5-222">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="0c7a5-222">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="0c7a5-223">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="0c7a5-223">Resource type</span></span> | <span data-ttu-id="0c7a5-224">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0c7a5-224">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="0c7a5-225">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="0c7a5-225">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="0c7a5-226">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="0c7a5-226">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0c7a5-227">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="0c7a5-227">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="0c7a5-228">Contatos</span><span class="sxs-lookup"><span data-stu-id="0c7a5-228">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="0c7a5-229">Conversas</span><span class="sxs-lookup"><span data-stu-id="0c7a5-229">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="0c7a5-230">Unidades</span><span class="sxs-lookup"><span data-stu-id="0c7a5-230">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="0c7a5-231">Eventos</span><span class="sxs-lookup"><span data-stu-id="0c7a5-231">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="0c7a5-232">Grupos</span><span class="sxs-lookup"><span data-stu-id="0c7a5-232">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="0c7a5-233">Lista</span><span class="sxs-lookup"><span data-stu-id="0c7a5-233">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="0c7a5-234">Email</span><span class="sxs-lookup"><span data-stu-id="0c7a5-234">Mail</span></span>](../resources/message.md)|<span data-ttu-id="0c7a5-235">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="0c7a5-235">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="0c7a5-236">Usuários</span><span class="sxs-lookup"><span data-stu-id="0c7a5-236">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="0c7a5-237">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="0c7a5-237">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="0c7a5-238">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-238">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="0c7a5-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c7a5-239">Response</span></span>

<span data-ttu-id="0c7a5-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="0c7a5-243">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="0c7a5-243">Notification endpoint validation</span></span>

<span data-ttu-id="0c7a5-244">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="0c7a5-244">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="0c7a5-245">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="0c7a5-245">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

