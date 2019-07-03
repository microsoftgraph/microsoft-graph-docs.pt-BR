---
title: Listar membros
description: Recupere uma lista de objetos conversationMember.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0a3c1dc177a497240faaf8bd3ee20fb2e2c2b6ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437843"
---
# <a name="list-members"></a><span data-ttu-id="9809d-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="9809d-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9809d-104">Recupere uma lista de objetos [conversationMember](../resources/conversationmember.md) .</span><span class="sxs-lookup"><span data-stu-id="9809d-104">Retrieve a list of [conversationMember](../resources/conversationmember.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9809d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9809d-105">Permissions</span></span>

<span data-ttu-id="9809d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9809d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9809d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9809d-108">Permission type</span></span>                        | <span data-ttu-id="9809d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9809d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9809d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9809d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9809d-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9809d-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="9809d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9809d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9809d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9809d-113">Not supported.</span></span> |
| <span data-ttu-id="9809d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9809d-114">Application</span></span>                            | <span data-ttu-id="9809d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9809d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9809d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9809d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9809d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9809d-117">Optional query parameters</span></span>

<span data-ttu-id="9809d-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9809d-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9809d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9809d-119">Request headers</span></span>

| <span data-ttu-id="9809d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9809d-120">Name</span></span>      |<span data-ttu-id="9809d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9809d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9809d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9809d-122">Authorization</span></span> | <span data-ttu-id="9809d-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9809d-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9809d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9809d-124">Request body</span></span>

<span data-ttu-id="9809d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9809d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9809d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9809d-126">Response</span></span>

<span data-ttu-id="9809d-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9809d-127">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9809d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9809d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9809d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9809d-129">Request</span></span>

<span data-ttu-id="9809d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9809d-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9809d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9809d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9809d-132">C#</span><span class="sxs-lookup"><span data-stu-id="9809d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9809d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="9809d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9809d-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9809d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9809d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9809d-135">Response</span></span>

<span data-ttu-id="9809d-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9809d-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9809d-137">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9809d-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9809d-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9809d-138">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
