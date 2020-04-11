---
title: Criar projectParticipation
description: Use esta API para criar um novo projectParticipation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16ffd76c33cf61d6e8ad7522d6e5978b9aad37dc
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228627"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="d9d3d-103">Criar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="d9d3d-103">Create projectParticipation</span></span>

<span data-ttu-id="d9d3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9d3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9d3d-105">Use esta API para criar um novo objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9d3d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9d3d-106">Permissions</span></span>

<span data-ttu-id="d9d3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9d3d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9d3d-109">Permission type</span></span>                        | <span data-ttu-id="d9d3d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9d3d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9d3d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9d3d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9d3d-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d9d3d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d9d3d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9d3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9d3d-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d9d3d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d9d3d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9d3d-115">Application</span></span>                            | <span data-ttu-id="d9d3d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d3d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d9d3d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d3d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="d9d3d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d3d-118">Request headers</span></span>

| <span data-ttu-id="d9d3d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d9d3d-119">Name</span></span>           |<span data-ttu-id="d9d3d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9d3d-120">Description</span></span>                  |
|:---------------|:----------                  |
| <span data-ttu-id="d9d3d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9d3d-121">Authorization</span></span>  | <span data-ttu-id="d9d3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d9d3d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9d3d-124">Content-Type</span></span>   | <span data-ttu-id="d9d3d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9d3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d3d-127">Request body</span></span>

<span data-ttu-id="d9d3d-128">No corpo da solicitação, forneça uma representação JSON do objeto [projectParticipation](../resources/projectparticipation.md) .</span><span class="sxs-lookup"><span data-stu-id="d9d3d-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9d3d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d3d-129">Response</span></span>

<span data-ttu-id="d9d3d-130">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [projectParticipation](../resources/projectparticipation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-130">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9d3d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9d3d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9d3d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d3d-132">Request</span></span>

<span data-ttu-id="d9d3d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9d3d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d9d3d-135">C#</span><span class="sxs-lookup"><span data-stu-id="d9d3d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9d3d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9d3d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9d3d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9d3d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9d3d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d3d-138">Response</span></span>

<span data-ttu-id="d9d3d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d9d3d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9d3d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create projectParticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
