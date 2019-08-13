---
title: Listar contratos
description: Recupere uma lista de objetos de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0a06dfbb3c7cb222d26d014a8f5b1d2357dd9e40
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318877"
---
# <a name="list-agreements"></a><span data-ttu-id="e1dea-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="e1dea-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1dea-104">Recupere uma lista de objetos de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="e1dea-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1dea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1dea-105">Permissions</span></span>
<span data-ttu-id="e1dea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1dea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1dea-108">Permission type</span></span>                        | <span data-ttu-id="e1dea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1dea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1dea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1dea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1dea-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1dea-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="e1dea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1dea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1dea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1dea-113">Not supported.</span></span> |
|<span data-ttu-id="e1dea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1dea-114">Application</span></span>                            | <span data-ttu-id="e1dea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1dea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1dea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1dea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="e1dea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1dea-117">Request headers</span></span>
| <span data-ttu-id="e1dea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e1dea-118">Name</span></span>         | <span data-ttu-id="e1dea-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1dea-119">Type</span></span>        | <span data-ttu-id="e1dea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1dea-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e1dea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1dea-121">Authorization</span></span> | <span data-ttu-id="e1dea-122">string</span><span class="sxs-lookup"><span data-stu-id="e1dea-122">string</span></span> | <span data-ttu-id="e1dea-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1dea-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1dea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1dea-125">Request body</span></span>
<span data-ttu-id="e1dea-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1dea-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e1dea-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1dea-127">Response</span></span>
<span data-ttu-id="e1dea-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1dea-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1dea-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1dea-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1dea-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1dea-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1dea-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1dea-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1dea-132">C#</span><span class="sxs-lookup"><span data-stu-id="e1dea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1dea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1dea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1dea-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e1dea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e1dea-135">Java</span><span class="sxs-lookup"><span data-stu-id="e1dea-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e1dea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1dea-136">Response</span></span>
><span data-ttu-id="e1dea-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1dea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
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
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
