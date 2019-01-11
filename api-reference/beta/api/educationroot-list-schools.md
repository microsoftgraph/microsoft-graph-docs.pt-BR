---
title: Listar educationSchools
description: Recupere uma lista de todos os objetos de escola.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0bef367932b89ba998405f5da8b27b7af54efb94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813577"
---
# <a name="list-educationschools"></a><span data-ttu-id="e67b1-103">Listar educationSchools</span><span class="sxs-lookup"><span data-stu-id="e67b1-103">List educationSchools</span></span>

> <span data-ttu-id="e67b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e67b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e67b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e67b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e67b1-106">Recupere uma lista de todos os objetos de escola.</span><span class="sxs-lookup"><span data-stu-id="e67b1-106">Retrieve a list of all school objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e67b1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e67b1-107">Permissions</span></span>
<span data-ttu-id="e67b1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e67b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e67b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e67b1-110">Permission type</span></span>      | <span data-ttu-id="e67b1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e67b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e67b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e67b1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e67b1-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e67b1-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e67b1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e67b1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e67b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e67b1-115">Not supported.</span></span>  |
|<span data-ttu-id="e67b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e67b1-116">Application</span></span> | <span data-ttu-id="e67b1-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e67b1-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e67b1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e67b1-118">HTTP request</span></span>
<span data-ttu-id="e67b1-119"><!-- { "blockType": "ignored" } -->' ' GET/educação/escolas de http</span><span class="sxs-lookup"><span data-stu-id="e67b1-119"><!-- { "blockType": "ignored" } --> \`\`\`http GET /education/schools</span></span>
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
##### <a name="response"></a><span data-ttu-id="e67b1-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="e67b1-120">Response</span></span>
<span data-ttu-id="e67b1-121">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e67b1-121">The following is an example of the response.</span></span> 

><span data-ttu-id="e67b1-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e67b1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
