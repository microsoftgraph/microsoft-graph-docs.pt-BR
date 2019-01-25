---
title: Criar educationUser
description: Crie um novo usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f3a687aa7193188f39eebacf7f448014c5309f20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525168"
---
# <a name="create-educationuser"></a><span data-ttu-id="ab42d-103">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="ab42d-103">Create educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab42d-104">Crie um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="ab42d-104">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="ab42d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab42d-105">Permissions</span></span>
<span data-ttu-id="ab42d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab42d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab42d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab42d-108">Permission type</span></span>      | <span data-ttu-id="ab42d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab42d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab42d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab42d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ab42d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab42d-111">Not supported.</span></span>  |
|<span data-ttu-id="ab42d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab42d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ab42d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab42d-113">Not supported.</span></span>  |
|<span data-ttu-id="ab42d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab42d-114">Application</span></span> | <span data-ttu-id="ab42d-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab42d-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ab42d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab42d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="ab42d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab42d-117">Request headers</span></span>
| <span data-ttu-id="ab42d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab42d-118">Header</span></span>       | <span data-ttu-id="ab42d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ab42d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab42d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab42d-120">Authorization</span></span>  | <span data-ttu-id="ab42d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab42d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab42d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab42d-123">Content-Type</span></span>  | <span data-ttu-id="ab42d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab42d-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab42d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab42d-125">Request body</span></span>
<span data-ttu-id="ab42d-126">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="ab42d-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ab42d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab42d-127">Response</span></span>
<span data-ttu-id="ab42d-128">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab42d-128">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab42d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab42d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab42d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab42d-130">Request</span></span>
<span data-ttu-id="ab42d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab42d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

##### <a name="response"></a><span data-ttu-id="ab42d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab42d-132">Response</span></span>
<span data-ttu-id="ab42d-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab42d-133">The following is an example of the response.</span></span> 

><span data-ttu-id="ab42d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab42d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationroot-post-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
