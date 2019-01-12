---
title: Obter educationAssignment
description: " professores podem ver todas as atribuições em uma classe."
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 66279d72952a561a5e98be00ae268ca58c5dcc92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976398"
---
# <a name="get-educationassignment"></a><span data-ttu-id="144e2-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="144e2-103">Get educationAssignment</span></span>

> <span data-ttu-id="144e2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="144e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="144e2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="144e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="144e2-106">Obtenha as propriedades e relacionamentos de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="144e2-106">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="144e2-107">Alunos só podem ver atribuições atribuídas a eles; professores podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="144e2-107">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="144e2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="144e2-108">Permissions</span></span>
<span data-ttu-id="144e2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="144e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="144e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="144e2-111">Permission type</span></span>      | <span data-ttu-id="144e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="144e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="144e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="144e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="144e2-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="144e2-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="144e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="144e2-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="144e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="144e2-116">Not supported.</span></span>  |
|<span data-ttu-id="144e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="144e2-117">Application</span></span> | <span data-ttu-id="144e2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="144e2-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="144e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="144e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="144e2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="144e2-120">Optional query parameters</span></span>
<span data-ttu-id="144e2-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="144e2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="144e2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="144e2-122">Request headers</span></span>
| <span data-ttu-id="144e2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="144e2-123">Header</span></span>       | <span data-ttu-id="144e2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="144e2-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="144e2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="144e2-125">Authorization</span></span>  | <span data-ttu-id="144e2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="144e2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="144e2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="144e2-128">Request body</span></span>
<span data-ttu-id="144e2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="144e2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="144e2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="144e2-130">Response</span></span>
<span data-ttu-id="144e2-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="144e2-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="144e2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="144e2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="144e2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="144e2-133">Request</span></span>
<span data-ttu-id="144e2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="144e2-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="144e2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="144e2-135">Response</span></span>
<span data-ttu-id="144e2-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="144e2-136">The following is an example of the response.</span></span> 

><span data-ttu-id="144e2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="144e2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
