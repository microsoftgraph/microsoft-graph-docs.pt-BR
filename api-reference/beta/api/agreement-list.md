---
title: Listar contratos
description: Recupere uma lista de objetos de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: e0e32646df18d7c6dfb58106568bb2a74261fa30
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217999"
---
# <a name="list-agreements"></a><span data-ttu-id="330e5-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="330e5-103">List agreements</span></span>

<span data-ttu-id="330e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="330e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="330e5-105">Recupere uma lista de objetos de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="330e5-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="330e5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="330e5-106">Permissions</span></span>
<span data-ttu-id="330e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="330e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="330e5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="330e5-109">Permission type</span></span>                        | <span data-ttu-id="330e5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="330e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="330e5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="330e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="330e5-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="330e5-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="330e5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="330e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="330e5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="330e5-114">Not supported.</span></span> |
|<span data-ttu-id="330e5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="330e5-115">Application</span></span>                            | <span data-ttu-id="330e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="330e5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="330e5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="330e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="330e5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="330e5-118">Request headers</span></span>
| <span data-ttu-id="330e5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="330e5-119">Name</span></span>         | <span data-ttu-id="330e5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="330e5-120">Type</span></span>        | <span data-ttu-id="330e5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="330e5-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="330e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="330e5-122">Authorization</span></span> | <span data-ttu-id="330e5-123">string</span><span class="sxs-lookup"><span data-stu-id="330e5-123">string</span></span> | <span data-ttu-id="330e5-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="330e5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="330e5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="330e5-126">Request body</span></span>
<span data-ttu-id="330e5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="330e5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="330e5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="330e5-128">Response</span></span>
<span data-ttu-id="330e5-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="330e5-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="330e5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="330e5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="330e5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="330e5-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="330e5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="330e5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/agreements
```
# <a name="c"></a>[<span data-ttu-id="330e5-133">C#</span><span class="sxs-lookup"><span data-stu-id="330e5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="330e5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="330e5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="330e5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="330e5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="330e5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="330e5-136">Response</span></span>
><span data-ttu-id="330e5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="330e5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
