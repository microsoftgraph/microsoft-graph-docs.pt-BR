---
title: Listar escolas de um educationUser
description: Recupere uma lista de escolas de um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 229c1182e45e9ac72e9ef984c9943823e4292536
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231875"
---
# <a name="list-schools-of-an-educationuser"></a><span data-ttu-id="a5bee-103">Listar escolas de um educationUser</span><span class="sxs-lookup"><span data-stu-id="a5bee-103">List schools of an educationUser</span></span>

<span data-ttu-id="a5bee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5bee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5bee-105">Recupere uma lista de escolas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a5bee-105">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="a5bee-106">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="a5bee-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="a5bee-107">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="a5bee-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5bee-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5bee-108">Permissions</span></span>

<span data-ttu-id="a5bee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5bee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5bee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5bee-111">Permission type</span></span>                        | <span data-ttu-id="a5bee-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5bee-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a5bee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5bee-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5bee-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a5bee-114">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a5bee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5bee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5bee-116">Not supported.</span></span>                              |
| <span data-ttu-id="a5bee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5bee-117">Application</span></span>                            | <span data-ttu-id="a5bee-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bee-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5bee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5bee-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{educationUserId}/schools
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5bee-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5bee-120">Optional query parameters</span></span>

<span data-ttu-id="a5bee-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5bee-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5bee-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bee-122">Request headers</span></span>

| <span data-ttu-id="a5bee-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5bee-123">Header</span></span>        | <span data-ttu-id="a5bee-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a5bee-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a5bee-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5bee-125">Authorization</span></span> | <span data-ttu-id="a5bee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5bee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5bee-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bee-128">Request body</span></span>

<span data-ttu-id="a5bee-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5bee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5bee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5bee-130">Response</span></span>

<span data-ttu-id="a5bee-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5bee-131">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5bee-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5bee-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5bee-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bee-133">Request</span></span>

<span data-ttu-id="a5bee-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5bee-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5bee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5bee-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/schools
```

# <a name="c"></a>[<span data-ttu-id="a5bee-136">C#</span><span class="sxs-lookup"><span data-stu-id="a5bee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5bee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5bee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5bee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5bee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5bee-139">Java</span><span class="sxs-lookup"><span data-stu-id="a5bee-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5bee-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5bee-140">Response</span></span>

<span data-ttu-id="a5bee-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5bee-141">The following is an example of the response.</span></span>

><span data-ttu-id="a5bee-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5bee-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
