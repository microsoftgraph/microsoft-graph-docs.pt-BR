---
title: Criar educationSchool
description: Crie uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6fda4389c74b975eb1d6a622b153dfa4459f8870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945472"
---
# <a name="create-educationschool"></a><span data-ttu-id="a22e5-103">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="a22e5-103">Create educationSchool</span></span>

> <span data-ttu-id="a22e5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a22e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a22e5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a22e5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a22e5-106">Crie uma escola.</span><span class="sxs-lookup"><span data-stu-id="a22e5-106">Create a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="a22e5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a22e5-107">Permissions</span></span>
<span data-ttu-id="a22e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a22e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a22e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a22e5-110">Permission type</span></span>      | <span data-ttu-id="a22e5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a22e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a22e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a22e5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a22e5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a22e5-113">Not supported.</span></span>  |
|<span data-ttu-id="a22e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a22e5-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a22e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a22e5-115">Not supported.</span></span>  |
|<span data-ttu-id="a22e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a22e5-116">Application</span></span> | <span data-ttu-id="a22e5-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a22e5-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a22e5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a22e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools
```
## <a name="request-headers"></a><span data-ttu-id="a22e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a22e5-119">Request headers</span></span>
| <span data-ttu-id="a22e5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a22e5-120">Header</span></span>       | <span data-ttu-id="a22e5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a22e5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a22e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a22e5-122">Authorization</span></span>  | <span data-ttu-id="a22e5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a22e5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a22e5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a22e5-125">Content-Type</span></span>  | <span data-ttu-id="a22e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a22e5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a22e5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a22e5-127">Request body</span></span>
<span data-ttu-id="a22e5-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="a22e5-128">In the request body, supply a JSON representation of an [educationSchool](../resources/educationschool.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a22e5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22e5-129">Response</span></span>
<span data-ttu-id="a22e5-130">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a22e5-130">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a22e5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a22e5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a22e5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a22e5-132">Request</span></span>
<span data-ttu-id="a22e5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a22e5-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

##### <a name="response"></a><span data-ttu-id="a22e5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22e5-134">Response</span></span>
<span data-ttu-id="a22e5-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a22e5-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a22e5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a22e5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
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
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
