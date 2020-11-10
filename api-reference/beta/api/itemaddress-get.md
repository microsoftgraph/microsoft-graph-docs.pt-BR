---
title: Get endereço
description: Leia as propriedades e os relacionamentos de um objeto item.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 11759bcc9d8529e14ef44df0de2932debea6ce1a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969971"
---
# <a name="get-itemaddress"></a><span data-ttu-id="6a0f0-103">Get endereço</span><span class="sxs-lookup"><span data-stu-id="6a0f0-103">Get itemAddress</span></span>
<span data-ttu-id="6a0f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a0f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a0f0-105">Leia as propriedades e os relacionamentos de [um objeto](../resources/itemaddress.md) item.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-105">Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a0f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a0f0-106">Permissions</span></span>

<span data-ttu-id="6a0f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a0f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a0f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a0f0-109">Permission type</span></span>                        | <span data-ttu-id="6a0f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a0f0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6a0f0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a0f0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a0f0-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a0f0-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6a0f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a0f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a0f0-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a0f0-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6a0f0-115">Application</span><span class="sxs-lookup"><span data-stu-id="6a0f0-115">Application</span></span>                            | <span data-ttu-id="6a0f0-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a0f0-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="6a0f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a0f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/addresses/{id}
GET /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a0f0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a0f0-118">Optional query parameters</span></span>

<span data-ttu-id="6a0f0-119">Este método dá suporte ao `$select` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="6a0f0-120">Especifique uma lista de propriedades a serem incluídas na resposta, separando-as por vírgulas.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="6a0f0-121">Para obter o desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a0f0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a0f0-122">Request headers</span></span>
|<span data-ttu-id="6a0f0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6a0f0-123">Name</span></span>|<span data-ttu-id="6a0f0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a0f0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a0f0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a0f0-125">Authorization</span></span>|<span data-ttu-id="6a0f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a0f0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a0f0-128">Request body</span></span>
<span data-ttu-id="6a0f0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a0f0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a0f0-130">Response</span></span>

<span data-ttu-id="6a0f0-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [myAddress](../resources/itemaddress.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-131">If successful, this method returns a `200 OK` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a0f0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a0f0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a0f0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a0f0-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="6a0f0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a0f0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemaddress"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="6a0f0-135">C#</span><span class="sxs-lookup"><span data-stu-id="6a0f0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a0f0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a0f0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a0f0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a0f0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a0f0-138">Java</span><span class="sxs-lookup"><span data-stu-id="6a0f0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itemaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6a0f0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a0f0-139">Response</span></span>

<span data-ttu-id="6a0f0-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6a0f0-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  },
  "geoCoordinates": null
}
```


