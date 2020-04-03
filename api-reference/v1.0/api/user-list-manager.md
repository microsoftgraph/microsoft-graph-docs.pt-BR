---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Priority
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e7c3987a2fa0b9de06da823c19831e51428f0ad3
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108806"
---
# <a name="list-manager"></a><span data-ttu-id="97f83-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="97f83-104">List manager</span></span>

<span data-ttu-id="97f83-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97f83-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97f83-106">Obtenha o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="97f83-106">Get user's manager.</span></span> <span data-ttu-id="97f83-107">Retorna o usuário ou o contato organizacional atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="97f83-107">Returns the user or organizational contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="97f83-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="97f83-108">Permissions</span></span>
<span data-ttu-id="97f83-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97f83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97f83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97f83-111">Permission type</span></span>      | <span data-ttu-id="97f83-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97f83-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97f83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97f83-113">Delegated (work or school account)</span></span> | <span data-ttu-id="97f83-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97f83-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97f83-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97f83-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97f83-116">Not supported.</span></span>    |
|<span data-ttu-id="97f83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97f83-117">Application</span></span> | <span data-ttu-id="97f83-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f83-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="97f83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97f83-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97f83-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97f83-120">Optional query parameters</span></span>
<span data-ttu-id="97f83-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97f83-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97f83-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97f83-122">Request headers</span></span>
| <span data-ttu-id="97f83-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97f83-123">Header</span></span>       | <span data-ttu-id="97f83-124">Valor</span><span class="sxs-lookup"><span data-stu-id="97f83-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="97f83-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="97f83-125">Authorization</span></span>  | <span data-ttu-id="97f83-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97f83-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97f83-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97f83-128">Request body</span></span>
<span data-ttu-id="97f83-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97f83-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97f83-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="97f83-130">Response</span></span>

<span data-ttu-id="97f83-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97f83-131">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97f83-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97f83-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97f83-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97f83-133">Request</span></span>
<span data-ttu-id="97f83-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97f83-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97f83-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="97f83-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="97f83-136">C#</span><span class="sxs-lookup"><span data-stu-id="97f83-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97f83-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97f83-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97f83-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97f83-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97f83-139">Java</span><span class="sxs-lookup"><span data-stu-id="97f83-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97f83-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="97f83-140">Response</span></span>
<span data-ttu-id="97f83-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97f83-141">The following is an example of the response.</span></span>
><span data-ttu-id="97f83-142">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="97f83-142">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
