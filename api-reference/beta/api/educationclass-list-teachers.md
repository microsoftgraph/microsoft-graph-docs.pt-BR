---
title: Listar professores
description: Recupere uma lista de professores de uma aula. Os tokens delegados devem ser membros da aula para obterem a lista de professores.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b4686c8399dd91d047d1f2f03f814956db32c69c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324008"
---
# <a name="list-teachers"></a><span data-ttu-id="c2473-104">Listar professores</span><span class="sxs-lookup"><span data-stu-id="c2473-104">List teachers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2473-105">Recupere uma lista de professores de uma aula.</span><span class="sxs-lookup"><span data-stu-id="c2473-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="c2473-106">Os tokens delegados devem ser membros da aula para obterem a lista de professores.</span><span class="sxs-lookup"><span data-stu-id="c2473-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2473-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2473-107">Permissions</span></span>
<span data-ttu-id="c2473-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2473-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2473-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2473-110">Permission type</span></span>      | <span data-ttu-id="c2473-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2473-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2473-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2473-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c2473-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c2473-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c2473-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2473-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="c2473-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2473-115">Not supported.</span></span>  |
|<span data-ttu-id="c2473-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2473-116">Application</span></span> | <span data-ttu-id="c2473-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2473-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c2473-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2473-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2473-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2473-119">Optional query parameters</span></span>
<span data-ttu-id="c2473-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2473-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2473-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2473-121">Request headers</span></span>
| <span data-ttu-id="c2473-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2473-122">Header</span></span>       | <span data-ttu-id="c2473-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c2473-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2473-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2473-124">Authorization</span></span>  | <span data-ttu-id="c2473-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2473-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2473-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2473-127">Request body</span></span>
<span data-ttu-id="c2473-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2473-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2473-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2473-129">Response</span></span>
<span data-ttu-id="c2473-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2473-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2473-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2473-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2473-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2473-132">Request</span></span>
<span data-ttu-id="c2473-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2473-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2473-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2473-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023/teachers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2473-135">C#</span><span class="sxs-lookup"><span data-stu-id="c2473-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teachers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2473-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2473-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teachers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2473-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2473-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teachers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2473-138">Java</span><span class="sxs-lookup"><span data-stu-id="c2473-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teachers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2473-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2473-139">Response</span></span>
<span data-ttu-id="c2473-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2473-140">The following is an example of the response.</span></span> 

><span data-ttu-id="c2473-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2473-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
