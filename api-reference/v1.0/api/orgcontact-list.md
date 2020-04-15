---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais desta organização.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c6ce5caffdc24306b93e61fce70802a04a4267b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463744"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="74e54-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="74e54-103">List orgContacts</span></span>

<span data-ttu-id="74e54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74e54-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74e54-105">Obtenha a lista de [contatos organizacionais](../resources/orgcontact.md) para esta organização.</span><span class="sxs-lookup"><span data-stu-id="74e54-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="74e54-106">Permissions</span></span>
<span data-ttu-id="74e54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e54-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74e54-109">Permission type</span></span>      | <span data-ttu-id="74e54-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74e54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e54-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74e54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74e54-112">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="74e54-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74e54-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74e54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74e54-114">Not supported.</span></span>    |
|<span data-ttu-id="74e54-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74e54-115">Application</span></span> | <span data-ttu-id="74e54-116">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="74e54-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e54-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74e54-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74e54-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74e54-118">Optional query parameters</span></span>
<span data-ttu-id="74e54-119">Este método oferece suporte `$expand`aos `$filter`parâmetros `$select`de `$top` [consulta OData](/graph/query-parameters) ,, e OData, para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74e54-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74e54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74e54-120">Request headers</span></span>
| <span data-ttu-id="74e54-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74e54-121">Header</span></span>       | <span data-ttu-id="74e54-122">Valor</span><span class="sxs-lookup"><span data-stu-id="74e54-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="74e54-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="74e54-123">Authorization</span></span>  |<span data-ttu-id="74e54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74e54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74e54-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74e54-126">Request body</span></span>
<span data-ttu-id="74e54-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74e54-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74e54-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e54-128">Response</span></span>

<span data-ttu-id="74e54-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74e54-129">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74e54-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74e54-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74e54-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74e54-131">Request</span></span>
<span data-ttu-id="74e54-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74e54-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="74e54-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="74e54-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="74e54-134">C#</span><span class="sxs-lookup"><span data-stu-id="74e54-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74e54-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74e54-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74e54-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74e54-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74e54-137">Java</span><span class="sxs-lookup"><span data-stu-id="74e54-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74e54-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e54-138">Response</span></span>
<span data-ttu-id="74e54-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74e54-139">The following is an example of the response.</span></span>
><span data-ttu-id="74e54-140">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74e54-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "addresses":[
          {
            "city": "string",
            "countryOrRegion": "string",
            "officeLocation": "string",
            "postalCode": "string",
            "state": "string",
            "street": "string"
          }
      ],
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "phones":[
          {
            "type": "string",
            "number": "string"
          }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
