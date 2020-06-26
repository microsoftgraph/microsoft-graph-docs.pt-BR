---
title: 'group: unsubscribeByMail'
description: 'Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suportado somente para grupos do Microsoft 365. '
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: afbee22fc9c51cd9b7428b89677907efc3786c1c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897117"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="94e37-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="94e37-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="94e37-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e37-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94e37-106">Chamar esse método impedirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="94e37-106">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="94e37-107">Suportado somente para grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="94e37-107">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="94e37-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="94e37-108">Permissions</span></span>
<span data-ttu-id="94e37-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="94e37-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="94e37-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e37-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e37-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94e37-111">Permission type</span></span>      | <span data-ttu-id="94e37-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94e37-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94e37-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94e37-113">Delegated (work or school account)</span></span> | <span data-ttu-id="94e37-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e37-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="94e37-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94e37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94e37-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94e37-116">Not supported.</span></span>    |
|<span data-ttu-id="94e37-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94e37-117">Application</span></span> | <span data-ttu-id="94e37-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94e37-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94e37-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94e37-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="94e37-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94e37-120">Request headers</span></span>
| <span data-ttu-id="94e37-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94e37-121">Header</span></span>       | <span data-ttu-id="94e37-122">Valor</span><span class="sxs-lookup"><span data-stu-id="94e37-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94e37-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94e37-123">Authorization</span></span>  | <span data-ttu-id="94e37-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="94e37-124">Bearer {token}.</span></span> <span data-ttu-id="94e37-125">Required.</span><span class="sxs-lookup"><span data-stu-id="94e37-125">Required.</span></span>  |
| <span data-ttu-id="94e37-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="94e37-126">Prefer</span></span> | <span data-ttu-id="94e37-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="94e37-127">return=minimal.</span></span> <span data-ttu-id="94e37-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94e37-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="94e37-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="94e37-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="94e37-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94e37-130">Request body</span></span>
<span data-ttu-id="94e37-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94e37-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e37-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="94e37-132">Response</span></span>
<span data-ttu-id="94e37-133">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="94e37-133">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="94e37-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="94e37-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e37-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94e37-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="94e37-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94e37-136">Request</span></span>
<span data-ttu-id="94e37-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94e37-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94e37-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="94e37-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="94e37-139">C#</span><span class="sxs-lookup"><span data-stu-id="94e37-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94e37-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94e37-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94e37-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94e37-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94e37-142">Java</span><span class="sxs-lookup"><span data-stu-id="94e37-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94e37-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="94e37-143">Response</span></span>
<span data-ttu-id="94e37-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94e37-144">The following is an example of the response.</span></span> 
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
