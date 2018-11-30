---
title: Criar educationUser
description: Crie um novo usuário.
ms.openlocfilehash: d0edc82187d52df07d1954e8098cc4744c68ca15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036551"
---
# <a name="create-educationuser"></a><span data-ttu-id="670e0-103">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="670e0-103">Create educationUser</span></span>

> <span data-ttu-id="670e0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="670e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="670e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="670e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="670e0-106">Crie um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="670e0-106">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="670e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="670e0-107">Permissions</span></span>
<span data-ttu-id="670e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="670e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="670e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="670e0-110">Permission type</span></span>      | <span data-ttu-id="670e0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="670e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="670e0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="670e0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="670e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="670e0-113">Not supported.</span></span>  |
|<span data-ttu-id="670e0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="670e0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="670e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="670e0-115">Not supported.</span></span>  |
|<span data-ttu-id="670e0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="670e0-116">Application</span></span> | <span data-ttu-id="670e0-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="670e0-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="670e0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="670e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="670e0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="670e0-119">Request headers</span></span>
| <span data-ttu-id="670e0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="670e0-120">Header</span></span>       | <span data-ttu-id="670e0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="670e0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="670e0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="670e0-122">Authorization</span></span>  | <span data-ttu-id="670e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="670e0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="670e0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="670e0-125">Content-Type</span></span>  | <span data-ttu-id="670e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="670e0-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="670e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="670e0-127">Request body</span></span>
<span data-ttu-id="670e0-128">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="670e0-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="670e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="670e0-129">Response</span></span>
<span data-ttu-id="670e0-130">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="670e0-130">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="670e0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="670e0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="670e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="670e0-132">Request</span></span>
<span data-ttu-id="670e0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="670e0-133">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="670e0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="670e0-134">Response</span></span>
<span data-ttu-id="670e0-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="670e0-135">The following is an example of the response.</span></span> 

><span data-ttu-id="670e0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="670e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->