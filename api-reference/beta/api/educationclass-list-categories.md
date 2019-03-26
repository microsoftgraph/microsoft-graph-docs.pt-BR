---
title: Listar educationCategories
description: Recupere uma lista de objetos Category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fc0f6908f710f53f73d558118b7b7a74f1494113
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800948"
---
# <a name="list-educationcategories"></a><span data-ttu-id="2ff0f-103">Listar educationCategories</span><span class="sxs-lookup"><span data-stu-id="2ff0f-103">List educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff0f-104">Recupere uma lista de objetos [educationCategory](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="2ff0f-104">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ff0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ff0f-105">Permissions</span></span>
<span data-ttu-id="2ff0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ff0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ff0f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ff0f-108">Permission type</span></span>      | <span data-ttu-id="2ff0f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ff0f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ff0f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ff0f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ff0f-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ff0f-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="2ff0f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ff0f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2ff0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-113">Not supported.</span></span>  |
|<span data-ttu-id="2ff0f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ff0f-114">Application</span></span> | <span data-ttu-id="2ff0f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2ff0f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ff0f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2ff0f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ff0f-117">Optional query parameters</span></span>
<span data-ttu-id="2ff0f-118">Este método oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ff0f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ff0f-119">Request headers</span></span>
| <span data-ttu-id="2ff0f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ff0f-120">Header</span></span>       | <span data-ttu-id="2ff0f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ff0f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ff0f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ff0f-122">Authorization</span></span>  | <span data-ttu-id="2ff0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ff0f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ff0f-125">Request body</span></span>
<span data-ttu-id="2ff0f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2ff0f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ff0f-127">Response</span></span>
<span data-ttu-id="2ff0f-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-128">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ff0f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ff0f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ff0f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ff0f-130">Request</span></span>
<span data-ttu-id="2ff0f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignmentCategories
```
##### <a name="response"></a><span data-ttu-id="2ff0f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ff0f-132">Response</span></span>
<span data-ttu-id="2ff0f-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-133">The following is an example of the response.</span></span> 

><span data-ttu-id="2ff0f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ff0f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-categories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
