---
title: Listar chats
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3e8ea297fe707c1076543f925610e30686627a7f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270165"
---
# <a name="list-chats"></a><span data-ttu-id="dfef6-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="dfef6-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfef6-104">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="dfef6-104">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfef6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfef6-105">Permissions</span></span>

<span data-ttu-id="dfef6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfef6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfef6-108">Permission type</span></span>                        | <span data-ttu-id="dfef6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfef6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dfef6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfef6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfef6-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfef6-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="dfef6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfef6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfef6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfef6-113">Not supported.</span></span> |
| <span data-ttu-id="dfef6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfef6-114">Application</span></span>                            | <span data-ttu-id="dfef6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfef6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfef6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfef6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfef6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfef6-117">Optional query parameters</span></span>

<span data-ttu-id="dfef6-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfef6-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfef6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfef6-119">Request headers</span></span>

| <span data-ttu-id="dfef6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dfef6-120">Name</span></span>      |<span data-ttu-id="dfef6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfef6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfef6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfef6-122">Authorization</span></span> | <span data-ttu-id="dfef6-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="dfef6-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfef6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfef6-124">Request body</span></span>

<span data-ttu-id="dfef6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfef6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfef6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfef6-126">Response</span></span>

<span data-ttu-id="dfef6-127">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfef6-127">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfef6-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfef6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfef6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfef6-129">Request</span></span>

<span data-ttu-id="dfef6-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfef6-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

### <a name="response"></a><span data-ttu-id="dfef6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfef6-131">Response</span></span>

<span data-ttu-id="dfef6-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfef6-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="dfef6-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dfef6-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dfef6-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfef6-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "topic": "topic-value",
      "createdDateTime": "datetime-value",
      "lastUpdatedDateTime": "datetime-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfef6-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dfef6-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="dfef6-136">C#</span><span class="sxs-lookup"><span data-stu-id="dfef6-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chats-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfef6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfef6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chats-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfef6-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dfef6-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chats-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-list-chats.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
