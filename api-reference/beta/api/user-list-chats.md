---
title: Listar chats
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1aabbc0facd809f8387ceb68c97fdf64c98845c1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951517"
---
# <a name="list-chats"></a><span data-ttu-id="cb211-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="cb211-103">List chats</span></span>

<span data-ttu-id="cb211-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb211-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb211-105">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="cb211-105">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb211-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb211-106">Permissions</span></span>

<span data-ttu-id="cb211-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb211-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb211-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb211-109">Permission type</span></span>                        | <span data-ttu-id="cb211-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb211-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb211-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb211-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb211-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb211-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="cb211-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb211-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb211-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb211-114">Not supported.</span></span> |
| <span data-ttu-id="cb211-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb211-115">Application</span></span>                            | <span data-ttu-id="cb211-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb211-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb211-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb211-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb211-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb211-118">Optional query parameters</span></span>

<span data-ttu-id="cb211-119">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb211-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb211-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb211-120">Request headers</span></span>

| <span data-ttu-id="cb211-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cb211-121">Name</span></span>      |<span data-ttu-id="cb211-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb211-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb211-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb211-123">Authorization</span></span> | <span data-ttu-id="cb211-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cb211-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb211-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb211-125">Request body</span></span>

<span data-ttu-id="cb211-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb211-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb211-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb211-127">Response</span></span>

<span data-ttu-id="cb211-128">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb211-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb211-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb211-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb211-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb211-130">Request</span></span>

<span data-ttu-id="cb211-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb211-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb211-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb211-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="cb211-133">C#</span><span class="sxs-lookup"><span data-stu-id="cb211-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb211-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb211-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb211-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb211-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb211-136">Java</span><span class="sxs-lookup"><span data-stu-id="cb211-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chats-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb211-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb211-137">Response</span></span>

<span data-ttu-id="cb211-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb211-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cb211-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cb211-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb211-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb211-140">All the properties will be returned from an actual call.</span></span>

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


