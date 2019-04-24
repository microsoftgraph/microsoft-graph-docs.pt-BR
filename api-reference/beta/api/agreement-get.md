---
title: Obter contrato
description: Recupere as propriedades e os relacionamentos de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: da36b6cb2d12c92d4bf12ec2ce4836f5bbc5efe1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459189"
---
# <a name="get-agreement"></a><span data-ttu-id="b3b0b-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="b3b0b-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b0b-104">Recupere as propriedades e os relacionamentos de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="b3b0b-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3b0b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3b0b-105">Permissions</span></span>
<span data-ttu-id="b3b0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3b0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3b0b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3b0b-108">Permission type</span></span>                        | <span data-ttu-id="b3b0b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3b0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3b0b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3b0b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3b0b-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3b0b-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="b3b0b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3b0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3b0b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3b0b-113">Not supported.</span></span> |
|<span data-ttu-id="b3b0b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3b0b-114">Application</span></span>                            | <span data-ttu-id="b3b0b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3b0b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3b0b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3b0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="b3b0b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3b0b-117">Request headers</span></span>
| <span data-ttu-id="b3b0b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b3b0b-118">Name</span></span>         | <span data-ttu-id="b3b0b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3b0b-119">Type</span></span>        | <span data-ttu-id="b3b0b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3b0b-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b3b0b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3b0b-121">Authorization</span></span> | <span data-ttu-id="b3b0b-122">string</span><span class="sxs-lookup"><span data-stu-id="b3b0b-122">string</span></span> | <span data-ttu-id="b3b0b-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3b0b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3b0b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3b0b-125">Request body</span></span>
<span data-ttu-id="b3b0b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3b0b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b3b0b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3b0b-127">Response</span></span>
<span data-ttu-id="b3b0b-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3b0b-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3b0b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3b0b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3b0b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3b0b-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="b3b0b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3b0b-131">Response</span></span>
><span data-ttu-id="b3b0b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3b0b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
