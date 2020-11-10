---
title: Obter educationalActivity
description: Recupere as propriedades e os relacionamentos de um objeto educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d0a789ab302d8a130d81c7acf06978ce841f081a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966661"
---
# <a name="get-educationalactivity"></a><span data-ttu-id="92d83-103">Obter educationalActivity</span><span class="sxs-lookup"><span data-stu-id="92d83-103">Get educationalActivity</span></span>

<span data-ttu-id="92d83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d83-105">Recupere as propriedades e os relacionamentos de um objeto [educationalActivity](../resources/educationalactivity.md) de um perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="92d83-105">Retrieve the properties and relationships of an [educationalActivity](../resources/educationalactivity.md) object from a users profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="92d83-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92d83-106">Permissions</span></span>

<span data-ttu-id="92d83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92d83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92d83-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92d83-109">Permission type</span></span>                        | <span data-ttu-id="92d83-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92d83-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="92d83-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92d83-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92d83-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92d83-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="92d83-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92d83-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92d83-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92d83-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="92d83-115">Application</span><span class="sxs-lookup"><span data-stu-id="92d83-115">Application</span></span>                            | <span data-ttu-id="92d83-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92d83-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="92d83-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92d83-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities/{id}
GET /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92d83-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92d83-118">Optional query parameters</span></span>

<span data-ttu-id="92d83-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="92d83-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="92d83-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="92d83-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="92d83-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="92d83-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92d83-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92d83-122">Request headers</span></span>

|<span data-ttu-id="92d83-123">Nome</span><span class="sxs-lookup"><span data-stu-id="92d83-123">Name</span></span>            |<span data-ttu-id="92d83-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d83-124">Description</span></span>                  |
|:---------------|:----------------------------|
|<span data-ttu-id="92d83-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="92d83-125">Authorization</span></span>   |<span data-ttu-id="92d83-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92d83-p103">Bearer {token}. Required.</span></span>    |

## <a name="request-body"></a><span data-ttu-id="92d83-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92d83-128">Request body</span></span>

<span data-ttu-id="92d83-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92d83-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92d83-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d83-130">Response</span></span>

<span data-ttu-id="92d83-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [educationalActivity](../resources/educationalactivity.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d83-131">If successful, this method returns a `200 OK` response code and the requested [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92d83-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92d83-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92d83-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92d83-133">Request</span></span>

<span data-ttu-id="92d83-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92d83-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92d83-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d83-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationalactivity"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="c"></a>[<span data-ttu-id="92d83-136">C#</span><span class="sxs-lookup"><span data-stu-id="92d83-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d83-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d83-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d83-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d83-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d83-139">Java</span><span class="sxs-lookup"><span data-stu-id="92d83-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationalactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="92d83-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d83-140">Response</span></span>

<span data-ttu-id="92d83-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92d83-141">The following is an example of the response.</span></span>

> <span data-ttu-id="92d83-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92d83-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
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
  "completionMonthYear": "Date",
  "endMonthYear": "Date",
  "institution": {
    "description": null,
    "displayName": "Colorado State University",
    "location": {
      "type": "business",
      "postOfficeBox": null,
      "street": "12000 E Prospect Rd",
      "city": "Fort Collins",
      "state": "Colorado",
      "countryOrRegion": "USA",
      "postalCode": "80525"
    },
    "webUrl": "https://www.colostate.edu"
  },
  "program": {
    "abbreviation": "MBA",
    "activities": null,
    "awards": null,
    "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
    "displayName": "Master of Business Administration",
    "fieldsOfStudy": null,
    "grade": "3.9",
    "notes": null,
    "webUrl": "https://biz.colostate.edu"
  },
  "startMonthYear": "Date"
}
```


