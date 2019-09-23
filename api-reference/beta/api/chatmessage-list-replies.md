---
title: Listar respostas
description: Recupere uma lista de objetos chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b5a781b6f6c4e3aeea7941ed956b99f182dc3110
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113860"
---
# <a name="list-replies"></a><span data-ttu-id="720ed-103">Listar respostas</span><span class="sxs-lookup"><span data-stu-id="720ed-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="720ed-104">Recupere uma lista de objetos chat.</span><span class="sxs-lookup"><span data-stu-id="720ed-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="720ed-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="720ed-105">Permissions</span></span>

<span data-ttu-id="720ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="720ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="720ed-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="720ed-108">Permission type</span></span>                        | <span data-ttu-id="720ed-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="720ed-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="720ed-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="720ed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="720ed-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="720ed-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="720ed-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="720ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="720ed-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="720ed-113">Not supported.</span></span> |
| <span data-ttu-id="720ed-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="720ed-114">Application</span></span>                            | <span data-ttu-id="720ed-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="720ed-115">Chat.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="720ed-116">Antes de chamar esta API com permissões de aplicativo, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="720ed-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="720ed-117">Para obter detalhes, consulte [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="720ed-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="720ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="720ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="720ed-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="720ed-119">Optional query parameters</span></span>

<span data-ttu-id="720ed-120">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="720ed-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="720ed-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="720ed-121">Request headers</span></span>

| <span data-ttu-id="720ed-122">Nome</span><span class="sxs-lookup"><span data-stu-id="720ed-122">Name</span></span>      |<span data-ttu-id="720ed-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="720ed-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="720ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="720ed-124">Authorization</span></span> | <span data-ttu-id="720ed-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="720ed-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="720ed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="720ed-126">Request body</span></span>

<span data-ttu-id="720ed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="720ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="720ed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="720ed-128">Response</span></span>

<span data-ttu-id="720ed-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [chatMessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="720ed-129">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="720ed-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="720ed-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="720ed-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="720ed-131">Request</span></span>

<span data-ttu-id="720ed-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="720ed-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="720ed-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="720ed-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="720ed-134">C#</span><span class="sxs-lookup"><span data-stu-id="720ed-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="720ed-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="720ed-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="720ed-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="720ed-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="720ed-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="720ed-137">Response</span></span>

<span data-ttu-id="720ed-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="720ed-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="720ed-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="720ed-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="720ed-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="720ed-140">All the properties will be returned from an actual call.</span></span>

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
