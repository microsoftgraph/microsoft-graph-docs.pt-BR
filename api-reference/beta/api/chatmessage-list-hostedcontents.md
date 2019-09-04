---
title: Listar hostedContents
description: Recupere uma lista de objetos chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3291426ec6cc0b5f98b3bc7f0a1c7465e1e1340c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719833"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="4506c-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="4506c-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4506c-104">Recupere uma lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="4506c-104">Retrieve a list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4506c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4506c-105">Permissions</span></span>

<span data-ttu-id="4506c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4506c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4506c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4506c-108">Permission type</span></span>                        | <span data-ttu-id="4506c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4506c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4506c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4506c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4506c-111">Chat. Read, chat. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="4506c-111">Chat.Read, Chat.ReadWrite.</span></span> |
| <span data-ttu-id="4506c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4506c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4506c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4506c-113">Not supported.</span></span> |
| <span data-ttu-id="4506c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4506c-114">Application</span></span>                            | <span data-ttu-id="4506c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4506c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4506c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4506c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4506c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4506c-117">Optional query parameters</span></span>

<span data-ttu-id="4506c-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4506c-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4506c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4506c-119">Request headers</span></span>

| <span data-ttu-id="4506c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4506c-120">Name</span></span>      |<span data-ttu-id="4506c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4506c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4506c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4506c-122">Authorization</span></span> | <span data-ttu-id="4506c-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4506c-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4506c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4506c-124">Request body</span></span>

<span data-ttu-id="4506c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4506c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4506c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4506c-126">Response</span></span>

<span data-ttu-id="4506c-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4506c-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4506c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4506c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4506c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4506c-129">Request</span></span>

<span data-ttu-id="4506c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4506c-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4506c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4506c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4506c-132">C#</span><span class="sxs-lookup"><span data-stu-id="4506c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4506c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4506c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4506c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4506c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4506c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4506c-135">Response</span></span>

<span data-ttu-id="4506c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4506c-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4506c-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4506c-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4506c-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4506c-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
