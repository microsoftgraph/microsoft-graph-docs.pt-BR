---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c6d83614d082341502474aea261b201361df0249
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433468"
---
# <a name="delete-subscription"></a><span data-ttu-id="227f0-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="227f0-103">Delete subscription</span></span>

<span data-ttu-id="227f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="227f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="227f0-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="227f0-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="227f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="227f0-106">Permissions</span></span>

<span data-ttu-id="227f0-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="227f0-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="227f0-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="227f0-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="227f0-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-109">Supported resource</span></span> | <span data-ttu-id="227f0-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="227f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="227f0-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="227f0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="227f0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="227f0-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="227f0-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="227f0-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="227f0-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="227f0-114">Not supported</span></span> | <span data-ttu-id="227f0-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="227f0-115">Not supported</span></span> | <span data-ttu-id="227f0-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="227f0-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="227f0-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="227f0-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-118">Not supported</span></span> | <span data-ttu-id="227f0-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-119">Not supported</span></span> | <span data-ttu-id="227f0-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="227f0-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="227f0-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="227f0-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-122">Not supported</span></span> | <span data-ttu-id="227f0-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-123">Not supported</span></span> | <span data-ttu-id="227f0-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="227f0-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="227f0-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="227f0-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-126">Not supported</span></span> | <span data-ttu-id="227f0-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-127">Not supported</span></span> | <span data-ttu-id="227f0-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="227f0-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="227f0-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="227f0-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-130">Not supported</span></span> | <span data-ttu-id="227f0-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-131">Not supported</span></span> | <span data-ttu-id="227f0-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="227f0-133">contato</span><span class="sxs-lookup"><span data-stu-id="227f0-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="227f0-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-134">Contacts.Read</span></span> | <span data-ttu-id="227f0-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-135">Contacts.Read</span></span> | <span data-ttu-id="227f0-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-136">Contacts.Read</span></span> |
|<span data-ttu-id="227f0-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="227f0-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="227f0-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-138">Not supported</span></span> | <span data-ttu-id="227f0-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="227f0-139">Files.ReadWrite</span></span> | <span data-ttu-id="227f0-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-140">Not supported</span></span> |
|<span data-ttu-id="227f0-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="227f0-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="227f0-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227f0-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="227f0-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-143">Not supported</span></span> | <span data-ttu-id="227f0-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227f0-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="227f0-145">evento</span><span class="sxs-lookup"><span data-stu-id="227f0-145">event</span></span>](../resources/event.md) | <span data-ttu-id="227f0-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-146">Calendars.Read</span></span> | <span data-ttu-id="227f0-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-147">Calendars.Read</span></span> | <span data-ttu-id="227f0-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-148">Calendars.Read</span></span> |
|[<span data-ttu-id="227f0-149">grupo</span><span class="sxs-lookup"><span data-stu-id="227f0-149">group</span></span>](../resources/group.md) | <span data-ttu-id="227f0-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-150">Group.Read.All</span></span> | <span data-ttu-id="227f0-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-151">Not supported</span></span> | <span data-ttu-id="227f0-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-152">Group.Read.All</span></span> |
|[<span data-ttu-id="227f0-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="227f0-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="227f0-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-154">Group.Read.All</span></span> | <span data-ttu-id="227f0-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-155">Not supported</span></span> | <span data-ttu-id="227f0-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-156">Not supported</span></span> |
|[<span data-ttu-id="227f0-157">list</span><span class="sxs-lookup"><span data-stu-id="227f0-157">list</span></span>](../resources/list.md) | <span data-ttu-id="227f0-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227f0-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="227f0-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-159">Not supported</span></span> | <span data-ttu-id="227f0-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227f0-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="227f0-161">message</span><span class="sxs-lookup"><span data-stu-id="227f0-161">message</span></span>](../resources/message.md) | <span data-ttu-id="227f0-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="227f0-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="227f0-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="227f0-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="227f0-165">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="227f0-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="227f0-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227f0-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="227f0-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="227f0-167">Not supported</span></span> | <span data-ttu-id="227f0-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227f0-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="227f0-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="227f0-169">user</span></span>](../resources/user.md) | <span data-ttu-id="227f0-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-170">User.Read.All</span></span> | <span data-ttu-id="227f0-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-171">User.Read.All</span></span> | <span data-ttu-id="227f0-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="227f0-172">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="227f0-173">chatMessage</span><span class="sxs-lookup"><span data-stu-id="227f0-173">chatMessage</span></span>

<span data-ttu-id="227f0-174">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="227f0-174">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="227f0-175">A criação da assinatura falhará se [encryptionCertificate](../resources/subscription.md) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="227f0-175">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="227f0-176">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="227f0-176">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="227f0-177">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="227f0-177">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="227f0-178">**Observação:** `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que têm as 
[licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="227f0-178">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="227f0-179">driveItem</span><span class="sxs-lookup"><span data-stu-id="227f0-179">driveItem</span></span>

<span data-ttu-id="227f0-180">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="227f0-180">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="227f0-181">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="227f0-181">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="227f0-182">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="227f0-182">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="227f0-183">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="227f0-183">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="227f0-184">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="227f0-184">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="227f0-185">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="227f0-185">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="227f0-186">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="227f0-186">contact, event, and message</span></span>

<span data-ttu-id="227f0-187">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="227f0-187">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="227f0-188">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="227f0-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="227f0-189">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="227f0-189">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="227f0-190">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="227f0-190">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="227f0-191">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas_compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="227f0-191">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="227f0-192">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="227f0-192">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="227f0-193">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não**suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="227f0-193">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="227f0-194">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="227f0-194">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="227f0-195">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="227f0-195">Request headers</span></span>

| <span data-ttu-id="227f0-196">Nome</span><span class="sxs-lookup"><span data-stu-id="227f0-196">Name</span></span>       | <span data-ttu-id="227f0-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="227f0-197">Type</span></span> | <span data-ttu-id="227f0-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="227f0-198">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="227f0-199">Autorização</span><span class="sxs-lookup"><span data-stu-id="227f0-199">Authorization</span></span>  | <span data-ttu-id="227f0-200">string</span><span class="sxs-lookup"><span data-stu-id="227f0-200">string</span></span>  | <span data-ttu-id="227f0-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227f0-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="227f0-203">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="227f0-203">Request body</span></span>

<span data-ttu-id="227f0-204">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="227f0-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="227f0-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="227f0-205">Response</span></span>

<span data-ttu-id="227f0-206">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="227f0-206">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="227f0-207">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="227f0-207">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="227f0-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="227f0-208">Example</span></span>

##### <a name="request"></a><span data-ttu-id="227f0-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="227f0-209">Request</span></span>

<span data-ttu-id="227f0-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="227f0-210">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="227f0-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="227f0-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="227f0-212">C#</span><span class="sxs-lookup"><span data-stu-id="227f0-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="227f0-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="227f0-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="227f0-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="227f0-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="227f0-215">Java</span><span class="sxs-lookup"><span data-stu-id="227f0-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="227f0-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="227f0-216">Response</span></span>

<span data-ttu-id="227f0-217">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="227f0-217">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

