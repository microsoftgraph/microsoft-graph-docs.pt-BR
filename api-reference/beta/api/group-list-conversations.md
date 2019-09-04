---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 309d665cfe7beee9a697e9c79ef7aec4b4fb65e4
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720575"
---
# <a name="list-conversations"></a><span data-ttu-id="916c5-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="916c5-103">List conversations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="916c5-104">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="916c5-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="916c5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="916c5-105">Permissions</span></span>
<span data-ttu-id="916c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="916c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="916c5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="916c5-108">Permission type</span></span>      | <span data-ttu-id="916c5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="916c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="916c5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="916c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="916c5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="916c5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="916c5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="916c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="916c5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916c5-113">Not supported.</span></span>    |
|<span data-ttu-id="916c5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="916c5-114">Application</span></span> | <span data-ttu-id="916c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916c5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="916c5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="916c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="916c5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="916c5-117">Optional query parameters</span></span>
<span data-ttu-id="916c5-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="916c5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="916c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="916c5-119">Request headers</span></span>
| <span data-ttu-id="916c5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="916c5-120">Header</span></span>       | <span data-ttu-id="916c5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="916c5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="916c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="916c5-122">Authorization</span></span>  | <span data-ttu-id="916c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="916c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="916c5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="916c5-125">Request body</span></span>
<span data-ttu-id="916c5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="916c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="916c5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="916c5-127">Response</span></span>
<span data-ttu-id="916c5-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916c5-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916c5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="916c5-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="916c5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="916c5-130">Request</span></span>
<span data-ttu-id="916c5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="916c5-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="916c5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="916c5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="916c5-133">C#</span><span class="sxs-lookup"><span data-stu-id="916c5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="916c5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="916c5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="916c5-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="916c5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="916c5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="916c5-136">Response</span></span>
<span data-ttu-id="916c5-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="916c5-137">The following is an example of the response.</span></span>
><span data-ttu-id="916c5-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="916c5-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="916c5-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="916c5-139">All the properties will be returned from an actual call.</span></span>
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
