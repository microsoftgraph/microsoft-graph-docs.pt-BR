---
title: Listar atribuições de um usuário
description: Obter uma lista de atribuições atribuídas a um usuário para todas as classes.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4d64a865bf6554cfb9c1a7e2abea812e6ba0b8e4
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912151"
---
# <a name="list-assignments-of-a-user"></a><span data-ttu-id="12a41-103">Listar atribuições de um usuário</span><span class="sxs-lookup"><span data-stu-id="12a41-103">List assignments of a user</span></span>

<span data-ttu-id="12a41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12a41-105">Obter uma lista de atribuições atribuídas a um usuário para todas as classes.</span><span class="sxs-lookup"><span data-stu-id="12a41-105">Get a list of assignments assigned to a user for all classes.</span></span> 

<span data-ttu-id="12a41-106">Esse namespace utilitário permite que um chamador encontre todas as atribuições de um aluno em uma única chamada, em vez de ter que solicitar atribuições de cada classe.</span><span class="sxs-lookup"><span data-stu-id="12a41-106">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="12a41-107">A lista de atribuições contém o que é necessário para obter as informações detalhadas para a atribuição de dentro do namespace de classe.</span><span class="sxs-lookup"><span data-stu-id="12a41-107">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="12a41-108">Todas as outras operações na atribuição devem usar o namespace de classe.</span><span class="sxs-lookup"><span data-stu-id="12a41-108">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="12a41-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="12a41-109">Permissions</span></span>

<span data-ttu-id="12a41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12a41-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12a41-112">Permission type</span></span>                        | <span data-ttu-id="12a41-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12a41-113">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="12a41-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12a41-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="12a41-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12a41-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="12a41-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12a41-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a41-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a41-117">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="12a41-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12a41-118">Application</span></span>                            | <span data-ttu-id="12a41-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a41-119">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="12a41-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12a41-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12a41-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12a41-121">Optional query parameters</span></span>

<span data-ttu-id="12a41-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12a41-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12a41-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12a41-123">Request headers</span></span>

| <span data-ttu-id="12a41-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12a41-124">Header</span></span>        | <span data-ttu-id="12a41-125">Valor</span><span class="sxs-lookup"><span data-stu-id="12a41-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="12a41-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="12a41-126">Authorization</span></span> | <span data-ttu-id="12a41-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12a41-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12a41-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12a41-129">Request body</span></span>

<span data-ttu-id="12a41-130">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="12a41-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a41-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a41-131">Response</span></span>

<span data-ttu-id="12a41-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12a41-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a41-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12a41-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a41-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12a41-134">Request</span></span>
<span data-ttu-id="12a41-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12a41-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_me_assignments"
}-->

```http 
GET https://graph.microsoft.com/v1.0/education/me/assignments
```

### <a name="response"></a><span data-ttu-id="12a41-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a41-136">Response</span></span>

<span data-ttu-id="12a41-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12a41-137">The following is an example of the response.</span></span> 

> <span data-ttu-id="12a41-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="12a41-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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
            "displayName": "Shawn Hughes",
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
            "displayName": "Shawn Hughes",
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
