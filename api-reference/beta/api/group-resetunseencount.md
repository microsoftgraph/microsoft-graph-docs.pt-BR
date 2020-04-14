---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ff1f80d8e716f0fe16ae4e34d40b8f40942f6e32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396305"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="e9fa7-103">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="e9fa7-103">group: resetUnseenCount</span></span>

<span data-ttu-id="e9fa7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9fa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9fa7-105">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="e9fa7-106">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9fa7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9fa7-107">Permissions</span></span>
<span data-ttu-id="e9fa7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9fa7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9fa7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9fa7-110">Permission type</span></span>      | <span data-ttu-id="e9fa7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9fa7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9fa7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9fa7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9fa7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9fa7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9fa7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9fa7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9fa7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-115">Not supported.</span></span>    |
|<span data-ttu-id="e9fa7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9fa7-116">Application</span></span> | <span data-ttu-id="e9fa7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9fa7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9fa7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="e9fa7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fa7-119">Request headers</span></span>
| <span data-ttu-id="e9fa7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9fa7-120">Header</span></span>       | <span data-ttu-id="e9fa7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e9fa7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9fa7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9fa7-122">Authorization</span></span>  | <span data-ttu-id="e9fa7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e9fa7-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="e9fa7-125">Prefer</span></span> | <span data-ttu-id="e9fa7-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-126">return=minimal.</span></span> <span data-ttu-id="e9fa7-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="e9fa7-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="e9fa7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fa7-129">Request body</span></span>
<span data-ttu-id="e9fa7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9fa7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9fa7-131">Response</span></span>
<span data-ttu-id="e9fa7-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9fa7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9fa7-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e9fa7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9fa7-135">Request</span></span>
<span data-ttu-id="e9fa7-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9fa7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9fa7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="e9fa7-138">C#</span><span class="sxs-lookup"><span data-stu-id="e9fa7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9fa7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9fa7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9fa7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9fa7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9fa7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9fa7-141">Response</span></span>
<span data-ttu-id="e9fa7-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9fa7-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
