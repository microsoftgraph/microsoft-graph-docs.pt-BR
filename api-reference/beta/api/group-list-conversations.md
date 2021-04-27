---
title: Listar conversas
description: Recupere a lista de conversas desse grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 36b5033eb6e389b6e22138a46cdc263b12abbf0f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041705"
---
# <a name="list-conversations"></a><span data-ttu-id="7e51c-103">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="7e51c-103">List conversations</span></span>

<span data-ttu-id="7e51c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e51c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e51c-105">Recupere a lista de [conversas](../resources/conversation.md) desse grupo.</span><span class="sxs-lookup"><span data-stu-id="7e51c-105">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e51c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e51c-106">Permissions</span></span>
<span data-ttu-id="7e51c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e51c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e51c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e51c-109">Permission type</span></span>      | <span data-ttu-id="7e51c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e51c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e51c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e51c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e51c-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e51c-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e51c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e51c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e51c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e51c-114">Not supported.</span></span>    |
|<span data-ttu-id="7e51c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e51c-115">Application</span></span> | <span data-ttu-id="7e51c-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e51c-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e51c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e51c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e51c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e51c-118">Optional query parameters</span></span>
<span data-ttu-id="7e51c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e51c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e51c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e51c-120">Request headers</span></span>
| <span data-ttu-id="7e51c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e51c-121">Header</span></span>       | <span data-ttu-id="7e51c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7e51c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e51c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e51c-123">Authorization</span></span>  | <span data-ttu-id="7e51c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e51c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e51c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e51c-126">Request body</span></span>
<span data-ttu-id="7e51c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e51c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e51c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e51c-128">Response</span></span>
<span data-ttu-id="7e51c-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e51c-129">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e51c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e51c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7e51c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e51c-131">Request</span></span>
<span data-ttu-id="7e51c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e51c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e51c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e51c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```
# <a name="c"></a>[<span data-ttu-id="7e51c-134">C#</span><span class="sxs-lookup"><span data-stu-id="7e51c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e51c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e51c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e51c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e51c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e51c-137">Java</span><span class="sxs-lookup"><span data-stu-id="7e51c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e51c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e51c-138">Response</span></span>
<span data-ttu-id="7e51c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e51c-139">The following is an example of the response.</span></span>
><span data-ttu-id="7e51c-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e51c-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


