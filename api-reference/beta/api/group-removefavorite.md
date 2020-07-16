---
title: 'group: removeFavorite'
description: Remover o grupo da lista de grupos de favoritos do usuário atual. Suportado somente para grupos do Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fe33a3ada951a87ea82f6f4875ab11843e9971b8
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895801"
---
# <a name="group-removefavorite"></a><span data-ttu-id="48017-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="48017-104">group: removeFavorite</span></span>

<span data-ttu-id="48017-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48017-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48017-106">Remover o grupo da lista de grupos de favoritos do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="48017-106">Remove the group from the list of the current user's favorite groups.</span></span> <span data-ttu-id="48017-107">Suportado somente para grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="48017-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="48017-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="48017-108">Permissions</span></span>
<span data-ttu-id="48017-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48017-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48017-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48017-111">Permission type</span></span>      | <span data-ttu-id="48017-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48017-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48017-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48017-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48017-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48017-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48017-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48017-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48017-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48017-116">Not supported.</span></span>    |
|<span data-ttu-id="48017-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48017-117">Application</span></span> | <span data-ttu-id="48017-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48017-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48017-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48017-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="48017-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48017-120">Request headers</span></span>
| <span data-ttu-id="48017-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48017-121">Header</span></span>       | <span data-ttu-id="48017-122">Valor</span><span class="sxs-lookup"><span data-stu-id="48017-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48017-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48017-123">Authorization</span></span>  | <span data-ttu-id="48017-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48017-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48017-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="48017-126">Prefer</span></span> | <span data-ttu-id="48017-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="48017-127">return=minimal.</span></span> <span data-ttu-id="48017-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48017-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="48017-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="48017-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="48017-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48017-130">Request body</span></span>
<span data-ttu-id="48017-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48017-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48017-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="48017-132">Response</span></span>
<span data-ttu-id="48017-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48017-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48017-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48017-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="48017-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48017-136">Request</span></span>
<span data-ttu-id="48017-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48017-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48017-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="48017-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```
# <a name="c"></a>[<span data-ttu-id="48017-139">C#</span><span class="sxs-lookup"><span data-stu-id="48017-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48017-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48017-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48017-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48017-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="48017-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="48017-142">Response</span></span>
<span data-ttu-id="48017-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48017-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
