---
title: Listar ownedObjects
description: Obtenha a lista de objetos de diretório de propriedade do usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 7623fcc571d4b9f54d59c28b79260f604af3f297
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52033647"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="5c144-103">Listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="5c144-103">List ownedObjects</span></span>

<span data-ttu-id="5c144-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c144-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c144-105">Obtenha a lista de objetos de diretório de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c144-105">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c144-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c144-106">Permissions</span></span>
<span data-ttu-id="5c144-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c144-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c144-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c144-109">Permission type</span></span>      | <span data-ttu-id="5c144-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c144-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c144-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c144-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c144-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c144-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c144-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c144-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c144-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c144-114">Not supported.</span></span>    |
|<span data-ttu-id="5c144-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c144-115">Application</span></span> | <span data-ttu-id="5c144-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c144-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5c144-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c144-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c144-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c144-118">Optional query parameters</span></span>
<span data-ttu-id="5c144-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c144-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5c144-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c144-120">Request headers</span></span>
| <span data-ttu-id="5c144-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c144-121">Header</span></span>       | <span data-ttu-id="5c144-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5c144-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c144-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c144-123">Authorization</span></span>  | <span data-ttu-id="5c144-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c144-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5c144-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c144-126">Accept</span></span>  | <span data-ttu-id="5c144-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c144-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c144-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c144-128">Request body</span></span>
<span data-ttu-id="5c144-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c144-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c144-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c144-130">Response</span></span>

<span data-ttu-id="5c144-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c144-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c144-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c144-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c144-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c144-133">Request</span></span>
<span data-ttu-id="5c144-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c144-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c144-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c144-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="5c144-136">C#</span><span class="sxs-lookup"><span data-stu-id="5c144-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c144-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c144-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c144-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c144-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c144-139">Java</span><span class="sxs-lookup"><span data-stu-id="5c144-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c144-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c144-140">Response</span></span>
<span data-ttu-id="5c144-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c144-141">Here is an example of the response.</span></span> <span data-ttu-id="5c144-142">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c144-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
