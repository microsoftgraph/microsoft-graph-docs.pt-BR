---
title: 'group: unsubscribeByMail'
description: 'Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Apenas grupos do Microsoft 365 são suportados. '
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 68f2e82ab47476af870c55b78716c174da3b16b1
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682625"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="6188b-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="6188b-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="6188b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6188b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6188b-106">Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="6188b-106">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="6188b-107">Apenas grupos do Microsoft 365 são suportados.</span><span class="sxs-lookup"><span data-stu-id="6188b-107">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6188b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6188b-108">Permissions</span></span>
<span data-ttu-id="6188b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6188b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6188b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6188b-111">Permission type</span></span>      | <span data-ttu-id="6188b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6188b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6188b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6188b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6188b-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6188b-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6188b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6188b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6188b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6188b-116">Not supported.</span></span>    |
|<span data-ttu-id="6188b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6188b-117">Application</span></span> | <span data-ttu-id="6188b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6188b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6188b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6188b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="6188b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6188b-120">Request headers</span></span>
| <span data-ttu-id="6188b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6188b-121">Header</span></span>       | <span data-ttu-id="6188b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6188b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6188b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6188b-123">Authorization</span></span>  | <span data-ttu-id="6188b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6188b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6188b-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="6188b-126">Prefer</span></span> | <span data-ttu-id="6188b-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="6188b-127">return=minimal.</span></span> <span data-ttu-id="6188b-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6188b-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="6188b-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6188b-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="6188b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6188b-130">Request body</span></span>
<span data-ttu-id="6188b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6188b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6188b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6188b-132">Response</span></span>
<span data-ttu-id="6188b-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6188b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6188b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6188b-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6188b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6188b-136">Request</span></span>
<span data-ttu-id="6188b-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6188b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6188b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6188b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="6188b-139">C#</span><span class="sxs-lookup"><span data-stu-id="6188b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6188b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6188b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6188b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6188b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6188b-142">Java</span><span class="sxs-lookup"><span data-stu-id="6188b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6188b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6188b-143">Response</span></span>
<span data-ttu-id="6188b-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6188b-144">The following is an example of the response.</span></span> 
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

