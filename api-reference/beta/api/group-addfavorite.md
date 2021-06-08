---
title: 'group: addFavorite'
description: Adicionar o grupo à lista de grupos de favoritos do usuário atual. Apenas grupos do Microsoft 365 são suportados.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1f8c0b327fabd60f52747cc7c78ff398709fe3ff
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786969"
---
# <a name="group-addfavorite"></a><span data-ttu-id="c8f23-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="c8f23-104">group: addFavorite</span></span>

<span data-ttu-id="c8f23-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8f23-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8f23-106">Adicionar o grupo à lista de grupos de favoritos do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="c8f23-106">Add the group to the list of the current user's favorite groups.</span></span> <span data-ttu-id="c8f23-107">Apenas grupos do Microsoft 365 são suportados.</span><span class="sxs-lookup"><span data-stu-id="c8f23-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8f23-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8f23-108">Permissions</span></span>
<span data-ttu-id="c8f23-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8f23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8f23-111">Permission type</span></span>      | <span data-ttu-id="c8f23-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8f23-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8f23-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8f23-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c8f23-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8f23-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c8f23-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8f23-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8f23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8f23-116">Not supported.</span></span>    |
|<span data-ttu-id="c8f23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8f23-117">Application</span></span> | <span data-ttu-id="c8f23-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8f23-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8f23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8f23-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="c8f23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f23-120">Request headers</span></span>
| <span data-ttu-id="c8f23-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8f23-121">Header</span></span>       | <span data-ttu-id="c8f23-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8f23-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8f23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8f23-123">Authorization</span></span>  | <span data-ttu-id="c8f23-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8f23-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c8f23-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="c8f23-126">Prefer</span></span> | <span data-ttu-id="c8f23-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="c8f23-127">return=minimal.</span></span> <span data-ttu-id="c8f23-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8f23-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="c8f23-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c8f23-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="c8f23-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f23-130">Request body</span></span>
<span data-ttu-id="c8f23-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8f23-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8f23-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f23-132">Response</span></span>
<span data-ttu-id="c8f23-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f23-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f23-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8f23-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c8f23-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8f23-136">Request</span></span>
<span data-ttu-id="c8f23-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8f23-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8f23-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8f23-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```
# <a name="c"></a>[<span data-ttu-id="c8f23-139">C#</span><span class="sxs-lookup"><span data-stu-id="c8f23-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-addfavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8f23-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8f23-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-addfavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8f23-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8f23-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-addfavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8f23-142">Java</span><span class="sxs-lookup"><span data-stu-id="c8f23-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-addfavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c8f23-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8f23-143">Response</span></span>
<span data-ttu-id="c8f23-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f23-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


