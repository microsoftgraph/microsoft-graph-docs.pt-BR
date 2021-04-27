---
title: Obter workPosition
description: Recupere as propriedades e as relações de um objeto workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a40f3b46d0cf929a05eb431bb9c431851794edeb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054669"
---
# <a name="get-workposition"></a><span data-ttu-id="9a909-103">Obter workPosition</span><span class="sxs-lookup"><span data-stu-id="9a909-103">Get workPosition</span></span>

<span data-ttu-id="9a909-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a909-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a909-105">Recupere as propriedades e as relações de um [objeto workPosition](../resources/workposition.md) no perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="9a909-105">Retrieve the properties and relationships of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a909-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a909-106">Permissions</span></span>

<span data-ttu-id="9a909-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a909-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a909-109">Permission type</span></span>                        | <span data-ttu-id="9a909-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a909-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="9a909-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a909-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a909-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a909-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9a909-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a909-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a909-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a909-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9a909-115">Application</span><span class="sxs-lookup"><span data-stu-id="9a909-115">Application</span></span>                            | <span data-ttu-id="9a909-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a909-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="9a909-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a909-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions/{id}
GET /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a909-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a909-118">Optional query parameters</span></span>

<span data-ttu-id="9a909-119">Este método dá suporte `$select` ao parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="9a909-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="9a909-120">Especifique uma lista de propriedades para incluir na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="9a909-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="9a909-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="9a909-121">For optimal performance, only select the subset of properties needed.</span></span>                                                                                                                                         |

## <a name="request-headers"></a><span data-ttu-id="9a909-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a909-122">Request headers</span></span>

| <span data-ttu-id="9a909-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9a909-123">Name</span></span>           |<span data-ttu-id="9a909-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a909-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="9a909-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a909-125">Authorization</span></span>  | <span data-ttu-id="9a909-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a909-p103">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="9a909-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a909-128">Request body</span></span>

<span data-ttu-id="9a909-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a909-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a909-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a909-130">Response</span></span>

<span data-ttu-id="9a909-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [workPosition](../resources/workposition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a909-131">If successful, this method returns a `200 OK` response code and the requested [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a909-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a909-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a909-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a909-133">Request</span></span>

<span data-ttu-id="9a909-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a909-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a909-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a909-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a909-136">C#</span><span class="sxs-lookup"><span data-stu-id="9a909-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a909-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a909-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a909-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a909-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a909-139">Java</span><span class="sxs-lookup"><span data-stu-id="9a909-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a909-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a909-140">Response</span></span>

<span data-ttu-id="9a909-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a909-141">The following is an example of the response.</span></span>

> <span data-ttu-id="9a909-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a909-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```


