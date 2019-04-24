---
title: Listar educationAssignmentResources
description: Obter todos os recursos associados a essa atribuição.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5556210604ce6b0c273a0e4d89e1a792d2639b12
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464772"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="53893-103">Listar educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="53893-103">List educationAssignmentResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53893-104">Obter todos os recursos associados a essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="53893-104">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="53893-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="53893-105">Permissions</span></span>
<span data-ttu-id="53893-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53893-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53893-108">Permission type</span></span>      | <span data-ttu-id="53893-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53893-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53893-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53893-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="53893-111">EduAssignments. ReadBasic, EduAssignments. ReadWriteBasic, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53893-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="53893-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53893-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53893-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53893-113">Not supported.</span></span>  |
|<span data-ttu-id="53893-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53893-114">Application</span></span> | <span data-ttu-id="53893-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53893-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="53893-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53893-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53893-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="53893-117">Optional query parameters</span></span>
<span data-ttu-id="53893-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="53893-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53893-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53893-119">Request headers</span></span>
| <span data-ttu-id="53893-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53893-120">Header</span></span>       | <span data-ttu-id="53893-121">Valor</span><span class="sxs-lookup"><span data-stu-id="53893-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53893-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="53893-122">Authorization</span></span>  | <span data-ttu-id="53893-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53893-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53893-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53893-125">Request body</span></span>
<span data-ttu-id="53893-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53893-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53893-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="53893-127">Response</span></span>
<span data-ttu-id="53893-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53893-128">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53893-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53893-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53893-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53893-130">Request</span></span>
<span data-ttu-id="53893-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="53893-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="53893-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="53893-132">Response</span></span>
<span data-ttu-id="53893-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="53893-133">The following is an example of the response.</span></span> 

><span data-ttu-id="53893-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53893-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
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
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
      "resource": {
          "@odata.type": "#microsoft.graph.educationWordResource",
          "displayName": "Report.docx",
          "createdDateTime": "2017-10-21T07:52:53.9863696Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
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
    "Error: /api-reference/beta/api/educationassignment-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
