---
title: Criar assinatura
description: Inscreve um aplicativo de ouvinte para receber notificações de alterações quando os dados no Microsoft Graph forem alterados.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 08278945e58c6792e8982d4f7ac1654661c25185
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222936"
---
# <a name="create-subscription"></a><span data-ttu-id="b8bdf-103">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="b8bdf-103">Create subscription</span></span>

<span data-ttu-id="b8bdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8bdf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8bdf-105">Inscreve um aplicativo de ouvinte para receber notificações de alterações quando o tipo de alteração solicitado ocorrer no recurso especificado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8bdf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8bdf-106">Permissions</span></span>

 <span data-ttu-id="b8bdf-107">Criar uma assinatura exige o escopo de leitura do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="b8bdf-108">Por exemplo, para receber notificações de alterações por mensagens, seu aplicativo precisa da permissão`Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="b8bdf-109">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b8bdf-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8bdf-111">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-111">Supported resource</span></span> | <span data-ttu-id="b8bdf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8bdf-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8bdf-114">Application</span><span class="sxs-lookup"><span data-stu-id="b8bdf-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="b8bdf-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="b8bdf-116">Incompatível</span><span class="sxs-lookup"><span data-stu-id="b8bdf-116">Not supported</span></span> | <span data-ttu-id="b8bdf-117">Incompatível</span><span class="sxs-lookup"><span data-stu-id="b8bdf-117">Not supported</span></span> | <span data-ttu-id="b8bdf-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="b8bdf-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="b8bdf-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-120">Not supported</span></span> | <span data-ttu-id="b8bdf-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-121">Not supported</span></span> | <span data-ttu-id="b8bdf-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="b8bdf-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="b8bdf-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-124">Not supported</span></span> | <span data-ttu-id="b8bdf-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-125">Not supported</span></span> | <span data-ttu-id="b8bdf-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="b8bdf-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="b8bdf-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-128">Not supported</span></span> | <span data-ttu-id="b8bdf-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-129">Not supported</span></span> | <span data-ttu-id="b8bdf-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="b8bdf-131">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="b8bdf-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-132">Not supported</span></span> | <span data-ttu-id="b8bdf-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-133">Not supported</span></span> | <span data-ttu-id="b8bdf-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="b8bdf-135">contato</span><span class="sxs-lookup"><span data-stu-id="b8bdf-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b8bdf-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-136">Contacts.Read</span></span> | <span data-ttu-id="b8bdf-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-137">Contacts.Read</span></span> | <span data-ttu-id="b8bdf-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-138">Contacts.Read</span></span> |
|<span data-ttu-id="b8bdf-139">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b8bdf-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-140">Not supported</span></span> | <span data-ttu-id="b8bdf-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8bdf-141">Files.ReadWrite</span></span> | <span data-ttu-id="b8bdf-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-142">Not supported</span></span> |
|<span data-ttu-id="b8bdf-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="b8bdf-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b8bdf-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="b8bdf-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-145">Not supported</span></span> | <span data-ttu-id="b8bdf-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b8bdf-147">evento</span><span class="sxs-lookup"><span data-stu-id="b8bdf-147">event</span></span>](../resources/event.md) | <span data-ttu-id="b8bdf-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-148">Calendars.Read</span></span> | <span data-ttu-id="b8bdf-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-149">Calendars.Read</span></span> | <span data-ttu-id="b8bdf-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-150">Calendars.Read</span></span> |
|[<span data-ttu-id="b8bdf-151">grupo</span><span class="sxs-lookup"><span data-stu-id="b8bdf-151">group</span></span>](../resources/group.md) | <span data-ttu-id="b8bdf-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-152">Group.Read.All</span></span> | <span data-ttu-id="b8bdf-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-153">Not supported</span></span> | <span data-ttu-id="b8bdf-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-154">Group.Read.All</span></span> |
|[<span data-ttu-id="b8bdf-155">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="b8bdf-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b8bdf-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-156">Group.Read.All</span></span> | <span data-ttu-id="b8bdf-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-157">Not supported</span></span> | <span data-ttu-id="b8bdf-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-158">Not supported</span></span> |
|[<span data-ttu-id="b8bdf-159">list</span><span class="sxs-lookup"><span data-stu-id="b8bdf-159">list</span></span>](../resources/list.md) | <span data-ttu-id="b8bdf-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="b8bdf-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-161">Not supported</span></span> | <span data-ttu-id="b8bdf-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="b8bdf-163">message</span><span class="sxs-lookup"><span data-stu-id="b8bdf-163">message</span></span>](../resources/message.md) | <span data-ttu-id="b8bdf-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b8bdf-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b8bdf-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b8bdf-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="b8bdf-167">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b8bdf-167">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="b8bdf-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b8bdf-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b8bdf-169">Not supported</span></span> | <span data-ttu-id="b8bdf-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="b8bdf-171">Usuário</span><span class="sxs-lookup"><span data-stu-id="b8bdf-171">user</span></span>](../resources/user.md) | <span data-ttu-id="b8bdf-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-172">User.Read.All</span></span> | <span data-ttu-id="b8bdf-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-173">User.Read.All</span></span> | <span data-ttu-id="b8bdf-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8bdf-174">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="b8bdf-175">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b8bdf-175">chatMessage</span></span>

<span data-ttu-id="b8bdf-176">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-176">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="b8bdf-177">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-177">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="b8bdf-178">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-178">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="b8bdf-179">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-179">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="b8bdf-180">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as[licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-180">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="b8bdf-181">driveItem</span><span class="sxs-lookup"><span data-stu-id="b8bdf-181">driveItem</span></span>

<span data-ttu-id="b8bdf-182">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-182">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="b8bdf-183">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="b8bdf-184">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-184">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b8bdf-185">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-185">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b8bdf-186">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-186">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="b8bdf-187">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-187">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="b8bdf-188">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="b8bdf-188">contact, event, and message</span></span>

<span data-ttu-id="b8bdf-189">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-189">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="b8bdf-190">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-190">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="b8bdf-191">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-191">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b8bdf-192">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-192">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="b8bdf-193">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="b8bdf-193">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b8bdf-194">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-194">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b8bdf-195">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-195">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8bdf-196">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8bdf-196">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="b8bdf-197">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8bdf-197">Request headers</span></span>

| <span data-ttu-id="b8bdf-198">Nome</span><span class="sxs-lookup"><span data-stu-id="b8bdf-198">Name</span></span>       | <span data-ttu-id="b8bdf-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8bdf-199">Type</span></span> | <span data-ttu-id="b8bdf-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8bdf-200">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8bdf-201">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8bdf-201">Authorization</span></span>  | <span data-ttu-id="b8bdf-202">string</span><span class="sxs-lookup"><span data-stu-id="b8bdf-202">string</span></span>  | <span data-ttu-id="b8bdf-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b8bdf-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8bdf-205">Response</span></span>

<span data-ttu-id="b8bdf-206">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-206">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="b8bdf-207">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="b8bdf-207">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="b8bdf-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8bdf-208">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8bdf-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8bdf-209">Request</span></span>

<span data-ttu-id="b8bdf-210">Veja a seguir um exemplo da solicitação de envio de uma notificação quando o usuário receber um novo email.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-210">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8bdf-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8bdf-211">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b8bdf-212">C#</span><span class="sxs-lookup"><span data-stu-id="b8bdf-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8bdf-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8bdf-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8bdf-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8bdf-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8bdf-215">Java</span><span class="sxs-lookup"><span data-stu-id="b8bdf-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="b8bdf-216">No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-216">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="b8bdf-217">Os campos `clientState` e `latestSupportedTlsVersion` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-217">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="b8bdf-218">Exemplos de recursos</span><span class="sxs-lookup"><span data-stu-id="b8bdf-218">Resources examples</span></span>

<span data-ttu-id="b8bdf-219">Estes são os valores válidos da propriedade de recurso da assinatura:</span><span class="sxs-lookup"><span data-stu-id="b8bdf-219">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="b8bdf-220">Tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="b8bdf-220">Resource type</span></span> | <span data-ttu-id="b8bdf-221">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8bdf-221">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="b8bdf-222">Registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="b8bdf-222">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="b8bdf-223">Mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="b8bdf-223">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b8bdf-224">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="b8bdf-224">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="b8bdf-225">Contatos</span><span class="sxs-lookup"><span data-stu-id="b8bdf-225">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="b8bdf-226">Conversas</span><span class="sxs-lookup"><span data-stu-id="b8bdf-226">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="b8bdf-227">Unidades</span><span class="sxs-lookup"><span data-stu-id="b8bdf-227">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="b8bdf-228">Eventos</span><span class="sxs-lookup"><span data-stu-id="b8bdf-228">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="b8bdf-229">Grupos</span><span class="sxs-lookup"><span data-stu-id="b8bdf-229">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="b8bdf-230">Lista</span><span class="sxs-lookup"><span data-stu-id="b8bdf-230">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="b8bdf-231">Email</span><span class="sxs-lookup"><span data-stu-id="b8bdf-231">Mail</span></span>](../resources/message.md)|<span data-ttu-id="b8bdf-232">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="b8bdf-232">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="b8bdf-233">Usuários</span><span class="sxs-lookup"><span data-stu-id="b8bdf-233">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="b8bdf-234">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b8bdf-234">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="b8bdf-235">**Observação:** qualquer caminho iniciado por `me` também pode ser usado com `users/{id}` em vez de `me` para direcionar um usuário específico, em vez de usar o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-235">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="b8bdf-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8bdf-236">Response</span></span>

<span data-ttu-id="b8bdf-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="b8bdf-240">Validação de ponto de extremidade da notificação</span><span class="sxs-lookup"><span data-stu-id="b8bdf-240">Notification endpoint validation</span></span>

<span data-ttu-id="b8bdf-241">O ponto de extremidade da notificação da assinatura (especificado na `notificationUrl` propriedade) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="b8bdf-241">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="b8bdf-242">Se a validação falhar, a solicitação para criar a assinatura retornará um erro de Solicitação Incorreta 400.</span><span class="sxs-lookup"><span data-stu-id="b8bdf-242">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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

