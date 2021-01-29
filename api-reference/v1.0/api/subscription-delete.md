---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b4b05d659453ef0867d60f3d43d137f4b697874
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034069"
---
# <a name="delete-subscription"></a><span data-ttu-id="6058c-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="6058c-103">Delete subscription</span></span>

<span data-ttu-id="6058c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6058c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6058c-105">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="6058c-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6058c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6058c-106">Permissions</span></span>

<span data-ttu-id="6058c-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="6058c-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6058c-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6058c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6058c-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-109">Supported resource</span></span> | <span data-ttu-id="6058c-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6058c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6058c-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6058c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6058c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6058c-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6058c-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="6058c-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6058c-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="6058c-114">Not supported</span></span> | <span data-ttu-id="6058c-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="6058c-115">Not supported</span></span> | <span data-ttu-id="6058c-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="6058c-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6058c-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6058c-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-118">Not supported</span></span> | <span data-ttu-id="6058c-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-119">Not supported</span></span> |  <span data-ttu-id="6058c-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6058c-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="6058c-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6058c-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-122">Not supported</span></span> | <span data-ttu-id="6058c-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-123">Not supported</span></span> | <span data-ttu-id="6058c-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6058c-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6058c-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6058c-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-126">Not supported</span></span> | <span data-ttu-id="6058c-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-127">Not supported</span></span> | <span data-ttu-id="6058c-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="6058c-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="6058c-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6058c-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-130">Not supported</span></span> | <span data-ttu-id="6058c-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-131">Not supported</span></span> | <span data-ttu-id="6058c-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6058c-133">contato</span><span class="sxs-lookup"><span data-stu-id="6058c-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6058c-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-134">Contacts.Read</span></span> | <span data-ttu-id="6058c-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-135">Contacts.Read</span></span> | <span data-ttu-id="6058c-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-136">Contacts.Read</span></span> |
|<span data-ttu-id="6058c-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="6058c-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6058c-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-138">Not supported</span></span> | <span data-ttu-id="6058c-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6058c-139">Files.ReadWrite</span></span> | <span data-ttu-id="6058c-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-140">Not supported</span></span> |
|<span data-ttu-id="6058c-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="6058c-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6058c-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6058c-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="6058c-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-143">Not supported</span></span> | <span data-ttu-id="6058c-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6058c-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6058c-145">evento</span><span class="sxs-lookup"><span data-stu-id="6058c-145">event</span></span>](../resources/event.md) | <span data-ttu-id="6058c-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-146">Calendars.Read</span></span> | <span data-ttu-id="6058c-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-147">Calendars.Read</span></span> | <span data-ttu-id="6058c-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-148">Calendars.Read</span></span> |
|[<span data-ttu-id="6058c-149">grupo</span><span class="sxs-lookup"><span data-stu-id="6058c-149">group</span></span>](../resources/group.md) | <span data-ttu-id="6058c-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-150">Group.Read.All</span></span> | <span data-ttu-id="6058c-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-151">Not supported</span></span> | <span data-ttu-id="6058c-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-152">Group.Read.All</span></span> |
|[<span data-ttu-id="6058c-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="6058c-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6058c-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-154">Group.Read.All</span></span> | <span data-ttu-id="6058c-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-155">Not supported</span></span> | <span data-ttu-id="6058c-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-156">Not supported</span></span> |
|[<span data-ttu-id="6058c-157">list</span><span class="sxs-lookup"><span data-stu-id="6058c-157">list</span></span>](../resources/list.md) | <span data-ttu-id="6058c-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6058c-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6058c-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-159">Not supported</span></span> | <span data-ttu-id="6058c-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6058c-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6058c-161">message</span><span class="sxs-lookup"><span data-stu-id="6058c-161">message</span></span>](../resources/message.md) | <span data-ttu-id="6058c-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6058c-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6058c-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6058c-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6058c-165">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="6058c-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6058c-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6058c-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6058c-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6058c-167">Not supported</span></span> | <span data-ttu-id="6058c-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6058c-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6058c-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="6058c-169">user</span></span>](../resources/user.md) | <span data-ttu-id="6058c-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-170">User.Read.All</span></span> | <span data-ttu-id="6058c-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-171">User.Read.All</span></span> | <span data-ttu-id="6058c-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6058c-172">User.Read.All</span></span> |

> <span data-ttu-id="6058c-173">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6058c-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="6058c-174">driveItem</span><span class="sxs-lookup"><span data-stu-id="6058c-174">driveItem</span></span>

<span data-ttu-id="6058c-175">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6058c-175">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6058c-176">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="6058c-176">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6058c-177">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="6058c-177">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6058c-178">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="6058c-178">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6058c-179">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="6058c-179">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6058c-180">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="6058c-180">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6058c-181">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="6058c-181">contact, event, and message</span></span>

<span data-ttu-id="6058c-182">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6058c-182">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6058c-183">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="6058c-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6058c-184">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="6058c-184">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6058c-185">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="6058c-185">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6058c-186">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="6058c-186">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6058c-187">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="6058c-187">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6058c-188">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="6058c-188">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="6058c-189">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6058c-189">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="6058c-190">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6058c-190">Request headers</span></span>

| <span data-ttu-id="6058c-191">Nome</span><span class="sxs-lookup"><span data-stu-id="6058c-191">Name</span></span>       | <span data-ttu-id="6058c-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="6058c-192">Type</span></span> | <span data-ttu-id="6058c-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="6058c-193">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6058c-194">Autorização</span><span class="sxs-lookup"><span data-stu-id="6058c-194">Authorization</span></span>  | <span data-ttu-id="6058c-195">string</span><span class="sxs-lookup"><span data-stu-id="6058c-195">string</span></span>  | <span data-ttu-id="6058c-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6058c-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6058c-198">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6058c-198">Request body</span></span>

<span data-ttu-id="6058c-199">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6058c-199">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6058c-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="6058c-200">Response</span></span>

<span data-ttu-id="6058c-201">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6058c-201">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="6058c-202">Para detalhes sobre como os erros são retornados, confira [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="6058c-202">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6058c-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6058c-203">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6058c-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6058c-204">Request</span></span>

<span data-ttu-id="6058c-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6058c-205">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6058c-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="6058c-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="6058c-207">C#</span><span class="sxs-lookup"><span data-stu-id="6058c-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6058c-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6058c-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6058c-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6058c-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6058c-210">Java</span><span class="sxs-lookup"><span data-stu-id="6058c-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6058c-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="6058c-211">Response</span></span>

<span data-ttu-id="6058c-212">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6058c-212">Here is an example of the response.</span></span>
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

