---
title: Obter transitiveReports para um usuário
description: Obter a contagem de relatórios transitivos para um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b6daf440cc9c1b3026fe7c5fa46838d0d59717d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210819"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="9189a-103">Obter transitiveReports para um usuário</span><span class="sxs-lookup"><span data-stu-id="9189a-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="9189a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9189a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9189a-105">Recupere uma contagem de relatórios transitivos para um usuário.</span><span class="sxs-lookup"><span data-stu-id="9189a-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9189a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9189a-106">Permissions</span></span>

<span data-ttu-id="9189a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9189a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="9189a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9189a-109">Permission type</span></span> | <span data-ttu-id="9189a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9189a-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="9189a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9189a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9189a-112">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9189a-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="9189a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9189a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9189a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9189a-114">Not supported.</span></span> |
| <span data-ttu-id="9189a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9189a-115">Application</span></span> | <span data-ttu-id="9189a-116">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9189a-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9189a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9189a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9189a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9189a-118">Optional query parameters</span></span>

<span data-ttu-id="9189a-119">Este método dá suporte `$filter` ao parâmetro de consulta apenas para a propriedade **accountEnabled.**</span><span class="sxs-lookup"><span data-stu-id="9189a-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="9189a-120">Para obter mais informações sobre como usar parâmetros de consulta, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9189a-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9189a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9189a-121">Request headers</span></span>

| <span data-ttu-id="9189a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9189a-122">Header</span></span>       | <span data-ttu-id="9189a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9189a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9189a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9189a-124">Authorization</span></span>  | <span data-ttu-id="9189a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9189a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9189a-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9189a-127">ConsistencyLevel</span></span> | <span data-ttu-id="9189a-128">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="9189a-128">eventual.</span></span> <span data-ttu-id="9189a-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9189a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9189a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9189a-130">Request body</span></span>

<span data-ttu-id="9189a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9189a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9189a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9189a-132">Response</span></span>

<span data-ttu-id="9189a-133">Se tiver êxito, este método retornará um código de resposta e uma contagem de relatórios `200 OK` transitivos para o usuário no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9189a-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9189a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9189a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9189a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9189a-135">Request</span></span>

<span data-ttu-id="9189a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9189a-136">The following is an example of the request.</span></span> <span data-ttu-id="9189a-137">O `$count` segmento de consulta é necessário.</span><span class="sxs-lookup"><span data-stu-id="9189a-137">The `$count` query segment is required.</span></span>


# <a name="http"></a>[<span data-ttu-id="9189a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9189a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="9189a-139">C#</span><span class="sxs-lookup"><span data-stu-id="9189a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9189a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9189a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9189a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9189a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9189a-142">Java</span><span class="sxs-lookup"><span data-stu-id="9189a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9189a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9189a-143">Response</span></span>

<span data-ttu-id="9189a-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9189a-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="9189a-145">5 </span><span class="sxs-lookup"><span data-stu-id="9189a-145">5</span></span>

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
