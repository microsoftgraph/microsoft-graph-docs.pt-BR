---
title: Listar directReports
description: Obter os subordinados diretos do contato.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 01a46af833b7dc5d827d73f2fd48353e0e2b3622
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633915"
---
# <a name="list-directreports"></a><span data-ttu-id="3f2e3-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="3f2e3-103">List directReports</span></span>

<span data-ttu-id="3f2e3-104">Obtenha os subordinados diretos para este [contato organizacional](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="3f2e3-104">Get the direct reports for this [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f2e3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f2e3-105">Permissions</span></span>
<span data-ttu-id="3f2e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f2e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f2e3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f2e3-108">Permission type</span></span>      | <span data-ttu-id="3f2e3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f2e3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f2e3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f2e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f2e3-111">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="3f2e3-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="3f2e3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f2e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f2e3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-113">Not supported.</span></span>    |
|<span data-ttu-id="3f2e3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f2e3-114">Application</span></span> | <span data-ttu-id="3f2e3-115">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="3f2e3-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f2e3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f2e3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f2e3-117">Optional query parameters</span></span>
<span data-ttu-id="3f2e3-118">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-118">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f2e3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f2e3-119">Request headers</span></span>
| <span data-ttu-id="3f2e3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f2e3-120">Header</span></span>       | <span data-ttu-id="3f2e3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3f2e3-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3f2e3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f2e3-122">Authorization</span></span>  | <span data-ttu-id="3f2e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f2e3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f2e3-125">Request body</span></span>
<span data-ttu-id="3f2e3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f2e3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f2e3-127">Response</span></span>

<span data-ttu-id="3f2e3-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f2e3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f2e3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f2e3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f2e3-130">Request</span></span>
<span data-ttu-id="3f2e3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3f2e3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2e3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f2e3-133">C#</span><span class="sxs-lookup"><span data-stu-id="3f2e3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f2e3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f2e3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f2e3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f2e3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3f2e3-136">Java</span><span class="sxs-lookup"><span data-stu-id="3f2e3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contacts-get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f2e3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f2e3-137">Response</span></span>
<span data-ttu-id="3f2e3-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-138">The following is an example of the response.</span></span>
><span data-ttu-id="3f2e3-139">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3f2e3-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
      "businessPhones": [
          "+1 205 555 0108"
      ],
      "displayName": "Diego Siciliani",
      "givenName": "Diego",
      "jobTitle": "CVP Finance",
      "mail": "DiegoS@contoso.com",
      "mobilePhone": null,
      "officeLocation": "14/1108",
      "preferredLanguage": "en-US",
      "surname": "Siciliani",
      "userPrincipalName": "DiegoS@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
