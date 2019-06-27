---
title: Obter conversation
description: Recupera as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 2435f192072d023f06cdc832f299e2a44ccdeeba
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273819"
---
# <a name="get-conversation"></a><span data-ttu-id="3a6b6-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="3a6b6-103">Get conversation</span></span>

<span data-ttu-id="3a6b6-104">Recupera as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a6b6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a6b6-105">Permissions</span></span>
<span data-ttu-id="3a6b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a6b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a6b6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a6b6-108">Permission type</span></span>      | <span data-ttu-id="3a6b6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a6b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a6b6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a6b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a6b6-111">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="3a6b6-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="3a6b6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a6b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a6b6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-113">Not supported.</span></span>    |
|<span data-ttu-id="3a6b6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a6b6-114">Application</span></span> | <span data-ttu-id="3a6b6-115">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="3a6b6-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a6b6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a6b6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a6b6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a6b6-117">Optional query parameters</span></span>
<span data-ttu-id="3a6b6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3a6b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a6b6-119">Request headers</span></span>
| <span data-ttu-id="3a6b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a6b6-120">Header</span></span>       | <span data-ttu-id="3a6b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3a6b6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a6b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a6b6-122">Authorization</span></span>  | <span data-ttu-id="3a6b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a6b6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a6b6-125">Request body</span></span>
<span data-ttu-id="3a6b6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a6b6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a6b6-127">Response</span></span>

<span data-ttu-id="3a6b6-128">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a6b6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a6b6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a6b6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a6b6-130">Request</span></span>
<span data-ttu-id="3a6b6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="3a6b6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a6b6-132">Response</span></span>
<span data-ttu-id="3a6b6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a6b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3a6b6-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3a6b6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3a6b6-137">C#</span><span class="sxs-lookup"><span data-stu-id="3a6b6-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a6b6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a6b6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3a6b6-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3a6b6-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversation-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
