---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo. Suportado somente para grupos do Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8e3cb0d0a79da9ec246f0da50f17c3987695bb27
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897124"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="97c78-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="97c78-104">group: subscribeByMail</span></span>

<span data-ttu-id="97c78-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97c78-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97c78-106">Chamar esse método permitirá que o usuário atual receba notificações por email para este grupo, sobre novas postagens, eventos e arquivos do grupo.</span><span class="sxs-lookup"><span data-stu-id="97c78-106">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="97c78-107">Suportado somente para grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="97c78-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="97c78-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="97c78-108">Permissions</span></span>
<span data-ttu-id="97c78-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="97c78-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="97c78-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97c78-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97c78-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97c78-111">Permission type</span></span>      | <span data-ttu-id="97c78-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97c78-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97c78-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97c78-113">Delegated (work or school account)</span></span> | <span data-ttu-id="97c78-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97c78-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97c78-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97c78-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97c78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97c78-116">Not supported.</span></span>    |
|<span data-ttu-id="97c78-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97c78-117">Application</span></span> | <span data-ttu-id="97c78-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97c78-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97c78-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97c78-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="97c78-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97c78-120">Request headers</span></span>
| <span data-ttu-id="97c78-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97c78-121">Header</span></span>       | <span data-ttu-id="97c78-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97c78-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97c78-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97c78-123">Authorization</span></span>  | <span data-ttu-id="97c78-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="97c78-124">Bearer {token}.</span></span> <span data-ttu-id="97c78-125">Required.</span><span class="sxs-lookup"><span data-stu-id="97c78-125">Required.</span></span>  |
| <span data-ttu-id="97c78-126">Preferir</span><span class="sxs-lookup"><span data-stu-id="97c78-126">Prefer</span></span> | <span data-ttu-id="97c78-127">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="97c78-127">return=minimal.</span></span> <span data-ttu-id="97c78-128">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97c78-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="97c78-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97c78-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="97c78-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97c78-130">Request body</span></span>
<span data-ttu-id="97c78-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97c78-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97c78-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c78-132">Response</span></span>
<span data-ttu-id="97c78-133">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="97c78-133">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="97c78-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="97c78-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97c78-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97c78-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="97c78-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97c78-136">Request</span></span>
<span data-ttu-id="97c78-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97c78-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97c78-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="97c78-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="97c78-139">C#</span><span class="sxs-lookup"><span data-stu-id="97c78-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97c78-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97c78-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97c78-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97c78-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97c78-142">Java</span><span class="sxs-lookup"><span data-stu-id="97c78-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97c78-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c78-143">Response</span></span>
<span data-ttu-id="97c78-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97c78-144">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
