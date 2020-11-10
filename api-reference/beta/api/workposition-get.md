---
title: Obter workPosition
description: Recupere as propriedades e os relacionamentos de um objeto workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ad4d47d9fd081a56a64af93ceb676afb52a56625
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979974"
---
# <a name="get-workposition"></a><span data-ttu-id="5fe30-103">Obter workPosition</span><span class="sxs-lookup"><span data-stu-id="5fe30-103">Get workPosition</span></span>

<span data-ttu-id="5fe30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fe30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fe30-105">Recupere as propriedades e os relacionamentos de um objeto [workPosition](../resources/workposition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5fe30-105">Retrieve the properties and relationships of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5fe30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fe30-106">Permissions</span></span>

<span data-ttu-id="5fe30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fe30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fe30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fe30-109">Permission type</span></span>                        | <span data-ttu-id="5fe30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fe30-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5fe30-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fe30-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fe30-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5fe30-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5fe30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fe30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fe30-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5fe30-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5fe30-115">Application</span><span class="sxs-lookup"><span data-stu-id="5fe30-115">Application</span></span>                            | <span data-ttu-id="5fe30-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5fe30-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5fe30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fe30-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions/{id}
GET /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fe30-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5fe30-118">Optional query parameters</span></span>

<span data-ttu-id="5fe30-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="5fe30-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="5fe30-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="5fe30-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="5fe30-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="5fe30-121">For optimal performance, only select the subset of properties needed.</span></span>                                                                                                                                         |

## <a name="request-headers"></a><span data-ttu-id="5fe30-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fe30-122">Request headers</span></span>

| <span data-ttu-id="5fe30-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5fe30-123">Name</span></span>           |<span data-ttu-id="5fe30-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fe30-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5fe30-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fe30-125">Authorization</span></span>  | <span data-ttu-id="5fe30-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fe30-p103">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="5fe30-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fe30-128">Request body</span></span>

<span data-ttu-id="5fe30-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fe30-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fe30-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fe30-130">Response</span></span>

<span data-ttu-id="5fe30-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [workPosition](../resources/workposition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe30-131">If successful, this method returns a `200 OK` response code and the requested [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fe30-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5fe30-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fe30-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fe30-133">Request</span></span>

<span data-ttu-id="5fe30-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fe30-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5fe30-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fe30-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="5fe30-136">C#</span><span class="sxs-lookup"><span data-stu-id="5fe30-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fe30-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fe30-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fe30-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fe30-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fe30-139">Java</span><span class="sxs-lookup"><span data-stu-id="5fe30-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5fe30-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fe30-140">Response</span></span>

<span data-ttu-id="5fe30-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe30-141">The following is an example of the response.</span></span>

> <span data-ttu-id="5fe30-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fe30-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


