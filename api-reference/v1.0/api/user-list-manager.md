---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81a7936f713e769b8025dfde0b2f3d42f7234d44
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727471"
---
# <a name="list-manager"></a><span data-ttu-id="0fe31-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="0fe31-104">List manager</span></span>

<span data-ttu-id="0fe31-105">Obtenha o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="0fe31-105">Get user's manager.</span></span> <span data-ttu-id="0fe31-106">Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="0fe31-106">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fe31-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fe31-107">Permissions</span></span>
<span data-ttu-id="0fe31-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fe31-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fe31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fe31-110">Permission type</span></span>      | <span data-ttu-id="0fe31-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fe31-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fe31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fe31-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0fe31-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0fe31-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0fe31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fe31-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fe31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fe31-115">Not supported.</span></span>    |
|<span data-ttu-id="0fe31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fe31-116">Application</span></span> | <span data-ttu-id="0fe31-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fe31-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe31-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0fe31-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fe31-119">Optional query parameters</span></span>
<span data-ttu-id="0fe31-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe31-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0fe31-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe31-121">Request headers</span></span>
| <span data-ttu-id="0fe31-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fe31-122">Header</span></span>       | <span data-ttu-id="0fe31-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0fe31-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0fe31-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fe31-124">Authorization</span></span>  | <span data-ttu-id="0fe31-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fe31-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0fe31-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fe31-127">Content-Type</span></span>   | <span data-ttu-id="0fe31-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0fe31-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fe31-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe31-129">Request body</span></span>
<span data-ttu-id="0fe31-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fe31-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe31-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe31-131">Response</span></span>

<span data-ttu-id="0fe31-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe31-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fe31-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fe31-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fe31-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fe31-134">Request</span></span>
<span data-ttu-id="0fe31-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fe31-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fe31-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe31-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fe31-137">C#</span><span class="sxs-lookup"><span data-stu-id="0fe31-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fe31-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fe31-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fe31-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fe31-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0fe31-140">Java</span><span class="sxs-lookup"><span data-stu-id="0fe31-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0fe31-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fe31-141">Response</span></span>
<span data-ttu-id="0fe31-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fe31-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
