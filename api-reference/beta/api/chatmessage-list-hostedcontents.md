---
title: Listar hostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ca2d61bd5362f4c0c5ec877fb2895ea4e175b8b
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695998"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="1a203-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="1a203-103">List hostedContents</span></span>

<span data-ttu-id="1a203-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a203-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a203-105">Recupere a lista de [objetos chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="1a203-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span> <span data-ttu-id="1a203-106">Essa API lista apenas os objetos de conteúdo hospedados.</span><span class="sxs-lookup"><span data-stu-id="1a203-106">This API only lists the hosted content objects.</span></span> <span data-ttu-id="1a203-107">Para obter os bytes de conteúdo, consulte [get chatmessage hosted content](chatmessagehostedcontent-get.md)</span><span class="sxs-lookup"><span data-stu-id="1a203-107">To get the content bytes, see [get chatmessage hosted content](chatmessagehostedcontent-get.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="1a203-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a203-108">Permissions</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="1a203-109">Permissões para o canal</span><span class="sxs-lookup"><span data-stu-id="1a203-109">Permissions for channel</span></span>

| <span data-ttu-id="1a203-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a203-110">Permission type</span></span>                        | <span data-ttu-id="1a203-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a203-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="1a203-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a203-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1a203-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="1a203-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="1a203-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a203-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a203-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a203-115">Not supported.</span></span>|
|<span data-ttu-id="1a203-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a203-116">Application</span></span>| <span data-ttu-id="1a203-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a203-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="1a203-118">Permissões para o chat</span><span class="sxs-lookup"><span data-stu-id="1a203-118">Permissions for chat</span></span>

| <span data-ttu-id="1a203-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a203-119">Permission type</span></span>                        | <span data-ttu-id="1a203-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a203-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="1a203-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a203-121">Delegated (work or school account)</span></span>| <span data-ttu-id="1a203-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a203-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="1a203-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a203-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a203-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a203-124">Not supported.</span></span>|
|<span data-ttu-id="1a203-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a203-125">Application</span></span>| <span data-ttu-id="1a203-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a203-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="1a203-127">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1a203-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="1a203-128">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1a203-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="1a203-129">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="1a203-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="1a203-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a203-130">HTTP request</span></span>

<span data-ttu-id="1a203-131">**Obter hostedContents em uma mensagem de canal**</span><span class="sxs-lookup"><span data-stu-id="1a203-131">**Get hostedContents in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents
```

<span data-ttu-id="1a203-132">**Obter hostedContents em uma mensagem de chat**</span><span class="sxs-lookup"><span data-stu-id="1a203-132">**Get hostedContents in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a203-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a203-133">Optional query parameters</span></span>

<span data-ttu-id="1a203-134">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a203-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a203-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a203-135">Request headers</span></span>

| <span data-ttu-id="1a203-136">Nome</span><span class="sxs-lookup"><span data-stu-id="1a203-136">Name</span></span>      |<span data-ttu-id="1a203-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a203-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a203-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a203-138">Authorization</span></span> | <span data-ttu-id="1a203-139">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1a203-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a203-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a203-140">Request body</span></span>

<span data-ttu-id="1a203-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a203-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a203-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a203-142">Response</span></span>

<span data-ttu-id="1a203-143">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a203-143">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a203-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a203-144">Examples</span></span>

### <a name="example-1-list-hosted-content-for-a-channel-message"></a><span data-ttu-id="1a203-145">Exemplo 1: Listar conteúdo hospedado para uma mensagem de canal</span><span class="sxs-lookup"><span data-stu-id="1a203-145">Example 1: List hosted content for a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="1a203-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a203-146">Request</span></span>

<span data-ttu-id="1a203-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a203-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1a203-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a203-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="1a203-149">C#</span><span class="sxs-lookup"><span data-stu-id="1a203-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschannelmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a203-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a203-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschannelmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a203-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a203-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschannelmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a203-152">Java</span><span class="sxs-lookup"><span data-stu-id="1a203-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschannelmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a203-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a203-153">Response</span></span>

<span data-ttu-id="1a203-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a203-154">The following is an example of the response.</span></span>

> <span data-ttu-id="1a203-155">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="1a203-155">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/hostedContents",
    "@odata.count": 2,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        },
        {
            "id": "aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

### <a name="example-2-list-hosted-content-for-reply-to-a-channel-message"></a><span data-ttu-id="1a203-156">Exemplo 2: Listar conteúdo hospedado para resposta a uma mensagem de canal</span><span class="sxs-lookup"><span data-stu-id="1a203-156">Example 2: List hosted content for reply to a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="1a203-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a203-157">Request</span></span>

<span data-ttu-id="1a203-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a203-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1a203-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a203-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies/1616963389737/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="1a203-160">C#</span><span class="sxs-lookup"><span data-stu-id="1a203-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschannelmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a203-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a203-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschannelmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a203-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a203-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschannelmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a203-163">Java</span><span class="sxs-lookup"><span data-stu-id="1a203-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschannelmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a203-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a203-164">Response</span></span>

<span data-ttu-id="1a203-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a203-165">The following is an example of the response.</span></span>

> <span data-ttu-id="1a203-166">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="1a203-166">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/replies('1616963389737')/hostedContents",
    "@odata.count": 2,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kMy1hMDE3MmZiYjVkYzcxNGM4NWU5NDQwNWE5ZjNkNThmYyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMy1hMDE3MmZiYjVkYzcxNGM4NWU5NDQwNWE5ZjNkNThmYy92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        },
        {
            "id": "aWQ9eF8wLXd1cy1kOS03ZDlmOGVlMzk4ZGQ3YTZkMDdhMDg4OGI5ODZlNDdkYyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS03ZDlmOGVlMzk4ZGQ3YTZkMDdhMDg4OGI5ODZlNDdkYy92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

### <a name="example-2--list-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="1a203-167">Exemplo 2 : Listar conteúdo hospedado para mensagem em um chat</span><span class="sxs-lookup"><span data-stu-id="1a203-167">Example 2 : List hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="1a203-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a203-168">Request</span></span>

<span data-ttu-id="1a203-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a203-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1a203-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a203-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschatmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="1a203-171">C#</span><span class="sxs-lookup"><span data-stu-id="1a203-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschatmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a203-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a203-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschatmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a203-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a203-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschatmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a203-174">Java</span><span class="sxs-lookup"><span data-stu-id="1a203-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschatmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a203-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a203-175">Response</span></span>

<span data-ttu-id="1a203-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a203-176">The following is an example of the response.</span></span>

> <span data-ttu-id="1a203-177">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="1a203-177">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


