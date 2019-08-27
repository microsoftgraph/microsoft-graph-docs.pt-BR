---
title: Obter conversationMember
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a1c4b522a828fcf08fe3b6385f6074aec4497b2a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633318"
---
# <a name="get-conversationmember"></a><span data-ttu-id="d2924-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="d2924-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2924-104">Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="d2924-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2924-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2924-105">Permissions</span></span>

<span data-ttu-id="d2924-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2924-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2924-108">Permission Type</span></span>|<span data-ttu-id="d2924-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2924-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="d2924-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2924-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d2924-111">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="d2924-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="d2924-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2924-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="d2924-113">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="d2924-113">For **channel** resource:</span></span><br/><span data-ttu-id="d2924-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2924-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="d2924-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2924-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2924-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d2924-116">Not supported</span></span>|
|<span data-ttu-id="d2924-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2924-117">Application</span></span>| <span data-ttu-id="d2924-118">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="d2924-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="d2924-119">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2924-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="d2924-120">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="d2924-120">For **channel** resource:</span></span><br/><span data-ttu-id="d2924-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2924-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2924-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2924-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2924-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2924-123">Optional query parameters</span></span>

<span data-ttu-id="d2924-124">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2924-124">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2924-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2924-125">Request headers</span></span>

| <span data-ttu-id="d2924-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2924-126">Header</span></span>       | <span data-ttu-id="d2924-127">Valor</span><span class="sxs-lookup"><span data-stu-id="d2924-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2924-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2924-128">Authorization</span></span>  | <span data-ttu-id="d2924-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2924-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2924-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2924-131">Request body</span></span>

<span data-ttu-id="d2924-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2924-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2924-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2924-133">Response</span></span>

<span data-ttu-id="d2924-134">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2924-134">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2924-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2924-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2924-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2924-136">Request</span></span>

<span data-ttu-id="d2924-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2924-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2924-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2924-138">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2924-139">C#</span><span class="sxs-lookup"><span data-stu-id="d2924-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2924-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2924-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2924-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2924-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d2924-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2924-142">Response</span></span>

<span data-ttu-id="d2924-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2924-143">Here is an example of the response.</span></span>

><span data-ttu-id="d2924-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2924-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "display-name-value"
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
