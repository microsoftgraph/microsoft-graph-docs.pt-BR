---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para Grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a44ad6af1731dddf9fb0e124a837ba165f5d0e0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953462"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="b1c84-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="b1c84-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1c84-105">Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="b1c84-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="b1c84-106">Suporte apenas para Grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b1c84-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c84-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1c84-107">Permissions</span></span>
<span data-ttu-id="b1c84-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c84-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1c84-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1c84-110">Permission type</span></span>      | <span data-ttu-id="b1c84-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1c84-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1c84-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1c84-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1c84-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c84-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1c84-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1c84-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1c84-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c84-115">Not supported.</span></span>    |
|<span data-ttu-id="b1c84-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1c84-116">Application</span></span> | <span data-ttu-id="b1c84-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c84-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1c84-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c84-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="b1c84-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c84-119">Request headers</span></span>
| <span data-ttu-id="b1c84-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1c84-120">Header</span></span>       | <span data-ttu-id="b1c84-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b1c84-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1c84-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1c84-122">Authorization</span></span>  | <span data-ttu-id="b1c84-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1c84-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1c84-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="b1c84-125">Prefer</span></span> | <span data-ttu-id="b1c84-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="b1c84-126">return=minimal.</span></span> <span data-ttu-id="b1c84-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b1c84-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="b1c84-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b1c84-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b1c84-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c84-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b1c84-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c84-130">Response</span></span>
<span data-ttu-id="b1c84-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c84-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1c84-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1c84-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b1c84-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c84-134">Request</span></span>
<span data-ttu-id="b1c84-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1c84-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1c84-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c84-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1c84-137">C#</span><span class="sxs-lookup"><span data-stu-id="b1c84-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1c84-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1c84-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1c84-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b1c84-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1c84-140">Java</span><span class="sxs-lookup"><span data-stu-id="b1c84-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b1c84-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c84-141">Response</span></span>
<span data-ttu-id="b1c84-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c84-142">The following is an example of the response.</span></span> 
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
