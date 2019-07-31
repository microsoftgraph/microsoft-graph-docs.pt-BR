---
title: Obter educationAssignment
description: " os professores podem ver todas as atribuições em uma classe."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 22db7dc1c85de37c991078ba4c7b718c2e2dbc52
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955645"
---
# <a name="get-educationassignment"></a><span data-ttu-id="dfdb1-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="dfdb1-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfdb1-104">Obtenha as propriedades e os relacionamentos de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="dfdb1-105">Os alunos só podem ver as atribuições atribuídas a eles; os professores podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfdb1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfdb1-106">Permissions</span></span>
<span data-ttu-id="dfdb1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfdb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dfdb1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfdb1-109">Permission type</span></span>      | <span data-ttu-id="dfdb1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfdb1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfdb1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfdb1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dfdb1-112">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfdb1-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="dfdb1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfdb1-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dfdb1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-114">Not supported.</span></span>  |
|<span data-ttu-id="dfdb1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfdb1-115">Application</span></span> | <span data-ttu-id="dfdb1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="dfdb1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfdb1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfdb1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfdb1-118">Optional query parameters</span></span>
<span data-ttu-id="dfdb1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfdb1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfdb1-120">Request headers</span></span>
| <span data-ttu-id="dfdb1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfdb1-121">Header</span></span>       | <span data-ttu-id="dfdb1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dfdb1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfdb1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfdb1-123">Authorization</span></span>  | <span data-ttu-id="dfdb1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfdb1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfdb1-126">Request body</span></span>
<span data-ttu-id="dfdb1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfdb1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfdb1-128">Response</span></span>
<span data-ttu-id="dfdb1-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfdb1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfdb1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfdb1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfdb1-131">Request</span></span>
<span data-ttu-id="dfdb1-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="dfdb1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfdb1-133">Response</span></span>
<span data-ttu-id="dfdb1-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="dfdb1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfdb1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
