---
title: Obter transitiveReports para um usuário
description: Obter a contagem de relatórios transitivos para um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5d04b1240c54b186a2e5f5cfb77f651e032f1eda
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316598"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="41d9b-103">Obter transitiveReports para um usuário</span><span class="sxs-lookup"><span data-stu-id="41d9b-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="41d9b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41d9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41d9b-105">Recupere uma contagem de relatórios transitivos para um usuário.</span><span class="sxs-lookup"><span data-stu-id="41d9b-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="41d9b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41d9b-106">Permissions</span></span>

<span data-ttu-id="41d9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="41d9b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41d9b-109">Permission type</span></span> | <span data-ttu-id="41d9b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41d9b-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="41d9b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41d9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="41d9b-112">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d9b-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="41d9b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41d9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41d9b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41d9b-114">Not supported.</span></span> |
| <span data-ttu-id="41d9b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41d9b-115">Application</span></span> | <span data-ttu-id="41d9b-116">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d9b-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41d9b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41d9b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41d9b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41d9b-118">Optional query parameters</span></span>

<span data-ttu-id="41d9b-119">Este método dá suporte `$filter` ao parâmetro de consulta apenas para a propriedade **accountEnabled.**</span><span class="sxs-lookup"><span data-stu-id="41d9b-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="41d9b-120">Para obter mais informações sobre como usar parâmetros de consulta, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="41d9b-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41d9b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41d9b-121">Request headers</span></span>

| <span data-ttu-id="41d9b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41d9b-122">Header</span></span>       | <span data-ttu-id="41d9b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="41d9b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41d9b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="41d9b-124">Authorization</span></span>  | <span data-ttu-id="41d9b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d9b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="41d9b-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="41d9b-127">ConsistencyLevel</span></span> | <span data-ttu-id="41d9b-128">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="41d9b-128">eventual.</span></span> <span data-ttu-id="41d9b-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41d9b-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41d9b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41d9b-130">Request body</span></span>

<span data-ttu-id="41d9b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41d9b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d9b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d9b-132">Response</span></span>

<span data-ttu-id="41d9b-133">Se tiver êxito, este método retornará um código de resposta e uma contagem de relatórios `200 OK` transitivos para o usuário no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41d9b-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41d9b-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41d9b-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41d9b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41d9b-135">Request</span></span>

<span data-ttu-id="41d9b-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41d9b-136">The following is an example of the request.</span></span> <span data-ttu-id="41d9b-137">O `$count` segmento de consulta é necessário.</span><span class="sxs-lookup"><span data-stu-id="41d9b-137">The `$count` query segment is required.</span></span>


# <a name="http"></a>[<span data-ttu-id="41d9b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="41d9b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="41d9b-139">C#</span><span class="sxs-lookup"><span data-stu-id="41d9b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41d9b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41d9b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41d9b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41d9b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41d9b-142">Java</span><span class="sxs-lookup"><span data-stu-id="41d9b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41d9b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="41d9b-143">Response</span></span>

<span data-ttu-id="41d9b-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41d9b-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="41d9b-145">5 </span><span class="sxs-lookup"><span data-stu-id="41d9b-145">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports for a user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
