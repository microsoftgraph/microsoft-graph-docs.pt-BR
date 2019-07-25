---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: cb6d6479a1bc3aba8f2d53327f88a9abdf12440a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858481"
---
# <a name="list-conversations"></a><span data-ttu-id="1b78e-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="1b78e-103">List conversations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b78e-104">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="1b78e-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b78e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b78e-105">Permissions</span></span>
<span data-ttu-id="1b78e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b78e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b78e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b78e-108">Permission type</span></span>      | <span data-ttu-id="1b78e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b78e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b78e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b78e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b78e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b78e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b78e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b78e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b78e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b78e-113">Not supported.</span></span>    |
|<span data-ttu-id="1b78e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b78e-114">Application</span></span> | <span data-ttu-id="1b78e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b78e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b78e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b78e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b78e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b78e-117">Optional query parameters</span></span>
<span data-ttu-id="1b78e-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b78e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b78e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b78e-119">Request headers</span></span>
| <span data-ttu-id="1b78e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b78e-120">Header</span></span>       | <span data-ttu-id="1b78e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1b78e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b78e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b78e-122">Authorization</span></span>  | <span data-ttu-id="1b78e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b78e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b78e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b78e-125">Request body</span></span>
<span data-ttu-id="1b78e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b78e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b78e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b78e-127">Response</span></span>
<span data-ttu-id="1b78e-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b78e-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b78e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b78e-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1b78e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b78e-130">Request</span></span>
<span data-ttu-id="1b78e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b78e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b78e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b78e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b78e-133">C#</span><span class="sxs-lookup"><span data-stu-id="1b78e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b78e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b78e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b78e-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1b78e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b78e-136">Java</span><span class="sxs-lookup"><span data-stu-id="1b78e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b78e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b78e-137">Response</span></span>
<span data-ttu-id="1b78e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b78e-138">The following is an example of the response.</span></span>
><span data-ttu-id="1b78e-139">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b78e-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1b78e-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b78e-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
