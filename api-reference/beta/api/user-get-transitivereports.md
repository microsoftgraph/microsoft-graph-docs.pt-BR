---
title: Obter transitiveReports para um usuário
description: Obter a contagem de relatórios transitivos para um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1ec6b231592ffec0d8847282b50e4ad227ecf06
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151770"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="f27ea-103">Obter transitiveReports para um usuário</span><span class="sxs-lookup"><span data-stu-id="f27ea-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="f27ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f27ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f27ea-105">Recupere uma contagem de relatórios transitivos para um usuário.</span><span class="sxs-lookup"><span data-stu-id="f27ea-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f27ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f27ea-106">Permissions</span></span>

<span data-ttu-id="f27ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f27ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="f27ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f27ea-109">Permission type</span></span> | <span data-ttu-id="f27ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f27ea-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="f27ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f27ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f27ea-112">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f27ea-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="f27ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f27ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f27ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f27ea-114">Not supported.</span></span> |
| <span data-ttu-id="f27ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f27ea-115">Application</span></span> | <span data-ttu-id="f27ea-116">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f27ea-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f27ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f27ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f27ea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f27ea-118">Optional query parameters</span></span>

<span data-ttu-id="f27ea-119">Este método dá suporte `$filter` ao parâmetro de consulta apenas para a propriedade **accountEnabled.**</span><span class="sxs-lookup"><span data-stu-id="f27ea-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="f27ea-120">Para obter mais informações sobre como usar parâmetros de consulta, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f27ea-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f27ea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f27ea-121">Request headers</span></span>

| <span data-ttu-id="f27ea-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f27ea-122">Header</span></span>       | <span data-ttu-id="f27ea-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f27ea-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f27ea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f27ea-124">Authorization</span></span>  | <span data-ttu-id="f27ea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f27ea-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f27ea-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f27ea-127">ConsistencyLevel</span></span> | <span data-ttu-id="f27ea-128">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="f27ea-128">eventual.</span></span> <span data-ttu-id="f27ea-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f27ea-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f27ea-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f27ea-130">Request body</span></span>

<span data-ttu-id="f27ea-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f27ea-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f27ea-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f27ea-132">Response</span></span>

<span data-ttu-id="f27ea-133">Se tiver êxito, este método retornará um código de resposta e uma contagem de relatórios `200 OK` transitivos para o usuário no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f27ea-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f27ea-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f27ea-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f27ea-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f27ea-135">Request</span></span>

<span data-ttu-id="f27ea-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f27ea-136">The following is an example of the request.</span></span> <span data-ttu-id="f27ea-137">O `$count` segmento de consulta é necessário.</span><span class="sxs-lookup"><span data-stu-id="f27ea-137">The `$count` query segment is required.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```http
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```

### <a name="response"></a><span data-ttu-id="f27ea-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f27ea-138">Response</span></span>

<span data-ttu-id="f27ea-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f27ea-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="f27ea-140">5 </span><span class="sxs-lookup"><span data-stu-id="f27ea-140">5</span></span>

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
