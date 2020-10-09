---
title: Obter educationAssignment
description: " os professores podem ver todas as atribuições em uma classe."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d31a7980c401fae746d0ebfc92742fe9f4cde702
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403640"
---
# <a name="get-educationassignment"></a><span data-ttu-id="dafae-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="dafae-103">Get educationAssignment</span></span>

<span data-ttu-id="dafae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dafae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dafae-105">Obtenha as propriedades e os relacionamentos de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="dafae-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="dafae-106">Os alunos só podem ver as atribuições atribuídas a eles; os professores podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="dafae-106">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="dafae-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dafae-107">Permissions</span></span>
<span data-ttu-id="dafae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dafae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dafae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dafae-110">Permission type</span></span>      | <span data-ttu-id="dafae-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dafae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dafae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dafae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dafae-113">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dafae-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="dafae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dafae-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dafae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dafae-115">Not supported.</span></span>  |
|<span data-ttu-id="dafae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dafae-116">Application</span></span> | <span data-ttu-id="dafae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dafae-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="dafae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dafae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dafae-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dafae-119">Optional query parameters</span></span>
<span data-ttu-id="dafae-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dafae-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dafae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dafae-121">Request headers</span></span>
| <span data-ttu-id="dafae-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dafae-122">Header</span></span>       | <span data-ttu-id="dafae-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dafae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dafae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dafae-124">Authorization</span></span>  | <span data-ttu-id="dafae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dafae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dafae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dafae-127">Request body</span></span>
<span data-ttu-id="dafae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dafae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dafae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dafae-129">Response</span></span>
<span data-ttu-id="dafae-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dafae-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dafae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dafae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dafae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dafae-132">Request</span></span>
<span data-ttu-id="dafae-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dafae-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="dafae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dafae-134">Response</span></span>
<span data-ttu-id="dafae-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dafae-135">The following is an example of the response.</span></span> 

><span data-ttu-id="dafae-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dafae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "closeDateTime": "2014-01-11T00:00:00Z",
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