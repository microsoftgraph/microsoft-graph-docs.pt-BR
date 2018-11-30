---
title: Lista de atribuições
description: Recupere uma lista de objetos assignment. Um professor é permitido para ver todos os objetos de atribuição para a classe. Alunos só podem ver atribuições que são atribuídas a eles.
ms.openlocfilehash: 664356620e83534c5cd686e0d1df796bd3743a3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035921"
---
# <a name="list-assignments"></a><span data-ttu-id="594ba-105">Lista de atribuições</span><span class="sxs-lookup"><span data-stu-id="594ba-105">List assignments</span></span>

> <span data-ttu-id="594ba-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="594ba-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="594ba-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="594ba-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="594ba-108">Recupere uma lista de objetos assignment.</span><span class="sxs-lookup"><span data-stu-id="594ba-108">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="594ba-109">Um professor é permitido para ver todos os objetos de atribuição para a classe.</span><span class="sxs-lookup"><span data-stu-id="594ba-109">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="594ba-110">Alunos só podem ver atribuições que são atribuídas a eles.</span><span class="sxs-lookup"><span data-stu-id="594ba-110">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="594ba-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="594ba-111">Permissions</span></span>
<span data-ttu-id="594ba-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="594ba-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="594ba-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="594ba-114">Permission type</span></span>      | <span data-ttu-id="594ba-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="594ba-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="594ba-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="594ba-116">Delegated (work or school account)</span></span> | <span data-ttu-id="594ba-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="594ba-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="594ba-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="594ba-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="594ba-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="594ba-119">Not supported.</span></span>  |
|<span data-ttu-id="594ba-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="594ba-120">Application</span></span> | <span data-ttu-id="594ba-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="594ba-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="594ba-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="594ba-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="594ba-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="594ba-123">Optional query parameters</span></span>
<span data-ttu-id="594ba-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="594ba-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="594ba-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="594ba-125">Request headers</span></span>
| <span data-ttu-id="594ba-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="594ba-126">Header</span></span>       | <span data-ttu-id="594ba-127">Valor</span><span class="sxs-lookup"><span data-stu-id="594ba-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="594ba-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="594ba-128">Authorization</span></span>  | <span data-ttu-id="594ba-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="594ba-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="594ba-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="594ba-131">Request body</span></span>
<span data-ttu-id="594ba-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="594ba-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="594ba-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="594ba-133">Response</span></span>
<span data-ttu-id="594ba-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="594ba-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="594ba-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="594ba-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="594ba-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="594ba-136">Request</span></span>
<span data-ttu-id="594ba-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="594ba-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="594ba-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="594ba-138">Response</span></span>
<span data-ttu-id="594ba-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="594ba-139">The following is an example of the response.</span></span> 

><span data-ttu-id="594ba-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="594ba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->