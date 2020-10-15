---
title: Listar professores
description: Recupere uma lista de professores de uma aula. Os tokens delegados devem ser membros da aula para obterem a lista de professores.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e0257d7f467fe5232ea1281f7ab4be6662934d5a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461150"
---
# <a name="list-teachers"></a><span data-ttu-id="b2c83-104">Listar professores</span><span class="sxs-lookup"><span data-stu-id="b2c83-104">List teachers</span></span>

<span data-ttu-id="b2c83-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2c83-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2c83-106">Recupere uma lista de professores de uma aula.</span><span class="sxs-lookup"><span data-stu-id="b2c83-106">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="b2c83-107">Os tokens delegados devem ser membros da aula para obterem a lista de professores.</span><span class="sxs-lookup"><span data-stu-id="b2c83-107">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2c83-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="b2c83-108">Permissions</span></span>
<span data-ttu-id="b2c83-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2c83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2c83-111">Permission type</span></span>      | <span data-ttu-id="b2c83-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2c83-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2c83-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2c83-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b2c83-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="b2c83-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="b2c83-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2c83-115">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="b2c83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c83-116">Not supported.</span></span>  |
|<span data-ttu-id="b2c83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2c83-117">Application</span></span> | <span data-ttu-id="b2c83-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2c83-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b2c83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c83-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b2c83-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b2c83-120">Optional query parameters</span></span>
<span data-ttu-id="b2c83-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c83-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2c83-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c83-122">Request headers</span></span>
| <span data-ttu-id="b2c83-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2c83-123">Header</span></span>       | <span data-ttu-id="b2c83-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b2c83-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b2c83-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2c83-125">Authorization</span></span>  | <span data-ttu-id="b2c83-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2c83-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2c83-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c83-128">Request body</span></span>
<span data-ttu-id="b2c83-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2c83-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b2c83-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c83-130">Response</span></span>
<span data-ttu-id="b2c83-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c83-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2c83-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2c83-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2c83-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c83-133">Request</span></span>
<span data-ttu-id="b2c83-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2c83-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2c83-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c83-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
# <a name="c"></a>[<span data-ttu-id="b2c83-136">C#</span><span class="sxs-lookup"><span data-stu-id="b2c83-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teachers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2c83-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2c83-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teachers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2c83-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2c83-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teachers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2c83-139">Java</span><span class="sxs-lookup"><span data-stu-id="b2c83-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teachers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b2c83-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c83-140">Response</span></span>
<span data-ttu-id="b2c83-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c83-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b2c83-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2c83-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
