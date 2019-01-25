---
title: Lista de atribuições
description: Recupere uma lista de objetos assignment. Um professor é permitido para ver todos os objetos de atribuição para a classe. Alunos só podem ver atribuições que são atribuídas a eles.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7cd47c61d4958d42ce099396147d421a6555041b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519140"
---
# <a name="list-assignments"></a><span data-ttu-id="6dd22-105">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="6dd22-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd22-106">Recupere uma lista de objetos assignment.</span><span class="sxs-lookup"><span data-stu-id="6dd22-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="6dd22-107">Um professor é permitido para ver todos os objetos de atribuição para a classe.</span><span class="sxs-lookup"><span data-stu-id="6dd22-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="6dd22-108">Alunos só podem ver atribuições que são atribuídas a eles.</span><span class="sxs-lookup"><span data-stu-id="6dd22-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd22-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dd22-109">Permissions</span></span>
<span data-ttu-id="6dd22-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd22-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd22-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dd22-112">Permission type</span></span>      | <span data-ttu-id="6dd22-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dd22-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dd22-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dd22-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6dd22-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dd22-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6dd22-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dd22-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6dd22-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dd22-117">Not supported.</span></span>  |
|<span data-ttu-id="6dd22-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dd22-118">Application</span></span> | <span data-ttu-id="6dd22-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dd22-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6dd22-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dd22-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6dd22-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6dd22-121">Optional query parameters</span></span>
<span data-ttu-id="6dd22-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6dd22-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dd22-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dd22-123">Request headers</span></span>
| <span data-ttu-id="6dd22-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6dd22-124">Header</span></span>       | <span data-ttu-id="6dd22-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6dd22-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6dd22-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dd22-126">Authorization</span></span>  | <span data-ttu-id="6dd22-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dd22-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6dd22-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dd22-129">Request body</span></span>
<span data-ttu-id="6dd22-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6dd22-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6dd22-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dd22-131">Response</span></span>
<span data-ttu-id="6dd22-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dd22-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dd22-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dd22-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dd22-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dd22-134">Request</span></span>
<span data-ttu-id="6dd22-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dd22-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="6dd22-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dd22-136">Response</span></span>
<span data-ttu-id="6dd22-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6dd22-137">The following is an example of the response.</span></span> 

><span data-ttu-id="6dd22-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dd22-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "createdDateTime": "2014-02-01T00:00:00Z",
      "displayName": "published",
      "dueDateTime": "2014-02-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "contentType": "Text",
        "content": "Read chapters 1 through 3"
      },
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2014-02-01T00:00:00Z",
      "status": "published"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
