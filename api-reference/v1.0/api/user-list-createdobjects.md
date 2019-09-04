---
title: Listar createdObjects
description: Obtenha uma lista de objetos de diretório criados pelo usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9fb8ef9cdaaecdb713b6e546d2f543361e9e83ea
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727513"
---
# <a name="list-createdobjects"></a><span data-ttu-id="3275a-103">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="3275a-103">List createdObjects</span></span>

<span data-ttu-id="3275a-104">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3275a-104">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="3275a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3275a-105">Permissions</span></span>
<span data-ttu-id="3275a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3275a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3275a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3275a-108">Permission type</span></span>      | <span data-ttu-id="3275a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3275a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3275a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3275a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3275a-111">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3275a-111">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3275a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3275a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3275a-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3275a-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="3275a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3275a-114">Application</span></span> | <span data-ttu-id="3275a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3275a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3275a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3275a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3275a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3275a-117">Optional query parameters</span></span>
<span data-ttu-id="3275a-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3275a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3275a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3275a-119">Request headers</span></span>
| <span data-ttu-id="3275a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3275a-120">Header</span></span>       | <span data-ttu-id="3275a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3275a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3275a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3275a-122">Authorization</span></span>  | <span data-ttu-id="3275a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3275a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3275a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3275a-125">Content-Type</span></span>  | <span data-ttu-id="3275a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3275a-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3275a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3275a-127">Request body</span></span>
<span data-ttu-id="3275a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3275a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3275a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3275a-129">Response</span></span>

<span data-ttu-id="3275a-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3275a-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3275a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3275a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3275a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3275a-132">Request</span></span>
<span data-ttu-id="3275a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3275a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3275a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3275a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3275a-135">C#</span><span class="sxs-lookup"><span data-stu-id="3275a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3275a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3275a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3275a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3275a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3275a-138">Java</span><span class="sxs-lookup"><span data-stu-id="3275a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3275a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3275a-139">Response</span></span>
<span data-ttu-id="3275a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3275a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
