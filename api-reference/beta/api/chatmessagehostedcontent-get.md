---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e os relacionamentos do objeto chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1cf0aa6bcca49921d90117be71f4cdc5af28372a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261359"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="52e39-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="52e39-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52e39-104">Recupere as propriedades e os relacionamentos do objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="52e39-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52e39-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52e39-105">Permissions</span></span>

<span data-ttu-id="52e39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52e39-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52e39-108">Permission type</span></span>                        | <span data-ttu-id="52e39-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52e39-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52e39-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52e39-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="52e39-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52e39-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="52e39-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52e39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52e39-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52e39-113">Not supported.</span></span> |
| <span data-ttu-id="52e39-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52e39-114">Application</span></span>                            | <span data-ttu-id="52e39-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52e39-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52e39-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52e39-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52e39-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52e39-117">Optional query parameters</span></span>

<span data-ttu-id="52e39-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52e39-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52e39-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52e39-119">Request headers</span></span>

| <span data-ttu-id="52e39-120">Nome</span><span class="sxs-lookup"><span data-stu-id="52e39-120">Name</span></span>      |<span data-ttu-id="52e39-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="52e39-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52e39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e39-122">Authorization</span></span> | <span data-ttu-id="52e39-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="52e39-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="52e39-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52e39-124">Request body</span></span>

<span data-ttu-id="52e39-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52e39-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52e39-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="52e39-126">Response</span></span>

<span data-ttu-id="52e39-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52e39-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52e39-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52e39-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52e39-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52e39-129">Request</span></span>

<span data-ttu-id="52e39-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52e39-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```

### <a name="response"></a><span data-ttu-id="52e39-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="52e39-131">Response</span></span>

<span data-ttu-id="52e39-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52e39-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="52e39-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52e39-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52e39-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52e39-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52e39-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="52e39-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="52e39-136">C#</span><span class="sxs-lookup"><span data-stu-id="52e39-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52e39-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="52e39-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52e39-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52e39-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chatmessagehostedcontent-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chatmessagehostedcontent-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
