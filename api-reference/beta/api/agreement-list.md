---
title: Contratos de lista
description: Recupere uma lista de objetos do contrato.
localization_priority: Normal
ms.openlocfilehash: 82674e81b6b059ffafedf3b9c15c19e90438dc28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525973"
---
# <a name="list-agreements"></a><span data-ttu-id="70be1-103">Contratos de lista</span><span class="sxs-lookup"><span data-stu-id="70be1-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70be1-104">Recupere uma lista de objetos do [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="70be1-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="70be1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="70be1-105">Permissions</span></span>
<span data-ttu-id="70be1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70be1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70be1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70be1-108">Permission type</span></span>                        | <span data-ttu-id="70be1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70be1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="70be1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70be1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="70be1-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="70be1-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="70be1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70be1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70be1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70be1-113">Not supported.</span></span> |
|<span data-ttu-id="70be1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70be1-114">Application</span></span>                            | <span data-ttu-id="70be1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70be1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70be1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70be1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="70be1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70be1-117">Request headers</span></span>
| <span data-ttu-id="70be1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="70be1-118">Name</span></span>         | <span data-ttu-id="70be1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="70be1-119">Type</span></span>        | <span data-ttu-id="70be1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="70be1-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="70be1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="70be1-121">Authorization</span></span> | <span data-ttu-id="70be1-122">string</span><span class="sxs-lookup"><span data-stu-id="70be1-122">string</span></span> | <span data-ttu-id="70be1-123">Token de portador</span><span class="sxs-lookup"><span data-stu-id="70be1-123">Bearer \{token\}.</span></span> <span data-ttu-id="70be1-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70be1-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70be1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70be1-125">Request body</span></span>
<span data-ttu-id="70be1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70be1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="70be1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="70be1-127">Response</span></span>
<span data-ttu-id="70be1-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [contrato](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70be1-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70be1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70be1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70be1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70be1-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="70be1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="70be1-131">Response</span></span>
><span data-ttu-id="70be1-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70be1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
