---
title: Obter conversationMember
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ae09333c14aeada9603483516746c2cfafbc3a98
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863005"
---
# <a name="get-conversationmember"></a><span data-ttu-id="5189f-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="5189f-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5189f-104">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="5189f-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5189f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5189f-105">Permissions</span></span>

<span data-ttu-id="5189f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5189f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5189f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5189f-108">Permission Type</span></span>|<span data-ttu-id="5189f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5189f-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5189f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5189f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5189f-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5189f-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="5189f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5189f-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5189f-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5189f-113">Not supported</span></span>|
|<span data-ttu-id="5189f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5189f-114">Application</span></span> |<span data-ttu-id="5189f-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5189f-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5189f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5189f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5189f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5189f-117">Optional query parameters</span></span>

<span data-ttu-id="5189f-118">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5189f-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5189f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5189f-119">Request headers</span></span>

| <span data-ttu-id="5189f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5189f-120">Header</span></span>       | <span data-ttu-id="5189f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5189f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5189f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5189f-122">Authorization</span></span>  | <span data-ttu-id="5189f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5189f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5189f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5189f-125">Request body</span></span>

<span data-ttu-id="5189f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5189f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5189f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5189f-127">Response</span></span>

<span data-ttu-id="5189f-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5189f-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5189f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5189f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5189f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5189f-130">Request</span></span>

<span data-ttu-id="5189f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5189f-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5189f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5189f-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5189f-133">C#</span><span class="sxs-lookup"><span data-stu-id="5189f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5189f-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="5189f-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5189f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5189f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5189f-136">Java</span><span class="sxs-lookup"><span data-stu-id="5189f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5189f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5189f-137">Response</span></span>

<span data-ttu-id="5189f-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5189f-138">Here is an example of the response.</span></span> 

><span data-ttu-id="5189f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5189f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
