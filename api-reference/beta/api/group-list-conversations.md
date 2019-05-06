---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d178c5ac2932590dffbcb41bb7105ab00124997e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593019"
---
# <a name="list-conversations"></a><span data-ttu-id="43c20-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="43c20-103">List conversations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43c20-104">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="43c20-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="43c20-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="43c20-105">Permissions</span></span>
<span data-ttu-id="43c20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43c20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c20-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43c20-108">Permission type</span></span>      | <span data-ttu-id="43c20-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43c20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43c20-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43c20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43c20-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c20-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="43c20-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43c20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43c20-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43c20-113">Not supported.</span></span>    |
|<span data-ttu-id="43c20-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43c20-114">Application</span></span> | <span data-ttu-id="43c20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43c20-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43c20-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43c20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43c20-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43c20-117">Optional query parameters</span></span>
<span data-ttu-id="43c20-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43c20-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43c20-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43c20-119">Request headers</span></span>
| <span data-ttu-id="43c20-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43c20-120">Header</span></span>       | <span data-ttu-id="43c20-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43c20-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="43c20-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43c20-122">Authorization</span></span>  | <span data-ttu-id="43c20-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43c20-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43c20-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43c20-125">Request body</span></span>
<span data-ttu-id="43c20-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43c20-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c20-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="43c20-127">Response</span></span>
<span data-ttu-id="43c20-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43c20-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43c20-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43c20-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="43c20-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43c20-130">Request</span></span>
<span data-ttu-id="43c20-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43c20-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="43c20-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="43c20-132">Response</span></span>
<span data-ttu-id="43c20-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43c20-133">The following is an example of the response.</span></span>
><span data-ttu-id="43c20-134">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="43c20-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="43c20-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43c20-135">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="43c20-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="43c20-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="43c20-137">Basic</span><span class="sxs-lookup"><span data-stu-id="43c20-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversations-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43c20-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43c20-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversations-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
