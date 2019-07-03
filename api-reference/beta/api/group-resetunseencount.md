---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para Grupos do Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6651cf4d8b4812bb1eba2b4d281643606c5d6d58
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442787"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="2692b-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="2692b-104">group: resetUnseenCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2692b-105">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita.</span><span class="sxs-lookup"><span data-stu-id="2692b-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="2692b-106">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2692b-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="2692b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2692b-107">Permissions</span></span>
<span data-ttu-id="2692b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2692b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2692b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2692b-110">Permission type</span></span>      | <span data-ttu-id="2692b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2692b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2692b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2692b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2692b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2692b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2692b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2692b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2692b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2692b-115">Not supported.</span></span>    |
|<span data-ttu-id="2692b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2692b-116">Application</span></span> | <span data-ttu-id="2692b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2692b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2692b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2692b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="2692b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2692b-119">Request headers</span></span>
| <span data-ttu-id="2692b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2692b-120">Header</span></span>       | <span data-ttu-id="2692b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2692b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2692b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2692b-122">Authorization</span></span>  | <span data-ttu-id="2692b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2692b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2692b-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="2692b-125">Prefer</span></span> | <span data-ttu-id="2692b-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="2692b-126">return=minimal.</span></span> <span data-ttu-id="2692b-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2692b-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="2692b-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2692b-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="2692b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2692b-129">Request body</span></span>
<span data-ttu-id="2692b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2692b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2692b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2692b-131">Response</span></span>
<span data-ttu-id="2692b-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2692b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2692b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2692b-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2692b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2692b-135">Request</span></span>
<span data-ttu-id="2692b-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2692b-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2692b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2692b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2692b-138">C#</span><span class="sxs-lookup"><span data-stu-id="2692b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2692b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="2692b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2692b-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2692b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2692b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2692b-141">Response</span></span>
<span data-ttu-id="2692b-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2692b-142">The following is an example of the response.</span></span> 
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
