---
title: 'group: removeFavorite'
description: Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b3279fb525b6556eadee6dd35a2d090b0e3ff9f2
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345846"
---
# <a name="group-removefavorite"></a><span data-ttu-id="ea9ad-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="ea9ad-104">group: removeFavorite</span></span>

<span data-ttu-id="ea9ad-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea9ad-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea9ad-p102">Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-p102">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea9ad-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea9ad-108">Permissions</span></span>
<span data-ttu-id="ea9ad-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea9ad-111">Permission type</span></span>      | <span data-ttu-id="ea9ad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea9ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea9ad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea9ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ea9ad-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9ad-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea9ad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea9ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea9ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-116">Not supported.</span></span>    |
|<span data-ttu-id="ea9ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea9ad-117">Application</span></span> | <span data-ttu-id="ea9ad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea9ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea9ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="ea9ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9ad-120">Request headers</span></span>
| <span data-ttu-id="ea9ad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea9ad-121">Header</span></span>       | <span data-ttu-id="ea9ad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea9ad-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea9ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea9ad-123">Authorization</span></span>  | <span data-ttu-id="ea9ad-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea9ad-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="ea9ad-126">Prefer</span></span> | <span data-ttu-id="ea9ad-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-127">return=minimal.</span></span> <span data-ttu-id="ea9ad-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="ea9ad-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ea9ad-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9ad-130">Request body</span></span>
<span data-ttu-id="ea9ad-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea9ad-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea9ad-132">Response</span></span>
<span data-ttu-id="ea9ad-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea9ad-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea9ad-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ea9ad-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea9ad-136">Request</span></span>
<span data-ttu-id="ea9ad-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea9ad-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea9ad-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```
# <a name="c"></a>[<span data-ttu-id="ea9ad-139">C#</span><span class="sxs-lookup"><span data-stu-id="ea9ad-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea9ad-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea9ad-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea9ad-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea9ad-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea9ad-142">Java</span><span class="sxs-lookup"><span data-stu-id="ea9ad-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removefavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ea9ad-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea9ad-143">Response</span></span>
<span data-ttu-id="ea9ad-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea9ad-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
