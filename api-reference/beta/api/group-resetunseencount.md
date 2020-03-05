---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para Grupos do Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c6500e7258026578e2adde35d0f194d1c42f9281
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418228"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="79d68-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="79d68-104">group: resetUnseenCount</span></span>

<span data-ttu-id="79d68-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79d68-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79d68-106">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita.</span><span class="sxs-lookup"><span data-stu-id="79d68-106">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="79d68-107">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="79d68-107">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="79d68-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="79d68-108">Permissions</span></span>
<span data-ttu-id="79d68-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79d68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79d68-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79d68-111">Permission type</span></span>      | <span data-ttu-id="79d68-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79d68-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79d68-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79d68-113">Delegated (work or school account)</span></span> | <span data-ttu-id="79d68-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d68-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="79d68-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79d68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79d68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79d68-116">Not supported.</span></span>    |
|<span data-ttu-id="79d68-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79d68-117">Application</span></span> | <span data-ttu-id="79d68-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79d68-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79d68-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79d68-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="79d68-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79d68-120">Request headers</span></span>
| <span data-ttu-id="79d68-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79d68-121">Header</span></span>       | <span data-ttu-id="79d68-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79d68-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79d68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79d68-123">Authorization</span></span>  | <span data-ttu-id="79d68-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79d68-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79d68-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="79d68-126">Prefer</span></span> | <span data-ttu-id="79d68-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="79d68-127">return=minimal.</span></span> <span data-ttu-id="79d68-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79d68-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="79d68-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="79d68-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="79d68-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79d68-130">Request body</span></span>
<span data-ttu-id="79d68-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79d68-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79d68-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="79d68-132">Response</span></span>
<span data-ttu-id="79d68-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79d68-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79d68-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79d68-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="79d68-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79d68-136">Request</span></span>
<span data-ttu-id="79d68-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79d68-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79d68-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="79d68-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="79d68-139">C#</span><span class="sxs-lookup"><span data-stu-id="79d68-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79d68-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79d68-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79d68-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79d68-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79d68-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="79d68-142">Response</span></span>
<span data-ttu-id="79d68-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79d68-143">The following is an example of the response.</span></span> 
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
