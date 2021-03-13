---
title: Listar directReports
description: Obter os relatórios diretos do contato.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1d294f80b8bf1e55e1575490fb1b888e78afbd47
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761629"
---
# <a name="list-directreports"></a><span data-ttu-id="3f1ea-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="3f1ea-103">List directReports</span></span>

<span data-ttu-id="3f1ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f1ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f1ea-105">Obter os relatórios diretos para esse [contato organizacional](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="3f1ea-105">Get the direct reports for this [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f1ea-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3f1ea-106">Permissions</span></span>
<span data-ttu-id="3f1ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f1ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f1ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f1ea-109">Permission type</span></span>      | <span data-ttu-id="3f1ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f1ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f1ea-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f1ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f1ea-112">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f1ea-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="3f1ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f1ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f1ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-114">Not supported.</span></span>    |
|<span data-ttu-id="3f1ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f1ea-115">Application</span></span> | <span data-ttu-id="3f1ea-116">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f1ea-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3f1ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f1ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f1ea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f1ea-118">Optional query parameters</span></span>
<span data-ttu-id="3f1ea-119">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-119">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f1ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f1ea-120">Request headers</span></span>
| <span data-ttu-id="3f1ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f1ea-121">Header</span></span>       | <span data-ttu-id="3f1ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3f1ea-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3f1ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f1ea-123">Authorization</span></span>  | <span data-ttu-id="3f1ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f1ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f1ea-126">Request body</span></span>
<span data-ttu-id="3f1ea-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f1ea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f1ea-128">Response</span></span>

<span data-ttu-id="3f1ea-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f1ea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f1ea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f1ea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f1ea-131">Request</span></span>
<span data-ttu-id="3f1ea-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f1ea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f1ea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/directReports
```
# <a name="c"></a>[<span data-ttu-id="3f1ea-134">C#</span><span class="sxs-lookup"><span data-stu-id="3f1ea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f1ea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f1ea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f1ea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f1ea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f1ea-137">Java</span><span class="sxs-lookup"><span data-stu-id="3f1ea-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contacts-get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f1ea-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f1ea-138">Response</span></span>
<span data-ttu-id="3f1ea-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-139">The following is an example of the response.</span></span>
><span data-ttu-id="3f1ea-140">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3f1ea-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

