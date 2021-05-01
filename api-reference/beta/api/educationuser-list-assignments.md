---
title: Listar tarefas
description: Retorna uma lista de atribuições atribuídas a um usuário para todas as classes. Esse namespace utilitário permite que um chamador encontre todas as atribuições de um aluno em uma única chamada, em vez de ter que solicitar atribuições de cada classe. A lista de atribuições contém o que é necessário para obter as informações detalhadas para a atribuição de dentro do namespace de classe. Todas as outras operações na atribuição devem usar o namespace de classe.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 682a03d4785184132c8a5aff3044f9ff9f2a4670
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118869"
---
# <a name="list-assignments"></a><span data-ttu-id="5ad24-106">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="5ad24-106">List assignments</span></span>

<span data-ttu-id="5ad24-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ad24-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ad24-108">Retorna uma lista de atribuições atribuídas a um usuário para todas as classes.</span><span class="sxs-lookup"><span data-stu-id="5ad24-108">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="5ad24-109">Esse namespace utilitário permite que um chamador encontre todas as atribuições de um aluno em uma única chamada, em vez de ter que solicitar atribuições de cada classe.</span><span class="sxs-lookup"><span data-stu-id="5ad24-109">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="5ad24-110">A lista de atribuições contém o que é necessário para obter as informações detalhadas para a atribuição de dentro do namespace de classe.</span><span class="sxs-lookup"><span data-stu-id="5ad24-110">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="5ad24-111">Todas as outras operações na atribuição devem usar o namespace de classe.</span><span class="sxs-lookup"><span data-stu-id="5ad24-111">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ad24-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ad24-112">Permissions</span></span>

<span data-ttu-id="5ad24-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ad24-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ad24-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ad24-115">Permission type</span></span>                        | <span data-ttu-id="5ad24-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ad24-116">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5ad24-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ad24-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ad24-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ad24-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="5ad24-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ad24-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ad24-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ad24-120">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="5ad24-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ad24-121">Application</span></span>                            | <span data-ttu-id="5ad24-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ad24-122">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="5ad24-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ad24-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ad24-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ad24-124">Optional query parameters</span></span>

<span data-ttu-id="5ad24-125">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ad24-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ad24-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ad24-126">Request headers</span></span>

| <span data-ttu-id="5ad24-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ad24-127">Header</span></span>        | <span data-ttu-id="5ad24-128">Valor</span><span class="sxs-lookup"><span data-stu-id="5ad24-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5ad24-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ad24-129">Authorization</span></span> | <span data-ttu-id="5ad24-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ad24-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ad24-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ad24-132">Request body</span></span>

<span data-ttu-id="5ad24-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ad24-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ad24-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ad24-134">Response</span></span>

<span data-ttu-id="5ad24-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ad24-135">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ad24-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ad24-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ad24-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ad24-137">Request</span></span>
<span data-ttu-id="5ad24-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ad24-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="5ad24-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ad24-139">Response</span></span>

<span data-ttu-id="5ad24-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ad24-140">The following is an example of the response.</span></span> 

> <span data-ttu-id="5ad24-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ad24-141">**Note:** The response object shown here might be shortened for readability.</span></span>


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
      "closeDateTime": "2014-01-11T00:00:00Z",
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
  "suppressions": []
}
-->