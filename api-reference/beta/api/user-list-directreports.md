---
title: Listar directReports
description: Obtenha relatórios diretos do usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5879128bc0fb8792d287d38b1c0478de940d807f
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107686"
---
# <a name="list-directreports"></a><span data-ttu-id="cdf29-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="cdf29-103">List directReports</span></span>

<span data-ttu-id="cdf29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdf29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdf29-105">Obtenha relatórios diretos do usuário.</span><span class="sxs-lookup"><span data-stu-id="cdf29-105">Get a user's direct reports.</span></span> <span data-ttu-id="cdf29-106">Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="cdf29-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdf29-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdf29-107">Permissions</span></span>
<span data-ttu-id="cdf29-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdf29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdf29-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdf29-110">Permission type</span></span>      | <span data-ttu-id="cdf29-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdf29-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdf29-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdf29-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cdf29-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cdf29-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="cdf29-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdf29-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdf29-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdf29-115">Not supported</span></span> |
|<span data-ttu-id="cdf29-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdf29-116">Application</span></span> | <span data-ttu-id="cdf29-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdf29-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cdf29-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdf29-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdf29-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cdf29-119">Optional query parameters</span></span>
<span data-ttu-id="cdf29-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cdf29-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdf29-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdf29-121">Request headers</span></span>
| <span data-ttu-id="cdf29-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdf29-122">Header</span></span>       | <span data-ttu-id="cdf29-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cdf29-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="cdf29-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdf29-124">Authorization</span></span>  | <span data-ttu-id="cdf29-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdf29-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdf29-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdf29-127">Content-Type</span></span>   | <span data-ttu-id="cdf29-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cdf29-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdf29-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdf29-129">Request body</span></span>
<span data-ttu-id="cdf29-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdf29-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdf29-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdf29-131">Response</span></span>

<span data-ttu-id="cdf29-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdf29-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdf29-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdf29-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdf29-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdf29-134">Request</span></span>
<span data-ttu-id="cdf29-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdf29-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdf29-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdf29-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="cdf29-137">C#</span><span class="sxs-lookup"><span data-stu-id="cdf29-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdf29-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdf29-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdf29-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdf29-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cdf29-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdf29-140">Response</span></span>
<span data-ttu-id="cdf29-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdf29-141">Here is an example of the response.</span></span> 

><span data-ttu-id="cdf29-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdf29-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
