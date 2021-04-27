---
title: Listar professores
description: Recupere uma lista de professores de uma aula. Os tokens delegados devem ser membros da aula para obterem a lista de professores.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3428127076947f1fe6bc9193a49829a6c3299a2c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043889"
---
# <a name="list-teachers"></a><span data-ttu-id="e4bc0-104">Listar professores</span><span class="sxs-lookup"><span data-stu-id="e4bc0-104">List teachers</span></span>

<span data-ttu-id="e4bc0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4bc0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4bc0-106">Recupere uma lista de professores de uma aula.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-106">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="e4bc0-107">Os tokens delegados devem ser membros da aula para obterem a lista de professores.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-107">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4bc0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4bc0-108">Permissions</span></span>
<span data-ttu-id="e4bc0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4bc0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bc0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4bc0-111">Permission type</span></span>      | <span data-ttu-id="e4bc0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4bc0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4bc0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4bc0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e4bc0-114">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e4bc0-114">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="e4bc0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4bc0-115">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="e4bc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-116">Not supported.</span></span>  |
|<span data-ttu-id="e4bc0-117">Application</span><span class="sxs-lookup"><span data-stu-id="e4bc0-117">Application</span></span> | <span data-ttu-id="e4bc0-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bc0-118">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e4bc0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4bc0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4bc0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4bc0-120">Optional query parameters</span></span>
<span data-ttu-id="e4bc0-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4bc0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bc0-122">Request headers</span></span>
| <span data-ttu-id="e4bc0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4bc0-123">Header</span></span>       | <span data-ttu-id="e4bc0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e4bc0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4bc0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4bc0-125">Authorization</span></span>  | <span data-ttu-id="e4bc0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4bc0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bc0-128">Request body</span></span>
<span data-ttu-id="e4bc0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e4bc0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4bc0-130">Response</span></span>
<span data-ttu-id="e4bc0-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-131">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4bc0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4bc0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4bc0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bc0-133">Request</span></span>
<span data-ttu-id="e4bc0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4bc0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4bc0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11023/teachers
```
# <a name="c"></a>[<span data-ttu-id="e4bc0-136">C#</span><span class="sxs-lookup"><span data-stu-id="e4bc0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teachers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4bc0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4bc0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teachers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4bc0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4bc0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teachers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4bc0-139">Java</span><span class="sxs-lookup"><span data-stu-id="e4bc0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teachers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4bc0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4bc0-140">Response</span></span>
<span data-ttu-id="e4bc0-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-141">The following is an example of the response.</span></span> 

><span data-ttu-id="e4bc0-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4bc0-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
