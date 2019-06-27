---
title: Listar membros
description: Recupere uma lista de objetos conversationMember.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bf4d178301be74410a894f05732679e482c64583
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261485"
---
# <a name="list-members"></a><span data-ttu-id="6d6cf-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="6d6cf-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d6cf-104">Recupere uma lista de objetos [conversationMember](../resources/conversationmember.md) .</span><span class="sxs-lookup"><span data-stu-id="6d6cf-104">Retrieve a list of [conversationMember](../resources/conversationmember.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d6cf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d6cf-105">Permissions</span></span>

<span data-ttu-id="6d6cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d6cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d6cf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d6cf-108">Permission type</span></span>                        | <span data-ttu-id="6d6cf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d6cf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d6cf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d6cf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d6cf-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d6cf-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="6d6cf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d6cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d6cf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-113">Not supported.</span></span> |
| <span data-ttu-id="6d6cf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d6cf-114">Application</span></span>                            | <span data-ttu-id="6d6cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d6cf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d6cf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d6cf-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d6cf-117">Optional query parameters</span></span>

<span data-ttu-id="6d6cf-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d6cf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d6cf-119">Request headers</span></span>

| <span data-ttu-id="6d6cf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6d6cf-120">Name</span></span>      |<span data-ttu-id="6d6cf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d6cf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d6cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d6cf-122">Authorization</span></span> | <span data-ttu-id="6d6cf-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6d6cf-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d6cf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d6cf-124">Request body</span></span>

<span data-ttu-id="6d6cf-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d6cf-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d6cf-126">Response</span></span>

<span data-ttu-id="6d6cf-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-127">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d6cf-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6d6cf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d6cf-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d6cf-129">Request</span></span>

<span data-ttu-id="6d6cf-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/members
```

### <a name="response"></a><span data-ttu-id="6d6cf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d6cf-131">Response</span></span>

<span data-ttu-id="6d6cf-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6d6cf-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d6cf-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d6cf-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "roles": [
        "roles-value"
      ],
      "displayName": "displayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6d6cf-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6d6cf-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6d6cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="6d6cf-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d6cf-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d6cf-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6d6cf-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6d6cf-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chat-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
