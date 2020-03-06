---
title: 'group: unsubscribeByMail'
description: 'Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suporte apenas para grupos do Office 365. '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cc0375efe70482c248fa5f9d3168e2562f9416a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516925"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="2fef2-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="2fef2-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="2fef2-105">Namespace: Microsoft. Graph chamar este método impedirá que o usuário atual receba notificações por email para este grupo sobre novas postagens, eventos e arquivos nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="2fef2-105">Namespace: microsoft.graph Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="2fef2-106">Suportado somente para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2fef2-106">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2fef2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fef2-107">Permissions</span></span>
<span data-ttu-id="2fef2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fef2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fef2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fef2-110">Permission type</span></span>      | <span data-ttu-id="2fef2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fef2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fef2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fef2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2fef2-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fef2-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2fef2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fef2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fef2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fef2-115">Not supported.</span></span>    |
|<span data-ttu-id="2fef2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fef2-116">Application</span></span> | <span data-ttu-id="2fef2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fef2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fef2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fef2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="2fef2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fef2-119">Request headers</span></span>
| <span data-ttu-id="2fef2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fef2-120">Header</span></span>       | <span data-ttu-id="2fef2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2fef2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2fef2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fef2-122">Authorization</span></span>  | <span data-ttu-id="2fef2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fef2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2fef2-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="2fef2-125">Prefer</span></span> | <span data-ttu-id="2fef2-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="2fef2-126">return=minimal.</span></span> <span data-ttu-id="2fef2-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2fef2-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="2fef2-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2fef2-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="2fef2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fef2-129">Request body</span></span>
<span data-ttu-id="2fef2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fef2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fef2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fef2-131">Response</span></span>
<span data-ttu-id="2fef2-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fef2-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fef2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fef2-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2fef2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fef2-135">Request</span></span>
<span data-ttu-id="2fef2-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fef2-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fef2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fef2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="2fef2-138">C#</span><span class="sxs-lookup"><span data-stu-id="2fef2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fef2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fef2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fef2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fef2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fef2-141">Java</span><span class="sxs-lookup"><span data-stu-id="2fef2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fef2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fef2-142">Response</span></span>
<span data-ttu-id="2fef2-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2fef2-143">The following is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
