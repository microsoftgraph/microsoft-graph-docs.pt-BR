---
title: Obter educationUser
description: Recupere as propriedades e as relações de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 893f484eaf03ef5102a22e70fdb946251af0cbd9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042881"
---
# <a name="get-educationuser"></a><span data-ttu-id="ff990-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="ff990-103">Get educationUser</span></span>

<span data-ttu-id="ff990-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff990-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff990-105">Recupere as propriedades e as relações de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ff990-105">Retrieve the properties and relationships of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff990-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff990-106">Permissions</span></span>

<span data-ttu-id="ff990-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> [!NOTE]
> <span data-ttu-id="ff990-109">Se o token delegado for usado, os membros poderão ver apenas informações sobre sua própria conta.</span><span class="sxs-lookup"><span data-stu-id="ff990-109">If the delegated token is used, members can only see information about their own account.</span></span> <span data-ttu-id="ff990-110">Nesse caso, use o recurso `beta/education/me/users`.</span><span class="sxs-lookup"><span data-stu-id="ff990-110">Use the `beta/education/me/users` resource in this case.</span></span>

| <span data-ttu-id="ff990-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff990-111">Permission type</span></span>                        | <span data-ttu-id="ff990-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff990-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ff990-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff990-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff990-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ff990-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="ff990-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff990-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff990-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff990-116">Not supported.</span></span>                              |
| <span data-ttu-id="ff990-117">Application</span><span class="sxs-lookup"><span data-stu-id="ff990-117">Application</span></span>                            | <span data-ttu-id="ff990-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff990-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="ff990-119">Ao usar escopos de permissão delegados, Graph retornará apenas um conjunto limitado de propriedades: `id` , , , , , , , , , `primaryRole` , `accountEnabled` , `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` `teacher/externalId` .</span><span class="sxs-lookup"><span data-stu-id="ff990-119">When using Delegated permission scopes, Graph will only return a limited set of properties: `id`, `primaryRole`, `accountEnabled`, `displayName`, `givenName`, `surname`, `userPrincipalName`, `userType`, `onPremisesInfo`, `student/externalId`, `teacher/externalId`.</span></span> <span data-ttu-id="ff990-120">Se seu aplicativo exigir propriedades adicionais, você deve usar escopos de permissão application.</span><span class="sxs-lookup"><span data-stu-id="ff990-120">If your application requires additional properties, you must use Application permission scopes.</span></span>

## <a name="http-request"></a><span data-ttu-id="ff990-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff990-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me
GET /education/users/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff990-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff990-122">Optional query parameters</span></span>

<span data-ttu-id="ff990-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff990-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff990-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff990-124">Request headers</span></span>

| <span data-ttu-id="ff990-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff990-125">Header</span></span>        | <span data-ttu-id="ff990-126">Valor</span><span class="sxs-lookup"><span data-stu-id="ff990-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ff990-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff990-127">Authorization</span></span> | <span data-ttu-id="ff990-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff990-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff990-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff990-130">Request body</span></span>

<span data-ttu-id="ff990-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff990-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff990-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff990-132">Response</span></span>

<span data-ttu-id="ff990-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff990-133">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff990-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff990-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ff990-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff990-135">Request</span></span>

<span data-ttu-id="ff990-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff990-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff990-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff990-137">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationuser_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/13012
```

# <a name="c"></a>[<span data-ttu-id="ff990-138">C#</span><span class="sxs-lookup"><span data-stu-id="ff990-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff990-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff990-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff990-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff990-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-2-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff990-141">Java</span><span class="sxs-lookup"><span data-stu-id="ff990-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff990-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff990-142">Response</span></span>

<span data-ttu-id="ff990-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff990-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ff990-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ff990-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
