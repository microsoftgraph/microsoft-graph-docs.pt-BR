---
title: Obter educationAssignment
description: Obter as propriedades e as relações de uma atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4d8eeaa80f94b867f4c0042302681631c343d459
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912174"
---
# <a name="get-educationassignment"></a><span data-ttu-id="8ed65-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ed65-103">Get educationAssignment</span></span>

<span data-ttu-id="8ed65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ed65-105">Obter as propriedades e as relações de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="8ed65-105">Get the properties and relationships of an assignment.</span></span> 

<span data-ttu-id="8ed65-106">Os alunos só podem ver atribuições atribuídas a eles; professores e aplicativos com permissões de aplicativo podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="8ed65-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed65-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ed65-107">Permissions</span></span>
<span data-ttu-id="8ed65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ed65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed65-110">Permission type</span></span>      | <span data-ttu-id="8ed65-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ed65-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ed65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed65-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8ed65-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ed65-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="8ed65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed65-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8ed65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed65-115">Not supported.</span></span>  |
|<span data-ttu-id="8ed65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ed65-116">Application</span></span> | <span data-ttu-id="8ed65-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ed65-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8ed65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed65-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ed65-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ed65-119">Optional query parameters</span></span>
<span data-ttu-id="8ed65-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed65-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ed65-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed65-121">Request headers</span></span>
| <span data-ttu-id="8ed65-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ed65-122">Header</span></span>       | <span data-ttu-id="8ed65-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8ed65-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ed65-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed65-124">Authorization</span></span>  | <span data-ttu-id="8ed65-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed65-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ed65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed65-127">Request body</span></span>
<span data-ttu-id="8ed65-128">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="8ed65-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ed65-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed65-129">Response</span></span>
<span data-ttu-id="8ed65-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed65-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed65-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ed65-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ed65-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed65-132">Request</span></span>
<span data-ttu-id="8ed65-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ed65-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0
```

### <a name="response"></a><span data-ttu-id="8ed65-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed65-134">Response</span></span>
<span data-ttu-id="8ed65-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed65-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8ed65-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ed65-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
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
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "notificationChannelUrl": null,
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
