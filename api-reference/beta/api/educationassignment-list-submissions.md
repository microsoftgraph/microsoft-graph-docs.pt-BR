---
title: Envios de lista
description: Liste todos os envios associados a essa atribuição. Um professor pode obter todos os envios enquanto um estudante só pode obter envios que eles estão associados.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47088cb7a4290827ce75e35d3ac705b31addefac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510635"
---
# <a name="list-submissions"></a><span data-ttu-id="41c31-104">Envios de lista</span><span class="sxs-lookup"><span data-stu-id="41c31-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41c31-105">Liste todos os envios associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="41c31-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="41c31-106">Um professor pode obter todos os envios enquanto um estudante só pode obter envios que eles estão associados.</span><span class="sxs-lookup"><span data-stu-id="41c31-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="41c31-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="41c31-107">Permissions</span></span>
<span data-ttu-id="41c31-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c31-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41c31-110">Permission type</span></span>      | <span data-ttu-id="41c31-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41c31-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41c31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41c31-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="41c31-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41c31-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="41c31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41c31-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="41c31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41c31-115">Not supported.</span></span>  |
|<span data-ttu-id="41c31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41c31-116">Application</span></span> | <span data-ttu-id="41c31-117">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="41c31-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="41c31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41c31-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41c31-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41c31-119">Optional query parameters</span></span>
<span data-ttu-id="41c31-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41c31-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41c31-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41c31-121">Request headers</span></span>
| <span data-ttu-id="41c31-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41c31-122">Header</span></span>       | <span data-ttu-id="41c31-123">Valor</span><span class="sxs-lookup"><span data-stu-id="41c31-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41c31-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="41c31-124">Authorization</span></span>  | <span data-ttu-id="41c31-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41c31-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41c31-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41c31-127">Request body</span></span>
<span data-ttu-id="41c31-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41c31-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="41c31-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c31-129">Response</span></span>
<span data-ttu-id="41c31-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [educationSubmission](../resources/educationsubmission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41c31-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41c31-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41c31-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41c31-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41c31-132">Request</span></span>
<span data-ttu-id="41c31-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41c31-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="41c31-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="41c31-134">Response</span></span>
<span data-ttu-id="41c31-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41c31-135">The following is an example of the response.</span></span> 

><span data-ttu-id="41c31-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41c31-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41c31-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41c31-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "feedback": {
        "text": {
          "content": "Good work!",
          "contentType": "Text"
        },
        "feedbackDateTime": "2014-01-01T00:00:00Z",
        "feedbackBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "@odata.type": "microsoft.graph.educationFeedback"
        },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-submissions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
