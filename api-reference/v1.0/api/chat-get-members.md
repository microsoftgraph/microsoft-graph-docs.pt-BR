---
title: Obtenha o conversationMember em um bate-papo.
description: Recuperar um membro de um bate-papo.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 19dd93d0316e818b16afa2035ab9614f38aa269f
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696139"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="ee30a-103">Obtenha o conversationMember em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="ee30a-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="ee30a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee30a-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="ee30a-105">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="ee30a-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="ee30a-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="ee30a-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="ee30a-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="ee30a-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="ee30a-p102">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros sejam apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="ee30a-p102">The membership results could map to users from different tenants, as indicated in the response, in the future. The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee30a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee30a-110">Permissions</span></span>

<span data-ttu-id="ee30a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee30a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee30a-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee30a-113">Permission Type</span></span>|<span data-ttu-id="ee30a-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee30a-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ee30a-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee30a-115">Delegated (work or school account)</span></span>| <span data-ttu-id="ee30a-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee30a-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="ee30a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee30a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee30a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee30a-118">Not supported.</span></span>|
|<span data-ttu-id="ee30a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee30a-119">Application</span></span>| <span data-ttu-id="ee30a-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ee30a-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span></span> |

> <span data-ttu-id="ee30a-121">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ee30a-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="ee30a-122">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee30a-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ee30a-123">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="ee30a-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ee30a-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee30a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id} | user-principal-name/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee30a-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee30a-125">Optional query parameters</span></span>

<span data-ttu-id="ee30a-126">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30a-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee30a-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30a-127">Request headers</span></span>

| <span data-ttu-id="ee30a-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee30a-128">Header</span></span>       | <span data-ttu-id="ee30a-129">Valor</span><span class="sxs-lookup"><span data-stu-id="ee30a-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ee30a-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee30a-130">Authorization</span></span>  | <span data-ttu-id="ee30a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee30a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee30a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30a-133">Request body</span></span>

<span data-ttu-id="ee30a-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee30a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee30a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee30a-135">Response</span></span>

<span data-ttu-id="ee30a-136">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30a-136">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee30a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee30a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee30a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30a-138">Request</span></span>

<span data-ttu-id="ee30a-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee30a-139">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="ee30a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee30a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==
```
# <a name="c"></a>[<span data-ttu-id="ee30a-141">C#</span><span class="sxs-lookup"><span data-stu-id="ee30a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee30a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee30a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee30a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee30a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee30a-144">Java</span><span class="sxs-lookup"><span data-stu-id="ee30a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee30a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee30a-145">Response</span></span>

<span data-ttu-id="ee30a-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30a-146">Here is an example of the response.</span></span>

<!-- 
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ab8577894a63548969c5c92bb9c80c5e1%40thread.v2')/members/$entity",
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==",
    "roles": [
        "owner"
    ],
    "displayName": "John Doe",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "userId": "2c8d2b5c-1849-4066-b57d-e7a0e9e44ec8",
    "email": "johndoe@contoso.onmicrosoft.com",
    "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


