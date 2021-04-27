---
title: Listar tarefas
description: Recupere uma lista de objetos de atribuição. Um professor ou um aplicativo que executa com permissões de aplicativo tem permissão para ver todos os objetos de atribuição da classe. Os alunos só podem ver atribuições atribuídas a eles.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a301303904cb042cf2dd87f7bb51b04957cd34bc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043966"
---
# <a name="list-assignments"></a><span data-ttu-id="a811c-105">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="a811c-105">List assignments</span></span>

<span data-ttu-id="a811c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a811c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a811c-107">Recupere uma lista de objetos de atribuição.</span><span class="sxs-lookup"><span data-stu-id="a811c-107">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="a811c-108">Um professor ou um aplicativo que executa com permissões de aplicativo tem permissão para ver todos os objetos de atribuição da classe.</span><span class="sxs-lookup"><span data-stu-id="a811c-108">A teacher or an application executing with application permissions is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="a811c-109">Os alunos só podem ver atribuições atribuídas a eles.</span><span class="sxs-lookup"><span data-stu-id="a811c-109">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="a811c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a811c-110">Permissions</span></span>

<span data-ttu-id="a811c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a811c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a811c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a811c-113">Permission type</span></span>                        | <span data-ttu-id="a811c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a811c-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a811c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a811c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a811c-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a811c-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a811c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a811c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a811c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a811c-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="a811c-119">Application</span><span class="sxs-lookup"><span data-stu-id="a811c-119">Application</span></span>                            | <span data-ttu-id="a811c-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a811c-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a811c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a811c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a811c-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a811c-122">Optional query parameters</span></span>
<span data-ttu-id="a811c-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a811c-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a811c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a811c-124">Request headers</span></span>

| <span data-ttu-id="a811c-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a811c-125">Header</span></span>        | <span data-ttu-id="a811c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a811c-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a811c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a811c-127">Authorization</span></span> | <span data-ttu-id="a811c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a811c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a811c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a811c-130">Request body</span></span>

<span data-ttu-id="a811c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a811c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a811c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a811c-132">Response</span></span>

<span data-ttu-id="a811c-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a811c-133">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a811c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a811c-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a811c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a811c-135">Request</span></span>

<span data-ttu-id="a811c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a811c-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="a811c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a811c-137">Response</span></span>

<span data-ttu-id="a811c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a811c-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a811c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a811c-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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