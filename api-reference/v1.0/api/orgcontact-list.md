---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais desta organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1bab6f4bc94bff94f347c54b429a009d0e5cdf27
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633856"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="f87ad-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="f87ad-103">List orgContacts</span></span>

<span data-ttu-id="f87ad-104">Obtenha a lista de [contatos organizacionais](../resources/orgcontact.md) para esta organização.</span><span class="sxs-lookup"><span data-stu-id="f87ad-104">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f87ad-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87ad-105">Permissions</span></span>
<span data-ttu-id="f87ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f87ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f87ad-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f87ad-108">Permission type</span></span>      | <span data-ttu-id="f87ad-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f87ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f87ad-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f87ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f87ad-111">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f87ad-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f87ad-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f87ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87ad-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87ad-113">Not supported.</span></span>    |
|<span data-ttu-id="f87ad-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f87ad-114">Application</span></span> | <span data-ttu-id="f87ad-115">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f87ad-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f87ad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f87ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f87ad-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f87ad-117">Optional query parameters</span></span>
<span data-ttu-id="f87ad-118">Este método oferece suporte `$expand`aos `$filter`parâmetros `$select`de `$top` [consulta OData](/graph/query-parameters) ,, e OData, para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f87ad-118">This method supports the `$expand`, `$filter`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f87ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f87ad-119">Request headers</span></span>
| <span data-ttu-id="f87ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f87ad-120">Header</span></span>       | <span data-ttu-id="f87ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f87ad-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f87ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f87ad-122">Authorization</span></span>  |<span data-ttu-id="f87ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f87ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f87ad-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f87ad-125">Request body</span></span>
<span data-ttu-id="f87ad-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f87ad-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f87ad-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87ad-127">Response</span></span>

<span data-ttu-id="f87ad-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f87ad-128">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f87ad-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f87ad-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f87ad-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f87ad-130">Request</span></span>
<span data-ttu-id="f87ad-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f87ad-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f87ad-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f87ad-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f87ad-133">C#</span><span class="sxs-lookup"><span data-stu-id="f87ad-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f87ad-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f87ad-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f87ad-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f87ad-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f87ad-136">Java</span><span class="sxs-lookup"><span data-stu-id="f87ad-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f87ad-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87ad-137">Response</span></span>
<span data-ttu-id="f87ad-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f87ad-138">The following is an example of the response.</span></span>
><span data-ttu-id="f87ad-139">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f87ad-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
