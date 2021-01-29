---
title: Obter assinatura
description: Recupere as propriedades e os relacionamentos da uma assinatura.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4550912f9f4392131e62cb26a3328698bf121c15
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034279"
---
# <a name="get-subscription"></a><span data-ttu-id="d62be-103">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="d62be-103">Get subscription</span></span>

<span data-ttu-id="d62be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d62be-105">Recupere as propriedades e os relacionamentos da uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d62be-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="d62be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d62be-106">Permissions</span></span>

<span data-ttu-id="d62be-107">Dependendo do recurso e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="d62be-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d62be-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d62be-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d62be-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-109">Supported resource</span></span> | <span data-ttu-id="d62be-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d62be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d62be-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d62be-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d62be-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d62be-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d62be-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="d62be-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="d62be-114">Incompatível</span><span class="sxs-lookup"><span data-stu-id="d62be-114">Not supported</span></span> | <span data-ttu-id="d62be-115">Incompatível</span><span class="sxs-lookup"><span data-stu-id="d62be-115">Not supported</span></span> | <span data-ttu-id="d62be-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="d62be-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d62be-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="d62be-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-118">Not supported</span></span> | <span data-ttu-id="d62be-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-119">Not supported</span></span> |  <span data-ttu-id="d62be-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d62be-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de canal na organização)</span><span class="sxs-lookup"><span data-stu-id="d62be-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="d62be-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-122">Not supported</span></span> | <span data-ttu-id="d62be-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-123">Not supported</span></span> | <span data-ttu-id="d62be-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d62be-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d62be-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="d62be-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-126">Not supported</span></span> | <span data-ttu-id="d62be-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-127">Not supported</span></span> | <span data-ttu-id="d62be-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="d62be-129">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- todas as mensagens de chat na organização)</span><span class="sxs-lookup"><span data-stu-id="d62be-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="d62be-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-130">Not supported</span></span> | <span data-ttu-id="d62be-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-131">Not supported</span></span> | <span data-ttu-id="d62be-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="d62be-133">contato</span><span class="sxs-lookup"><span data-stu-id="d62be-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d62be-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-134">Contacts.Read</span></span> | <span data-ttu-id="d62be-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-135">Contacts.Read</span></span> | <span data-ttu-id="d62be-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-136">Contacts.Read</span></span> |
|<span data-ttu-id="d62be-137">[driveItem](../resources/driveitem.md) (OneDrive pessoal de um usuário)</span><span class="sxs-lookup"><span data-stu-id="d62be-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d62be-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-138">Not supported</span></span> | <span data-ttu-id="d62be-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d62be-139">Files.ReadWrite</span></span> | <span data-ttu-id="d62be-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-140">Not supported</span></span> |
|<span data-ttu-id="d62be-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="d62be-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d62be-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62be-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="d62be-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-143">Not supported</span></span> | <span data-ttu-id="d62be-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62be-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d62be-145">evento</span><span class="sxs-lookup"><span data-stu-id="d62be-145">event</span></span>](../resources/event.md) | <span data-ttu-id="d62be-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-146">Calendars.Read</span></span> | <span data-ttu-id="d62be-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-147">Calendars.Read</span></span> | <span data-ttu-id="d62be-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-148">Calendars.Read</span></span> |
|[<span data-ttu-id="d62be-149">grupo</span><span class="sxs-lookup"><span data-stu-id="d62be-149">group</span></span>](../resources/group.md) | <span data-ttu-id="d62be-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-150">Group.Read.All</span></span> | <span data-ttu-id="d62be-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-151">Not supported</span></span> | <span data-ttu-id="d62be-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-152">Group.Read.All</span></span> |
|[<span data-ttu-id="d62be-153">conversa em grupo</span><span class="sxs-lookup"><span data-stu-id="d62be-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d62be-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-154">Group.Read.All</span></span> | <span data-ttu-id="d62be-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-155">Not supported</span></span> | <span data-ttu-id="d62be-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-156">Not supported</span></span> |
|[<span data-ttu-id="d62be-157">list</span><span class="sxs-lookup"><span data-stu-id="d62be-157">list</span></span>](../resources/list.md) | <span data-ttu-id="d62be-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62be-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d62be-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-159">Not supported</span></span> | <span data-ttu-id="d62be-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62be-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d62be-161">message</span><span class="sxs-lookup"><span data-stu-id="d62be-161">message</span></span>](../resources/message.md) | <span data-ttu-id="d62be-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d62be-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d62be-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d62be-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="d62be-165">alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="d62be-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="d62be-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62be-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d62be-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d62be-167">Not supported</span></span> | <span data-ttu-id="d62be-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62be-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d62be-169">Usuário</span><span class="sxs-lookup"><span data-stu-id="d62be-169">user</span></span>](../resources/user.md) | <span data-ttu-id="d62be-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-170">User.Read.All</span></span> | <span data-ttu-id="d62be-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-171">User.Read.All</span></span> | <span data-ttu-id="d62be-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d62be-172">User.Read.All</span></span> |

> <span data-ttu-id="d62be-173">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d62be-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="d62be-174">driveItem</span><span class="sxs-lookup"><span data-stu-id="d62be-174">driveItem</span></span>

<span data-ttu-id="d62be-175">As limitações adicionais se aplicam aos itens do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d62be-175">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="d62be-176">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="d62be-176">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="d62be-177">No OneDrive pessoal, você pode se inscrever em qualquer pasta raiz ou qualquer subpasta da unidade.</span><span class="sxs-lookup"><span data-stu-id="d62be-177">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d62be-178">No OneDrive for Business, você pode assinar somente a pasta raiz.</span><span class="sxs-lookup"><span data-stu-id="d62be-178">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d62be-179">As notificações de alteração são enviadas para os tipos de alterações solicitados na pasta assinada ou em qualquer arquivo, pasta ou outras instâncias **driveItem** em sua hierarquia.</span><span class="sxs-lookup"><span data-stu-id="d62be-179">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="d62be-180">Você não pode inscrever as instâncias **unidade** ou **driveItem** que não sejam pastas, como arquivos individuais.</span><span class="sxs-lookup"><span data-stu-id="d62be-180">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="d62be-181">contato, evento e mensagem</span><span class="sxs-lookup"><span data-stu-id="d62be-181">contact, event, and message</span></span>

<span data-ttu-id="d62be-182">As limitações adicionais se aplicam aos itens do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d62be-182">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="d62be-183">As limitações se aplicam para criação e gerenciamento de assinaturas (receber, atualizar e excluir assinaturas).</span><span class="sxs-lookup"><span data-stu-id="d62be-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="d62be-184">A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d62be-184">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d62be-185">Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="d62be-185">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d62be-186">Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:</span><span class="sxs-lookup"><span data-stu-id="d62be-186">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d62be-187">Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="d62be-187">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d62be-188">Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="d62be-188">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="d62be-189">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d62be-189">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d62be-190">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d62be-190">Optional query parameters</span></span>

<span data-ttu-id="d62be-191">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d62be-191">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d62be-192">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d62be-192">Request headers</span></span>

| <span data-ttu-id="d62be-193">Nome</span><span class="sxs-lookup"><span data-stu-id="d62be-193">Name</span></span>       | <span data-ttu-id="d62be-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="d62be-194">Type</span></span> | <span data-ttu-id="d62be-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="d62be-195">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d62be-196">Autorização</span><span class="sxs-lookup"><span data-stu-id="d62be-196">Authorization</span></span>  | <span data-ttu-id="d62be-197">string</span><span class="sxs-lookup"><span data-stu-id="d62be-197">string</span></span>  | <span data-ttu-id="d62be-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d62be-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d62be-200">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d62be-200">Request body</span></span>

<span data-ttu-id="d62be-201">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d62be-201">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d62be-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="d62be-202">Response</span></span>

<span data-ttu-id="d62be-203">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d62be-203">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d62be-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d62be-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d62be-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d62be-205">Request</span></span>

<span data-ttu-id="d62be-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d62be-206">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d62be-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="d62be-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="d62be-208">C#</span><span class="sxs-lookup"><span data-stu-id="d62be-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d62be-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d62be-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d62be-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d62be-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d62be-211">Java</span><span class="sxs-lookup"><span data-stu-id="d62be-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d62be-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="d62be-212">Response</span></span>

<span data-ttu-id="d62be-213">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d62be-213">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
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
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

