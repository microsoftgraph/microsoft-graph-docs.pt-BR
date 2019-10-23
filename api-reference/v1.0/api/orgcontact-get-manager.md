---
title: Obter gerente
description: Obtenha o gerente do contato organizacional.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c29f3912280faef09753d89be148c9f93e350053
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633991"
---
# <a name="get-manager"></a><span data-ttu-id="5f1f6-103">Obter gerente</span><span class="sxs-lookup"><span data-stu-id="5f1f6-103">Get manager</span></span>

<span data-ttu-id="5f1f6-104">Obtenha o gerente do contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-104">Get this organizational contact's manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f1f6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f1f6-105">Permissions</span></span>
<span data-ttu-id="5f1f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f1f6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f1f6-108">Permission type</span></span>      | <span data-ttu-id="5f1f6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f1f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f1f6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f1f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f1f6-111">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="5f1f6-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>   |
|<span data-ttu-id="5f1f6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f1f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f1f6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-113">Not supported.</span></span>    |
|<span data-ttu-id="5f1f6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f1f6-114">Application</span></span> | <span data-ttu-id="5f1f6-115">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="5f1f6-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f1f6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1f6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f1f6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f1f6-117">Optional query parameters</span></span>
<span data-ttu-id="5f1f6-118">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-118">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f1f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1f6-119">Request headers</span></span>
| <span data-ttu-id="5f1f6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f1f6-120">Header</span></span>       | <span data-ttu-id="5f1f6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5f1f6-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5f1f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f1f6-122">Authorization</span></span>  | <span data-ttu-id="5f1f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f1f6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1f6-125">Request body</span></span>
<span data-ttu-id="5f1f6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f1f6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1f6-127">Response</span></span>

<span data-ttu-id="5f1f6-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f1f6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f1f6-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f1f6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1f6-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5f1f6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1f6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f1f6-132">C#</span><span class="sxs-lookup"><span data-stu-id="5f1f6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f1f6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f1f6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f1f6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f1f6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5f1f6-135">Java</span><span class="sxs-lookup"><span data-stu-id="5f1f6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5f1f6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1f6-136">Response</span></span>
<span data-ttu-id="5f1f6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-137">The following is an example of the response.</span></span>
><span data-ttu-id="5f1f6-138">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f1f6-138">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
