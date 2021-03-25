---
title: Listar conversationMembers
description: Recupere a lista do bate-papo ou de membros do canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f065a9cc508e557cc57c7c3658b9816baf47b1d3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202344"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="3a249-103">Listar conversationMembers</span><span class="sxs-lookup"><span data-stu-id="3a249-103">List conversationMembers</span></span>

<span data-ttu-id="3a249-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a249-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a249-105">Listar todos os [membros da conversa](../resources/conversationmember.md) de um [chat](../resources/chatmessage.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="3a249-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3a249-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="3a249-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="3a249-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="3a249-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="3a249-108">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros sejam apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="3a249-108">The membership results could map to users from different tenants, as indicated in the response, in the future.The client should not assume that all members are from the current tenant only.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="3a249-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="3a249-109">Permissions</span></span>

<span data-ttu-id="3a249-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a249-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a249-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a249-112">Permission Type</span></span>|<span data-ttu-id="3a249-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a249-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3a249-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a249-114">Delegated (work or school account)</span></span>| <span data-ttu-id="3a249-115">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a249-115">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="3a249-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a249-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a249-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a249-117">Not supported.</span></span>|
|<span data-ttu-id="3a249-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a249-118">Application</span></span>| <span data-ttu-id="3a249-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a249-119">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="3a249-120">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3a249-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="3a249-121">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="3a249-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="3a249-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a249-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a249-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a249-123">Optional query parameters</span></span>

<span data-ttu-id="3a249-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a249-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a249-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a249-125">Request headers</span></span>

| <span data-ttu-id="3a249-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a249-126">Header</span></span>       | <span data-ttu-id="3a249-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3a249-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a249-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a249-128">Authorization</span></span>  | <span data-ttu-id="3a249-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a249-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a249-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a249-131">Request body</span></span>

<span data-ttu-id="3a249-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a249-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a249-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a249-133">Response</span></span>

<span data-ttu-id="3a249-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a249-134">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a249-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a249-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a249-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a249-136">Request</span></span>

<span data-ttu-id="3a249-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a249-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a249-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a249-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="3a249-139">C#</span><span class="sxs-lookup"><span data-stu-id="3a249-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a249-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a249-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a249-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a249-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a249-142">Java</span><span class="sxs-lookup"><span data-stu-id="3a249-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a249-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a249-143">Response</span></span>

<span data-ttu-id="3a249-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a249-144">The following is an example of the response.</span></span>

><span data-ttu-id="3a249-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a249-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
