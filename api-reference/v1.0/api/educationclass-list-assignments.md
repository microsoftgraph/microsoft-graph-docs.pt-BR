---
title: Listar atribuições de classe
description: Recupere uma lista de objetos de atribuição.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a0c85c4aaac82583acda75158ec73c31d2d91837
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993070"
---
# <a name="list-class-assignments"></a><span data-ttu-id="fb0c0-103">Listar atribuições de classe</span><span class="sxs-lookup"><span data-stu-id="fb0c0-103">List class assignments</span></span>

<span data-ttu-id="fb0c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb0c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb0c0-105">Recupere uma lista de objetos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-105">Retrieve a list of assignment objects.</span></span> 

<span data-ttu-id="fb0c0-106">Um professor ou um aplicativo que executa com permissões de aplicativo pode ver todos os objetos de atribuição da classe.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-106">A teacher or an application executing with application permissions can see all assignment objects for the class.</span></span> <span data-ttu-id="fb0c0-107">Os alunos só podem ver atribuições atribuídas a eles.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-107">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb0c0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb0c0-108">Permissions</span></span>

<span data-ttu-id="fb0c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb0c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb0c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb0c0-111">Permission type</span></span>                        | <span data-ttu-id="fb0c0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb0c0-112">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fb0c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb0c0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb0c0-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb0c0-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="fb0c0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb0c0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb0c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-116">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="fb0c0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb0c0-117">Application</span></span>                            | <span data-ttu-id="fb0c0-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb0c0-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb0c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb0c0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb0c0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb0c0-120">Optional query parameters</span></span>
<span data-ttu-id="fb0c0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb0c0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb0c0-122">Request headers</span></span>

| <span data-ttu-id="fb0c0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb0c0-123">Header</span></span>        | <span data-ttu-id="fb0c0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fb0c0-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="fb0c0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb0c0-125">Authorization</span></span> | <span data-ttu-id="fb0c0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb0c0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb0c0-128">Request body</span></span>

<span data-ttu-id="fb0c0-129">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb0c0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb0c0-130">Response</span></span>

<span data-ttu-id="fb0c0-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-131">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb0c0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb0c0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb0c0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb0c0-133">Request</span></span>

<span data-ttu-id="fb0c0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fb0c0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb0c0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments
```
# <a name="c"></a>[<span data-ttu-id="fb0c0-136">C#</span><span class="sxs-lookup"><span data-stu-id="fb0c0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb0c0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb0c0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb0c0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb0c0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb0c0-139">Java</span><span class="sxs-lookup"><span data-stu-id="fb0c0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb0c0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb0c0-140">Response</span></span>

<span data-ttu-id="fb0c0-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-141">The following is an example of the response.</span></span> 

><span data-ttu-id="fb0c0-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb0c0-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "addedStudentAction": "none",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "closeDateTime": "2014-02-11T00:00:00Z",
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
      "notificationChannelUrl": null,
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
