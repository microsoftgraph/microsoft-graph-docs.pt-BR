---
title: Obter contrato
description: Recupere as propriedades e os relacionamentos de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: b500aa5a18fff6e2554dddea76dd02201e4467e8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258636"
---
# <a name="get-agreement"></a><span data-ttu-id="53d36-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="53d36-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53d36-104">Recupere as propriedades e os relacionamentos de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="53d36-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53d36-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="53d36-105">Permissions</span></span>
<span data-ttu-id="53d36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53d36-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53d36-108">Permission type</span></span>                        | <span data-ttu-id="53d36-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53d36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="53d36-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53d36-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53d36-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="53d36-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="53d36-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53d36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53d36-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53d36-113">Not supported.</span></span> |
|<span data-ttu-id="53d36-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53d36-114">Application</span></span>                            | <span data-ttu-id="53d36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53d36-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53d36-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53d36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="53d36-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53d36-117">Request headers</span></span>
| <span data-ttu-id="53d36-118">Nome</span><span class="sxs-lookup"><span data-stu-id="53d36-118">Name</span></span>         | <span data-ttu-id="53d36-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="53d36-119">Type</span></span>        | <span data-ttu-id="53d36-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="53d36-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53d36-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="53d36-121">Authorization</span></span> | <span data-ttu-id="53d36-122">string</span><span class="sxs-lookup"><span data-stu-id="53d36-122">string</span></span> | <span data-ttu-id="53d36-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53d36-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53d36-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53d36-125">Request body</span></span>
<span data-ttu-id="53d36-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53d36-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53d36-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="53d36-127">Response</span></span>
<span data-ttu-id="53d36-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53d36-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53d36-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53d36-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53d36-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53d36-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="53d36-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="53d36-131">Response</span></span>
><span data-ttu-id="53d36-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53d36-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="53d36-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="53d36-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="53d36-135">C#</span><span class="sxs-lookup"><span data-stu-id="53d36-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53d36-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="53d36-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreement-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="53d36-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="53d36-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_agreement-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
