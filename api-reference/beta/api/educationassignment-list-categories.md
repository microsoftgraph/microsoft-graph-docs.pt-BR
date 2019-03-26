---
title: Listar categorias
description: Listar todas as categorias associadas a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 925b2f558b98e50cfcebd7b68c3af52452f2e3df
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800950"
---
# <a name="list-categories"></a><span data-ttu-id="7d065-103">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="7d065-103">List categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d065-104">Listar todas as categorias associadas a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="7d065-104">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d065-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d065-105">Permissions</span></span>
<span data-ttu-id="7d065-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d065-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d065-108">Permission type</span></span>      | <span data-ttu-id="7d065-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d065-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d065-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d065-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7d065-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d065-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7d065-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d065-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7d065-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d065-113">Not supported.</span></span>  |
|<span data-ttu-id="7d065-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d065-114">Application</span></span> | <span data-ttu-id="7d065-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d065-115">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7d065-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d065-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d065-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d065-117">Optional query parameters</span></span>
<span data-ttu-id="7d065-118">Este método oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d065-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d065-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d065-119">Request headers</span></span>
| <span data-ttu-id="7d065-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d065-120">Header</span></span>       | <span data-ttu-id="7d065-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d065-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d065-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d065-122">Authorization</span></span>  | <span data-ttu-id="7d065-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d065-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d065-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d065-125">Request body</span></span>
<span data-ttu-id="7d065-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d065-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7d065-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d065-127">Response</span></span>
<span data-ttu-id="7d065-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d065-128">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d065-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d065-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d065-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d065-130">Request</span></span>
<span data-ttu-id="7d065-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d065-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="7d065-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d065-132">Response</span></span>
<span data-ttu-id="7d065-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d065-133">The following is an example of the response.</span></span> 

><span data-ttu-id="7d065-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d065-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7d065-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d065-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-categories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
