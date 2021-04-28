---
title: Listar usuários
description: Recupere uma lista de objetos user. Esses objetos de usuário incluirão propriedades específicas de educação.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 48253e39c70ff481eaab450e96428d4af63d523a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053143"
---
# <a name="list-users"></a><span data-ttu-id="dca25-104">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="dca25-104">List users</span></span>

<span data-ttu-id="dca25-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca25-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dca25-106">Recupera uma lista de objetos de usuário.</span><span class="sxs-lookup"><span data-stu-id="dca25-106">Retrieve a list of user objects.</span></span> <span data-ttu-id="dca25-107">Esses objetos de usuário incluirão propriedades específicas de educação.</span><span class="sxs-lookup"><span data-stu-id="dca25-107">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="dca25-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dca25-108">Permissions</span></span>
<span data-ttu-id="dca25-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca25-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dca25-111">Permission type</span></span>      | <span data-ttu-id="dca25-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dca25-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dca25-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dca25-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="dca25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dca25-114">Not supported.</span></span>  |
|<span data-ttu-id="dca25-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dca25-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dca25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dca25-116">Not supported.</span></span>  |
|<span data-ttu-id="dca25-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dca25-117">Application</span></span> | <span data-ttu-id="dca25-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca25-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="dca25-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dca25-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dca25-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dca25-120">Optional query parameters</span></span>
<span data-ttu-id="dca25-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dca25-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dca25-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dca25-122">Request headers</span></span>
| <span data-ttu-id="dca25-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dca25-123">Header</span></span>       | <span data-ttu-id="dca25-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dca25-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dca25-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dca25-125">Authorization</span></span>  | <span data-ttu-id="dca25-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dca25-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dca25-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dca25-128">Request body</span></span>
<span data-ttu-id="dca25-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dca25-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dca25-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca25-130">Response</span></span>
<span data-ttu-id="dca25-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dca25-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dca25-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dca25-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dca25-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dca25-133">Request</span></span>
<span data-ttu-id="dca25-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dca25-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dca25-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dca25-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationroot_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users
```
# <a name="c"></a>[<span data-ttu-id="dca25-136">C#</span><span class="sxs-lookup"><span data-stu-id="dca25-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationroot-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dca25-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dca25-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationroot-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dca25-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dca25-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationroot-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dca25-139">Java</span><span class="sxs-lookup"><span data-stu-id="dca25-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationroot-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dca25-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca25-140">Response</span></span>
<span data-ttu-id="dca25-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dca25-141">The following is an example of the response.</span></span> 

><span data-ttu-id="dca25-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dca25-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": null,
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
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
