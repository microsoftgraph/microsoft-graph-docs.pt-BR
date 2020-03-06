---
title: Obter orgContact
description: Recupere as propriedades de um objeto orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 041898cb17c827835db016c1955135d312432a9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511198"
---
# <a name="get-orgcontact"></a><span data-ttu-id="ab030-103">Obter orgContact</span><span class="sxs-lookup"><span data-stu-id="ab030-103">Get orgContact</span></span>

<span data-ttu-id="ab030-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab030-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab030-105">Obtenha as propriedades e os relacionamentos de um [contato organizacional](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="ab030-105">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab030-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab030-106">Permissions</span></span>
<span data-ttu-id="ab030-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab030-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab030-109">Permission type</span></span>      | <span data-ttu-id="ab030-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab030-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab030-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab030-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab030-112">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ab030-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab030-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab030-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab030-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab030-114">Not supported.</span></span>    |
|<span data-ttu-id="ab030-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab030-115">Application</span></span> | <span data-ttu-id="ab030-116">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab030-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab030-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab030-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab030-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab030-118">Optional query parameters</span></span>
<span data-ttu-id="ab030-119">Este método oferece suporte `$select` aos `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab030-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab030-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab030-120">Request headers</span></span>
| <span data-ttu-id="ab030-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab030-121">Header</span></span>       | <span data-ttu-id="ab030-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ab030-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ab030-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab030-123">Authorization</span></span>  | <span data-ttu-id="ab030-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab030-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab030-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab030-126">Request body</span></span>
<span data-ttu-id="ab030-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab030-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab030-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab030-128">Response</span></span>

<span data-ttu-id="ab030-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab030-129">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab030-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab030-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab030-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab030-131">Request</span></span>
<span data-ttu-id="ab030-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab030-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ab030-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab030-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="ab030-134">C#</span><span class="sxs-lookup"><span data-stu-id="ab030-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab030-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab030-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab030-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab030-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab030-137">Java</span><span class="sxs-lookup"><span data-stu-id="ab030-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab030-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab030-138">Response</span></span>
<span data-ttu-id="ab030-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab030-139">The following is an example of the response.</span></span>
><span data-ttu-id="ab030-140">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab030-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
