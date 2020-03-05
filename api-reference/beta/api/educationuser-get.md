---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e2b63cd90478eb199d30137a171846fa2c832e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423858"
---
# <a name="get-educationuser"></a><span data-ttu-id="ac219-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="ac219-103">Get educationUser</span></span>

<span data-ttu-id="ac219-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ac219-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac219-105">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ac219-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac219-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac219-106">Permissions</span></span>

<span data-ttu-id="ac219-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac219-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac219-109">Permission type</span></span>                        | <span data-ttu-id="ac219-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac219-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ac219-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac219-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac219-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ac219-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="ac219-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac219-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac219-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac219-114">Not supported.</span></span>                              |
| <span data-ttu-id="ac219-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac219-115">Application</span></span>                            | <span data-ttu-id="ac219-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac219-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

>[!IMPORTANT]
><span data-ttu-id="ac219-117">Ao usar escopos de permissão delegada, o Graph retornará somente um conjunto limitado de `id`propriedades `primaryRole`: `accountEnabled`, `displayName` `givenName` `surname`,,, `userPrincipalName`, `userType`, `onPremisesInfo`,,.</span><span class="sxs-lookup"><span data-stu-id="ac219-117">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`.</span></span> <span data-ttu-id="ac219-118">Se seu aplicativo exigir propriedades adicionais, você deve usar escopos de permissão de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac219-118">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="ac219-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac219-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac219-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac219-120">Optional query parameters</span></span>

<span data-ttu-id="ac219-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac219-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac219-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac219-122">Request headers</span></span>

| <span data-ttu-id="ac219-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac219-123">Header</span></span>        | <span data-ttu-id="ac219-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ac219-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ac219-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac219-125">Authorization</span></span> | <span data-ttu-id="ac219-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac219-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac219-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac219-128">Request body</span></span>

<span data-ttu-id="ac219-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac219-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac219-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac219-130">Response</span></span>

<span data-ttu-id="ac219-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac219-131">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac219-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac219-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac219-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac219-133">Request</span></span>

<span data-ttu-id="ac219-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac219-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac219-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac219-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="ac219-136">C#</span><span class="sxs-lookup"><span data-stu-id="ac219-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac219-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac219-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac219-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac219-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ac219-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac219-139">Response</span></span>

<span data-ttu-id="ac219-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac219-140">The following is an example of the response.</span></span> 

><span data-ttu-id="ac219-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac219-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
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
  },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
