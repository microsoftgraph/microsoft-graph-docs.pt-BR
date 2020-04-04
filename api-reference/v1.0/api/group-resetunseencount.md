---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d0b6207eaa0329a1f664298955a57f2d6fbb1e9a
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144251"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="6994c-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="6994c-104">group: resetUnseenCount</span></span>

<span data-ttu-id="6994c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6994c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6994c-p102">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="6994c-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="6994c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6994c-108">Permissions</span></span>
<span data-ttu-id="6994c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6994c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6994c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6994c-111">Permission type</span></span>      | <span data-ttu-id="6994c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6994c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6994c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6994c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6994c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6994c-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6994c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6994c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6994c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6994c-116">Not supported.</span></span>    |
|<span data-ttu-id="6994c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6994c-117">Application</span></span> | <span data-ttu-id="6994c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6994c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6994c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6994c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="6994c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6994c-120">Request headers</span></span>
| <span data-ttu-id="6994c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6994c-121">Header</span></span>       | <span data-ttu-id="6994c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6994c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6994c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6994c-123">Authorization</span></span>  | <span data-ttu-id="6994c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6994c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6994c-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="6994c-126">Prefer</span></span> | <span data-ttu-id="6994c-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="6994c-127">return=minimal.</span></span> <span data-ttu-id="6994c-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6994c-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="6994c-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6994c-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="6994c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6994c-130">Request body</span></span>
<span data-ttu-id="6994c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6994c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6994c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6994c-132">Response</span></span>
<span data-ttu-id="6994c-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6994c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6994c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6994c-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6994c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6994c-136">Request</span></span>
<span data-ttu-id="6994c-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6994c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6994c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6994c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="6994c-139">C#</span><span class="sxs-lookup"><span data-stu-id="6994c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6994c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6994c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6994c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6994c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6994c-142">Java</span><span class="sxs-lookup"><span data-stu-id="6994c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6994c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6994c-143">Response</span></span>
<span data-ttu-id="6994c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6994c-144">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
