---
title: Listar respostas
description: Recupere uma lista de objetos chatmessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 025607cb1b2b9bb33820b8877cbde1d6a1fac844
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947789"
---
# <a name="list-replies"></a><span data-ttu-id="4669f-103">Listar respostas</span><span class="sxs-lookup"><span data-stu-id="4669f-103">List replies</span></span>

<span data-ttu-id="4669f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4669f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4669f-105">Recupere uma lista de objetos chatmessage.</span><span class="sxs-lookup"><span data-stu-id="4669f-105">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4669f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4669f-106">Permissions</span></span>

<span data-ttu-id="4669f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4669f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4669f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4669f-109">Permission type</span></span>                        | <span data-ttu-id="4669f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4669f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4669f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4669f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4669f-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4669f-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="4669f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4669f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4669f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4669f-114">Not supported.</span></span> |
| <span data-ttu-id="4669f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4669f-115">Application</span></span>                            | <span data-ttu-id="4669f-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4669f-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="4669f-117">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4669f-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="4669f-118">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="4669f-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="4669f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4669f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4669f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4669f-120">Optional query parameters</span></span>

<span data-ttu-id="4669f-121">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4669f-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4669f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4669f-122">Request headers</span></span>

| <span data-ttu-id="4669f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4669f-123">Name</span></span>      |<span data-ttu-id="4669f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4669f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4669f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4669f-125">Authorization</span></span> | <span data-ttu-id="4669f-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4669f-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4669f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4669f-127">Request body</span></span>

<span data-ttu-id="4669f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4669f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4669f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4669f-129">Response</span></span>

<span data-ttu-id="4669f-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4669f-130">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4669f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4669f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4669f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4669f-132">Request</span></span>

<span data-ttu-id="4669f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4669f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4669f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4669f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="4669f-135">C#</span><span class="sxs-lookup"><span data-stu-id="4669f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4669f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4669f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4669f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4669f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4669f-138">Java</span><span class="sxs-lookup"><span data-stu-id="4669f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4669f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4669f-139">Response</span></span>

<span data-ttu-id="4669f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4669f-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4669f-141">O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="4669f-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4669f-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4669f-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "replyToId": "replyToId-value",
      "from": {
        "application": {
          "id": "id-value",
          "displayName": "displayName-value"
        },
        "device": {
          "id": "id-value",
          "displayName": "displayName-value"
        },
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "etag": "etag-value",
      "messageType": "messageType-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


