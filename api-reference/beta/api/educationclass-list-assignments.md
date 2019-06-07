---
title: Listar tarefas
description: Recupere uma lista de objetos assignment. Um professor tem permissão para ver todos os objetos Assignment da classe. Os alunos só podem ver as atribuições atribuídas a eles.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 58ce5e911806e6e4c6e19ce3e419bd9b02c1a990
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750007"
---
# <a name="list-assignments"></a><span data-ttu-id="43f52-105">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="43f52-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f52-106">Recupere uma lista de objetos assignment.</span><span class="sxs-lookup"><span data-stu-id="43f52-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="43f52-107">Um professor tem permissão para ver todos os objetos Assignment da classe.</span><span class="sxs-lookup"><span data-stu-id="43f52-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="43f52-108">Os alunos só podem ver as atribuições atribuídas a eles.</span><span class="sxs-lookup"><span data-stu-id="43f52-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="43f52-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="43f52-109">Permissions</span></span>

<span data-ttu-id="43f52-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43f52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43f52-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43f52-112">Permission type</span></span>                        | <span data-ttu-id="43f52-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43f52-113">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="43f52-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43f52-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="43f52-115">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43f52-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="43f52-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43f52-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43f52-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43f52-117">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="43f52-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f52-118">Application</span></span>                            | <span data-ttu-id="43f52-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43f52-119">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="43f52-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43f52-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43f52-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43f52-121">Optional query parameters</span></span>
<span data-ttu-id="43f52-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43f52-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43f52-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43f52-123">Request headers</span></span>

| <span data-ttu-id="43f52-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43f52-124">Header</span></span>        | <span data-ttu-id="43f52-125">Valor</span><span class="sxs-lookup"><span data-stu-id="43f52-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="43f52-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="43f52-126">Authorization</span></span> | <span data-ttu-id="43f52-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43f52-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43f52-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43f52-129">Request body</span></span>

<span data-ttu-id="43f52-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43f52-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43f52-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f52-131">Response</span></span>

<span data-ttu-id="43f52-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43f52-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f52-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43f52-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="43f52-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f52-134">Request</span></span>

<span data-ttu-id="43f52-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f52-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="43f52-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f52-136">Response</span></span>

<span data-ttu-id="43f52-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43f52-137">The following is an example of the response.</span></span> 

><span data-ttu-id="43f52-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43f52-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
