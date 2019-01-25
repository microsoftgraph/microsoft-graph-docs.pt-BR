---
title: Lista de recursos
description: Lista os recursos associados a esse envio. O objeto de **submissionResource** é que um wrapper ao redor do objeto de recurso real do aluno está funcionando no. O wrapper também inclui um ponteiro para os recursos na atribuição se isso foi copiado da atribuição durante o processo de atribuir. Esses recursos estão a cópia de trabalho da atribuição. O **submittedResources** são os recursos que foram enviados para ser graduadas oficialmente.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b9069cb6ec20f65b82cacca8f862a05ff0af7b5d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526183"
---
# <a name="list-resources"></a><span data-ttu-id="3cab2-107">Lista de recursos</span><span class="sxs-lookup"><span data-stu-id="3cab2-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cab2-108">Lista os recursos associados a esse envio.</span><span class="sxs-lookup"><span data-stu-id="3cab2-108">List the resources associated with this submission.</span></span> <span data-ttu-id="3cab2-109">O objeto de **submissionResource** é que um wrapper ao redor do objeto de recurso real do aluno está funcionando no.</span><span class="sxs-lookup"><span data-stu-id="3cab2-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="3cab2-110">O wrapper também inclui um ponteiro para os recursos na atribuição se isso foi copiado da atribuição durante o processo de atribuir.</span><span class="sxs-lookup"><span data-stu-id="3cab2-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="3cab2-111">Esses recursos estão a cópia de trabalho da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3cab2-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="3cab2-112">O **submittedResources** são os recursos que foram enviados para ser graduadas oficialmente.</span><span class="sxs-lookup"><span data-stu-id="3cab2-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cab2-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cab2-113">Permissions</span></span>
<span data-ttu-id="3cab2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cab2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cab2-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cab2-116">Permission type</span></span>      | <span data-ttu-id="3cab2-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cab2-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cab2-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cab2-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cab2-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cab2-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3cab2-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cab2-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cab2-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cab2-121">Not supported.</span></span>   |
|<span data-ttu-id="3cab2-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cab2-122">Application</span></span> | <span data-ttu-id="3cab2-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cab2-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3cab2-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cab2-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cab2-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3cab2-125">Optional query parameters</span></span>
<span data-ttu-id="3cab2-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3cab2-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cab2-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cab2-127">Request headers</span></span>
| <span data-ttu-id="3cab2-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cab2-128">Header</span></span>       | <span data-ttu-id="3cab2-129">Valor</span><span class="sxs-lookup"><span data-stu-id="3cab2-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cab2-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cab2-130">Authorization</span></span>  | <span data-ttu-id="3cab2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cab2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cab2-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cab2-133">Request body</span></span>
<span data-ttu-id="3cab2-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cab2-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3cab2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cab2-135">Response</span></span>
<span data-ttu-id="3cab2-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [educationSubmissionResource](../resources/educationsubmissionresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cab2-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3cab2-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cab2-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cab2-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cab2-138">Request</span></span>
<span data-ttu-id="3cab2-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cab2-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="3cab2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cab2-140">Response</span></span>
<span data-ttu-id="3cab2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cab2-141">The following is an example of the response.</span></span> 

><span data-ttu-id="3cab2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cab2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
