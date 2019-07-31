---
title: Obter contrato
description: Recupere as propriedades e os relacionamentos de um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 21d090a3e1b23a1870fc86d418fd3edfc3ff69ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945689"
---
# <a name="get-agreement"></a><span data-ttu-id="748dc-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="748dc-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="748dc-104">Recupere as propriedades e os relacionamentos de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="748dc-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="748dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="748dc-105">Permissions</span></span>
<span data-ttu-id="748dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="748dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="748dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="748dc-108">Permission type</span></span>                        | <span data-ttu-id="748dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="748dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="748dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="748dc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="748dc-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="748dc-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="748dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="748dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="748dc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="748dc-113">Not supported.</span></span> |
|<span data-ttu-id="748dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="748dc-114">Application</span></span>                            | <span data-ttu-id="748dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="748dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="748dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="748dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="748dc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="748dc-117">Request headers</span></span>
| <span data-ttu-id="748dc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="748dc-118">Name</span></span>         | <span data-ttu-id="748dc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="748dc-119">Type</span></span>        | <span data-ttu-id="748dc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="748dc-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="748dc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="748dc-121">Authorization</span></span> | <span data-ttu-id="748dc-122">string</span><span class="sxs-lookup"><span data-stu-id="748dc-122">string</span></span> | <span data-ttu-id="748dc-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="748dc-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="748dc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="748dc-125">Request body</span></span>
<span data-ttu-id="748dc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="748dc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="748dc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="748dc-127">Response</span></span>
<span data-ttu-id="748dc-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="748dc-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="748dc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="748dc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="748dc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="748dc-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="748dc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="748dc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="748dc-132">C#</span><span class="sxs-lookup"><span data-stu-id="748dc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="748dc-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="748dc-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="748dc-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="748dc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="748dc-135">Java</span><span class="sxs-lookup"><span data-stu-id="748dc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="748dc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="748dc-136">Response</span></span>
><span data-ttu-id="748dc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="748dc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
