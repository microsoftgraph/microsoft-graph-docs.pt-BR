---
title: Listar directReports
description: Obter os relatórios diretos de um usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff22d99f4982669ba8276a4699c22fdb57c407a7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721982"
---
# <a name="list-directreports"></a><span data-ttu-id="b3776-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="b3776-103">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3776-104">Obter os relatórios diretos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b3776-104">Get a user's direct reports.</span></span> <span data-ttu-id="b3776-105">Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="b3776-105">Returns the users and contacts for whom this user is assigned as manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3776-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3776-106">Permissions</span></span>
<span data-ttu-id="b3776-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3776-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3776-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3776-109">Permission type</span></span>      | <span data-ttu-id="b3776-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3776-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3776-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3776-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3776-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3776-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b3776-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3776-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3776-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b3776-114">Not supported</span></span> |
|<span data-ttu-id="b3776-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3776-115">Application</span></span> | <span data-ttu-id="b3776-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3776-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3776-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3776-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3776-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3776-118">Optional query parameters</span></span>
<span data-ttu-id="b3776-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3776-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b3776-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3776-120">Request headers</span></span>
| <span data-ttu-id="b3776-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3776-121">Header</span></span>       | <span data-ttu-id="b3776-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3776-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b3776-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3776-123">Authorization</span></span>  | <span data-ttu-id="b3776-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3776-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b3776-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3776-126">Content-Type</span></span>   | <span data-ttu-id="b3776-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b3776-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3776-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3776-128">Request body</span></span>
<span data-ttu-id="b3776-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3776-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3776-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3776-130">Response</span></span>

<span data-ttu-id="b3776-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3776-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3776-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3776-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3776-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3776-133">Request</span></span>
<span data-ttu-id="b3776-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3776-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3776-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3776-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3776-136">C#</span><span class="sxs-lookup"><span data-stu-id="b3776-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3776-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3776-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3776-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b3776-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3776-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3776-139">Response</span></span>
<span data-ttu-id="b3776-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3776-140">Here is an example of the response.</span></span> 

><span data-ttu-id="b3776-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3776-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
