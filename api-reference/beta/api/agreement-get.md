---
title: Obter contrato
description: Recupere as propriedades e relacionamentos de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: da36b6cb2d12c92d4bf12ec2ce4836f5bbc5efe1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517124"
---
# <a name="get-agreement"></a><span data-ttu-id="263a6-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="263a6-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="263a6-104">Recupere as propriedades e relacionamentos de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="263a6-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="263a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="263a6-105">Permissions</span></span>
<span data-ttu-id="263a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="263a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="263a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="263a6-108">Permission type</span></span>                        | <span data-ttu-id="263a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="263a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="263a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="263a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="263a6-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="263a6-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="263a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="263a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="263a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="263a6-113">Not supported.</span></span> |
|<span data-ttu-id="263a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="263a6-114">Application</span></span>                            | <span data-ttu-id="263a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="263a6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="263a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="263a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="263a6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="263a6-117">Request headers</span></span>
| <span data-ttu-id="263a6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="263a6-118">Name</span></span>         | <span data-ttu-id="263a6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="263a6-119">Type</span></span>        | <span data-ttu-id="263a6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="263a6-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="263a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="263a6-121">Authorization</span></span> | <span data-ttu-id="263a6-122">string</span><span class="sxs-lookup"><span data-stu-id="263a6-122">string</span></span> | <span data-ttu-id="263a6-123">Token de portador</span><span class="sxs-lookup"><span data-stu-id="263a6-123">Bearer \{token\}.</span></span> <span data-ttu-id="263a6-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="263a6-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="263a6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="263a6-125">Request body</span></span>
<span data-ttu-id="263a6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="263a6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="263a6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="263a6-127">Response</span></span>
<span data-ttu-id="263a6-128">Se tiver êxito, este método retornará um `200 OK` objeto de [contrato](../resources/agreement.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="263a6-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="263a6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="263a6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="263a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="263a6-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="263a6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="263a6-131">Response</span></span>
><span data-ttu-id="263a6-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="263a6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
