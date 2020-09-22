---
title: Listar tarefas
description: Retorna uma lista de atribuições atribuídas a um usuário para todas as classes. Este namespace de utilitário permite que um chamador encontre todas as atribuições de um aluno em uma única chamada, em vez de solicitar as atribuições de cada classe. A lista de atribuição contém o que é necessário para obter as informações detalhadas da atribuição de dentro do namespace da classe. Todas as outras operações na atribuição devem usar o namespace de classe.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b0fbc71cd5ac089a56a9acc6062112e69e956933
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981118"
---
# <a name="list-assignments"></a><span data-ttu-id="7ba5c-106">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="7ba5c-106">List assignments</span></span>

<span data-ttu-id="7ba5c-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ba5c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba5c-108">Retorna uma lista de atribuições atribuídas a um usuário para todas as classes.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-108">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="7ba5c-109">Este namespace de utilitário permite que um chamador encontre todas as atribuições de um aluno em uma única chamada, em vez de solicitar as atribuições de cada classe.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-109">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="7ba5c-110">A lista de atribuição contém o que é necessário para obter as informações detalhadas da atribuição de dentro do namespace da classe.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-110">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="7ba5c-111">Todas as outras operações na atribuição devem usar o namespace de classe.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-111">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ba5c-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ba5c-112">Permissions</span></span>

<span data-ttu-id="7ba5c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ba5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ba5c-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ba5c-115">Permission type</span></span>                        | <span data-ttu-id="7ba5c-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ba5c-116">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7ba5c-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ba5c-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ba5c-118">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ba5c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7ba5c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ba5c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ba5c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-120">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="7ba5c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ba5c-121">Application</span></span>                            | <span data-ttu-id="7ba5c-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-122">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="7ba5c-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ba5c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ba5c-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ba5c-124">Optional query parameters</span></span>

<span data-ttu-id="7ba5c-125">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ba5c-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ba5c-126">Request headers</span></span>

| <span data-ttu-id="7ba5c-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ba5c-127">Header</span></span>        | <span data-ttu-id="7ba5c-128">Valor</span><span class="sxs-lookup"><span data-stu-id="7ba5c-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7ba5c-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ba5c-129">Authorization</span></span> | <span data-ttu-id="7ba5c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ba5c-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ba5c-132">Request body</span></span>

<span data-ttu-id="7ba5c-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ba5c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ba5c-134">Response</span></span>

<span data-ttu-id="7ba5c-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-135">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ba5c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ba5c-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7ba5c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ba5c-137">Request</span></span>
<span data-ttu-id="7ba5c-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```

##### <a name="response"></a><span data-ttu-id="7ba5c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ba5c-139">Response</span></span>

<span data-ttu-id="7ba5c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-140">The following is an example of the response.</span></span> 

> <span data-ttu-id="7ba5c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ba5c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>


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


