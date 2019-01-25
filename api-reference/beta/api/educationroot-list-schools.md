---
title: Listar educationSchools
description: Recupere uma lista de todos os objetos de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cf10d18188f09ee7c65195358e224f183ffd906e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515724"
---
# <a name="list-educationschools"></a><span data-ttu-id="7ff86-103">Listar educationSchools</span><span class="sxs-lookup"><span data-stu-id="7ff86-103">List educationSchools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff86-104">Recupere uma lista de todos os objetos de escola.</span><span class="sxs-lookup"><span data-stu-id="7ff86-104">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ff86-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ff86-105">Permissions</span></span>
<span data-ttu-id="7ff86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff86-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ff86-108">Permission type</span></span>      | <span data-ttu-id="7ff86-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ff86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ff86-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ff86-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7ff86-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="7ff86-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="7ff86-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ff86-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7ff86-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ff86-113">Not supported.</span></span>  |
|<span data-ttu-id="7ff86-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ff86-114">Application</span></span> | <span data-ttu-id="7ff86-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff86-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7ff86-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff86-116">HTTP request</span></span>
<span data-ttu-id="7ff86-117"><!-- { "blockType": "ignored" } -->' ' GET/educação/escolas de http</span><span class="sxs-lookup"><span data-stu-id="7ff86-117"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
```
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.

## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.
## Example
##### Request
The following is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools
```
##### <a name="response"></a><span data-ttu-id="7ff86-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ff86-118">Response</span></span>
<span data-ttu-id="7ff86-119">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ff86-119">The following is an example of the response.</span></span> 

><span data-ttu-id="7ff86-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ff86-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationroot-list-schools.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
