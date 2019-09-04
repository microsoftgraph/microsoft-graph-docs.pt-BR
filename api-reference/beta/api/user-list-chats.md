---
title: Listar chats
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 076e7ad9a8b97b3ddd6238f412f59ac651980722
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724222"
---
# <a name="list-chats"></a><span data-ttu-id="9be0e-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="9be0e-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be0e-104">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="9be0e-104">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9be0e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9be0e-105">Permissions</span></span>

<span data-ttu-id="9be0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9be0e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9be0e-108">Permission type</span></span>                        | <span data-ttu-id="9be0e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9be0e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9be0e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9be0e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be0e-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9be0e-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="9be0e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9be0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be0e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be0e-113">Not supported.</span></span> |
| <span data-ttu-id="9be0e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9be0e-114">Application</span></span>                            | <span data-ttu-id="9be0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be0e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9be0e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9be0e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9be0e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9be0e-117">Optional query parameters</span></span>

<span data-ttu-id="9be0e-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9be0e-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9be0e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9be0e-119">Request headers</span></span>

| <span data-ttu-id="9be0e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9be0e-120">Name</span></span>      |<span data-ttu-id="9be0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be0e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9be0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9be0e-122">Authorization</span></span> | <span data-ttu-id="9be0e-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9be0e-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9be0e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9be0e-124">Request body</span></span>

<span data-ttu-id="9be0e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9be0e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9be0e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be0e-126">Response</span></span>

<span data-ttu-id="9be0e-127">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9be0e-127">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9be0e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9be0e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9be0e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9be0e-129">Request</span></span>

<span data-ttu-id="9be0e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9be0e-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9be0e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be0e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9be0e-132">C#</span><span class="sxs-lookup"><span data-stu-id="9be0e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9be0e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9be0e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9be0e-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9be0e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9be0e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be0e-135">Response</span></span>

<span data-ttu-id="9be0e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9be0e-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9be0e-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9be0e-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9be0e-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9be0e-138">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
