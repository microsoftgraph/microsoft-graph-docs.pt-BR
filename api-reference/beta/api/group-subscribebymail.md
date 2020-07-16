---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d5865086ff1fd97af8e9897cde66a5cdd1599923
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895787"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="5998b-103">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="5998b-103">group: subscribeByMail</span></span>

<span data-ttu-id="5998b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5998b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5998b-105">Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="5998b-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="5998b-106">Suportado somente para grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5998b-106">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="5998b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5998b-107">Permissions</span></span>
<span data-ttu-id="5998b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5998b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5998b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5998b-110">Permission type</span></span>      | <span data-ttu-id="5998b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5998b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5998b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5998b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5998b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5998b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5998b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5998b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5998b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5998b-115">Not supported.</span></span>    |
|<span data-ttu-id="5998b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5998b-116">Application</span></span> | <span data-ttu-id="5998b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5998b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5998b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5998b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="5998b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5998b-119">Request headers</span></span>
| <span data-ttu-id="5998b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5998b-120">Header</span></span>       | <span data-ttu-id="5998b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5998b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5998b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5998b-122">Authorization</span></span>  | <span data-ttu-id="5998b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5998b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5998b-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="5998b-125">Prefer</span></span> | <span data-ttu-id="5998b-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="5998b-126">return=minimal.</span></span> <span data-ttu-id="5998b-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5998b-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="5998b-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5998b-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="5998b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5998b-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5998b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5998b-130">Response</span></span>
<span data-ttu-id="5998b-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5998b-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5998b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5998b-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5998b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5998b-134">Request</span></span>
<span data-ttu-id="5998b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5998b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5998b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5998b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="5998b-137">C#</span><span class="sxs-lookup"><span data-stu-id="5998b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5998b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5998b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5998b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5998b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5998b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5998b-140">Response</span></span>
<span data-ttu-id="5998b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5998b-141">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
