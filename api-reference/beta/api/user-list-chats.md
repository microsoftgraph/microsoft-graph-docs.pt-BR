---
title: Listar chats
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1dd4dee5f807f31cd9d8110be37abb14b792fdef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451886"
---
# <a name="list-chats"></a><span data-ttu-id="a574f-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="a574f-103">List chats</span></span>

<span data-ttu-id="a574f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a574f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a574f-105">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="a574f-105">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a574f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a574f-106">Permissions</span></span>

<span data-ttu-id="a574f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a574f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a574f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a574f-109">Permission type</span></span>                        | <span data-ttu-id="a574f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a574f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a574f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a574f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a574f-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a574f-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="a574f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a574f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a574f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a574f-114">Not supported.</span></span> |
| <span data-ttu-id="a574f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a574f-115">Application</span></span>                            | <span data-ttu-id="a574f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a574f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a574f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a574f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a574f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a574f-118">Optional query parameters</span></span>

<span data-ttu-id="a574f-119">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a574f-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a574f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a574f-120">Request headers</span></span>

| <span data-ttu-id="a574f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a574f-121">Name</span></span>      |<span data-ttu-id="a574f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a574f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a574f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a574f-123">Authorization</span></span> | <span data-ttu-id="a574f-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a574f-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a574f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a574f-125">Request body</span></span>

<span data-ttu-id="a574f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a574f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a574f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a574f-127">Response</span></span>

<span data-ttu-id="a574f-128">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a574f-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a574f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a574f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a574f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a574f-130">Request</span></span>

<span data-ttu-id="a574f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a574f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a574f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a574f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="a574f-133">C#</span><span class="sxs-lookup"><span data-stu-id="a574f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a574f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a574f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a574f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a574f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a574f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a574f-136">Response</span></span>

<span data-ttu-id="a574f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a574f-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a574f-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a574f-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a574f-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a574f-139">All the properties will be returned from an actual call.</span></span>

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
