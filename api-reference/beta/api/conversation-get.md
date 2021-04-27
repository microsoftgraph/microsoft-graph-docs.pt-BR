---
title: Obter conversation
description: Recupera as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 937ad1e434f01716fbbd6c5634fbd60716f2a2c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047039"
---
# <a name="get-conversation"></a><span data-ttu-id="4b171-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="4b171-103">Get conversation</span></span>

<span data-ttu-id="4b171-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b171-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b171-105">Recupera as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="4b171-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b171-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b171-106">Permissions</span></span>
<span data-ttu-id="4b171-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b171-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b171-109">Permission type</span></span>      | <span data-ttu-id="4b171-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b171-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b171-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b171-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b171-112">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b171-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="4b171-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b171-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b171-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b171-114">Not supported.</span></span>    |
|<span data-ttu-id="4b171-115">Application</span><span class="sxs-lookup"><span data-stu-id="4b171-115">Application</span></span> | <span data-ttu-id="4b171-116">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b171-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b171-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b171-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b171-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4b171-118">Optional query parameters</span></span>
<span data-ttu-id="4b171-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4b171-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4b171-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b171-120">Request headers</span></span>
| <span data-ttu-id="4b171-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b171-121">Header</span></span>       | <span data-ttu-id="4b171-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b171-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b171-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b171-123">Authorization</span></span>  | <span data-ttu-id="4b171-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b171-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b171-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b171-126">Request body</span></span>
<span data-ttu-id="4b171-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b171-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b171-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b171-128">Response</span></span>

<span data-ttu-id="4b171-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b171-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b171-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b171-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b171-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b171-131">Request</span></span>
<span data-ttu-id="4b171-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b171-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b171-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b171-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="4b171-134">C#</span><span class="sxs-lookup"><span data-stu-id="4b171-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b171-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b171-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b171-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b171-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b171-137">Java</span><span class="sxs-lookup"><span data-stu-id="4b171-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4b171-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b171-138">Response</span></span>
<span data-ttu-id="4b171-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b171-139">Here is an example of the response.</span></span> <span data-ttu-id="4b171-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b171-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
