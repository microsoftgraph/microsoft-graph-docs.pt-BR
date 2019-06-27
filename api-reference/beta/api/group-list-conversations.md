---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6fe5d6e127f5fa33d9ff9ef87514ad74c992d7fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263228"
---
# <a name="list-conversations"></a><span data-ttu-id="3d716-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="3d716-103">List conversations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d716-104">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="3d716-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d716-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d716-105">Permissions</span></span>
<span data-ttu-id="3d716-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d716-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d716-108">Permission type</span></span>      | <span data-ttu-id="3d716-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d716-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d716-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d716-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d716-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d716-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d716-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d716-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d716-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d716-113">Not supported.</span></span>    |
|<span data-ttu-id="3d716-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d716-114">Application</span></span> | <span data-ttu-id="3d716-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d716-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d716-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d716-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d716-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d716-117">Optional query parameters</span></span>
<span data-ttu-id="3d716-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3d716-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d716-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d716-119">Request headers</span></span>
| <span data-ttu-id="3d716-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d716-120">Header</span></span>       | <span data-ttu-id="3d716-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3d716-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3d716-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d716-122">Authorization</span></span>  | <span data-ttu-id="3d716-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d716-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3d716-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d716-125">Request body</span></span>
<span data-ttu-id="3d716-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d716-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d716-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d716-127">Response</span></span>
<span data-ttu-id="3d716-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d716-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d716-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d716-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3d716-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d716-130">Request</span></span>
<span data-ttu-id="3d716-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d716-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="3d716-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d716-132">Response</span></span>
<span data-ttu-id="3d716-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d716-133">The following is an example of the response.</span></span>
><span data-ttu-id="3d716-134">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3d716-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3d716-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d716-135">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d716-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3d716-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d716-137">C#</span><span class="sxs-lookup"><span data-stu-id="3d716-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversations-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d716-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d716-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversations-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d716-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3d716-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversations-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
