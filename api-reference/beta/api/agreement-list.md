---
title: Listar contratos
description: Recupere uma lista de objetos de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7c07a0308443c1d631122dd22c031789d8eb5acf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945703"
---
# <a name="list-agreements"></a><span data-ttu-id="c6816-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="c6816-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6816-104">Recupere uma lista de objetos de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="c6816-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6816-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6816-105">Permissions</span></span>
<span data-ttu-id="c6816-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6816-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6816-108">Permission type</span></span>                        | <span data-ttu-id="c6816-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6816-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6816-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6816-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6816-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6816-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="c6816-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6816-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6816-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6816-113">Not supported.</span></span> |
|<span data-ttu-id="c6816-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6816-114">Application</span></span>                            | <span data-ttu-id="c6816-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6816-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6816-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6816-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="c6816-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6816-117">Request headers</span></span>
| <span data-ttu-id="c6816-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c6816-118">Name</span></span>         | <span data-ttu-id="c6816-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6816-119">Type</span></span>        | <span data-ttu-id="c6816-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6816-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c6816-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6816-121">Authorization</span></span> | <span data-ttu-id="c6816-122">string</span><span class="sxs-lookup"><span data-stu-id="c6816-122">string</span></span> | <span data-ttu-id="c6816-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6816-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6816-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6816-125">Request body</span></span>
<span data-ttu-id="c6816-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6816-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c6816-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6816-127">Response</span></span>
<span data-ttu-id="c6816-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6816-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6816-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6816-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6816-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6816-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c6816-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6816-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c6816-132">C#</span><span class="sxs-lookup"><span data-stu-id="c6816-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6816-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6816-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c6816-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c6816-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c6816-135">Java</span><span class="sxs-lookup"><span data-stu-id="c6816-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6816-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6816-136">Response</span></span>
><span data-ttu-id="c6816-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6816-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
