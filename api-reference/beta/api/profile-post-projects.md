---
title: Criar projectParticipation
description: Use esta API para criar um novo projectParticipation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a186c9f2e44f2772dc7de065d92386e270ab9bc9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937662"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="9460b-103">Criar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="9460b-103">Create projectParticipation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9460b-104">Use esta API para criar um novo objeto [projectParticipation](../resources/projectParticipation.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9460b-104">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9460b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9460b-105">Permissions</span></span>

<span data-ttu-id="9460b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9460b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9460b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9460b-108">Permission type</span></span>                        | <span data-ttu-id="9460b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9460b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9460b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9460b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9460b-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9460b-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9460b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9460b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9460b-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9460b-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9460b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9460b-114">Application</span></span>                            | <span data-ttu-id="9460b-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9460b-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9460b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9460b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="9460b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9460b-117">Request headers</span></span>

| <span data-ttu-id="9460b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9460b-118">Name</span></span>      |<span data-ttu-id="9460b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9460b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9460b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9460b-120">Authorization</span></span>  | <span data-ttu-id="9460b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9460b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9460b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9460b-123">Content-Type</span></span>   | <span data-ttu-id="9460b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9460b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9460b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9460b-126">Request body</span></span>

<span data-ttu-id="9460b-127">No corpo da solicitação, forneça uma representação JSON do objeto [projectParticipation](../resources/projectparticipation.md) .</span><span class="sxs-lookup"><span data-stu-id="9460b-127">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9460b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9460b-128">Response</span></span>

<span data-ttu-id="9460b-129">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [projectParticipation](../resources/projectparticipation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9460b-129">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9460b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9460b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9460b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9460b-131">Request</span></span>

<span data-ttu-id="9460b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9460b-132">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9460b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9460b-133">Response</span></span>

<span data-ttu-id="9460b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9460b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9460b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9460b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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