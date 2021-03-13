---
title: Obter orgContact
description: Recupere as propriedades de um objeto orgContact.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f3702f51779bfb42d794aa011bc671b5b7dd99d3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761647"
---
# <a name="get-orgcontact"></a><span data-ttu-id="ee7dd-103">Obter orgContact</span><span class="sxs-lookup"><span data-stu-id="ee7dd-103">Get orgContact</span></span>

<span data-ttu-id="ee7dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee7dd-105">Obter as propriedades e as relações de um [contato organizacional](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="ee7dd-105">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee7dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee7dd-106">Permissions</span></span>
<span data-ttu-id="ee7dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee7dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee7dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee7dd-109">Permission type</span></span>      | <span data-ttu-id="ee7dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee7dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee7dd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee7dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee7dd-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee7dd-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee7dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee7dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee7dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-114">Not supported.</span></span>    |
|<span data-ttu-id="ee7dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee7dd-115">Application</span></span> | <span data-ttu-id="ee7dd-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7dd-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee7dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee7dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee7dd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee7dd-118">Optional query parameters</span></span>
<span data-ttu-id="ee7dd-119">Este método oferece suporte aos parâmetros de consulta `$select` e `$expand`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee7dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7dd-120">Request headers</span></span>
| <span data-ttu-id="ee7dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee7dd-121">Header</span></span>       | <span data-ttu-id="ee7dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee7dd-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ee7dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee7dd-123">Authorization</span></span>  | <span data-ttu-id="ee7dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee7dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7dd-126">Request body</span></span>
<span data-ttu-id="ee7dd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee7dd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee7dd-128">Response</span></span>

<span data-ttu-id="ee7dd-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-129">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee7dd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee7dd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee7dd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7dd-131">Request</span></span>
<span data-ttu-id="ee7dd-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee7dd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee7dd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="ee7dd-134">C#</span><span class="sxs-lookup"><span data-stu-id="ee7dd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee7dd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee7dd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee7dd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee7dd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee7dd-137">Java</span><span class="sxs-lookup"><span data-stu-id="ee7dd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee7dd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee7dd-138">Response</span></span>
<span data-ttu-id="ee7dd-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-139">The following is an example of the response.</span></span>
><span data-ttu-id="ee7dd-140">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee7dd-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

