---
title: Listar escolas
description: Recupere uma lista de escolas de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f69fb905fb886cd6dc06da90f0a8d997954b6cc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006987"
---
# <a name="list-schools"></a><span data-ttu-id="a0871-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="a0871-103">List schools</span></span>

<span data-ttu-id="a0871-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a0871-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0871-105">Recupere uma lista de escolas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a0871-105">Retrieve a list of schools for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0871-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0871-106">Permissions</span></span>

<span data-ttu-id="a0871-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0871-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0871-109">Permission type</span></span>                        | <span data-ttu-id="a0871-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0871-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a0871-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0871-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0871-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a0871-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a0871-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0871-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0871-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0871-114">Not supported.</span></span>                              |
| <span data-ttu-id="a0871-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0871-115">Application</span></span>                            | <span data-ttu-id="a0871-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0871-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a0871-117">Quando as permissões delegadas são usadas, somente os recursos do educationSchool de que o usuário de autenticação é um membro será retornado.</span><span class="sxs-lookup"><span data-stu-id="a0871-117">When delegated permissions are used, only educationSchool resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0871-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0871-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/schools
GET /education/users/{id}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0871-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0871-119">Optional query parameters</span></span>

<span data-ttu-id="a0871-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0871-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0871-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0871-121">Request headers</span></span>

| <span data-ttu-id="a0871-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0871-122">Header</span></span>        | <span data-ttu-id="a0871-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a0871-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a0871-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0871-124">Authorization</span></span> | <span data-ttu-id="a0871-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0871-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0871-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0871-127">Request body</span></span>

<span data-ttu-id="a0871-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0871-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0871-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0871-129">Response</span></span>

<span data-ttu-id="a0871-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0871-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0871-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0871-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0871-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0871-132">Request</span></span>

<span data-ttu-id="a0871-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0871-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0871-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0871-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="a0871-135">C#</span><span class="sxs-lookup"><span data-stu-id="a0871-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0871-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0871-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0871-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0871-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0871-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0871-138">Response</span></span>

<span data-ttu-id="a0871-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0871-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a0871-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0871-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


