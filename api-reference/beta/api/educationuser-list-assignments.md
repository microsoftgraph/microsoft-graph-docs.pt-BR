---
title: Lista de atribuições
description: Retorna uma lista de atribuições atribuídas a um usuário para todas as classes. Esse namespace utilitário permite que um chamador localizar as atribuições de todos os student em uma única chamada em vez de solicitar atribuições de cada classe. A lista de atribuição contém o que é necessário para obter as informações detalhadas para a atribuição no namespace da classe. Todas as outras operações na atribuição devem usar o namespace de classe.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e2e11eb94c07fc523d6d64143ffc3df401fd9906
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515976"
---
# <a name="list-assignments"></a><span data-ttu-id="4d9b4-106">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="4d9b4-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d9b4-107">Retorna uma lista de atribuições atribuídas a um usuário para todas as classes.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="4d9b4-108">Esse namespace utilitário permite que um chamador localizar as atribuições de todos os student em uma única chamada em vez de solicitar atribuições de cada classe.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="4d9b4-109">A lista de atribuição contém o que é necessário para obter as informações detalhadas para a atribuição no namespace da classe.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="4d9b4-110">Todas as outras operações na atribuição devem usar o namespace de classe.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d9b4-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d9b4-111">Permissions</span></span>
<span data-ttu-id="4d9b4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d9b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d9b4-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d9b4-114">Permission type</span></span>      | <span data-ttu-id="4d9b4-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d9b4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d9b4-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d9b4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4d9b4-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d9b4-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4d9b4-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d9b4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d9b4-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-119">Not supported.</span></span>   |
|<span data-ttu-id="4d9b4-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d9b4-120">Application</span></span> | <span data-ttu-id="4d9b4-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4d9b4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d9b4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4d9b4-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4d9b4-123">Optional query parameters</span></span>
<span data-ttu-id="4d9b4-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d9b4-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d9b4-125">Request headers</span></span>
| <span data-ttu-id="4d9b4-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d9b4-126">Header</span></span>       | <span data-ttu-id="4d9b4-127">Valor</span><span class="sxs-lookup"><span data-stu-id="4d9b4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d9b4-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d9b4-128">Authorization</span></span>  | <span data-ttu-id="4d9b4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d9b4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d9b4-131">Request body</span></span>
<span data-ttu-id="4d9b4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4d9b4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d9b4-133">Response</span></span>
<span data-ttu-id="4d9b4-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d9b4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d9b4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d9b4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d9b4-136">Request</span></span>
<span data-ttu-id="4d9b4-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="4d9b4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d9b4-138">Response</span></span>
<span data-ttu-id="4d9b4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-139">The following is an example of the response.</span></span> 

><span data-ttu-id="4d9b4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d9b4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
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
    "Error: /api-reference/beta/api/educationuser-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
