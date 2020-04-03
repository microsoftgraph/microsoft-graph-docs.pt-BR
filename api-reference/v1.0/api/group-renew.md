---
title: 'group: renew'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8e1e9403acf31df4544c5e894895aa17a1e86e2a
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124123"
---
# <a name="group-renew"></a><span data-ttu-id="c2ce0-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="c2ce0-104">group: renew</span></span>

<span data-ttu-id="c2ce0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2ce0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2ce0-106">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c2ce0-106">Renews a group's expiration.</span></span> <span data-ttu-id="c2ce0-107">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="c2ce0-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2ce0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2ce0-108">Permissions</span></span>

<span data-ttu-id="c2ce0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ce0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="c2ce0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2ce0-111">Permission type</span></span>      | <span data-ttu-id="c2ce0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2ce0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ce0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2ce0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c2ce0-114">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ce0-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2ce0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2ce0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ce0-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c2ce0-116">Not supported</span></span> |
|<span data-ttu-id="c2ce0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2ce0-117">Application</span></span> | <span data-ttu-id="c2ce0-118">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ce0-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2ce0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ce0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="c2ce0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2ce0-120">Request headers</span></span>
| <span data-ttu-id="c2ce0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c2ce0-121">Name</span></span>       | <span data-ttu-id="c2ce0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ce0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2ce0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2ce0-123">Authorization</span></span>  | <span data-ttu-id="c2ce0-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c2ce0-124">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="c2ce0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2ce0-125">Request body</span></span>

<span data-ttu-id="c2ce0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2ce0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2ce0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2ce0-127">Response</span></span>

<span data-ttu-id="c2ce0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2ce0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ce0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2ce0-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2ce0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2ce0-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2ce0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ce0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="c2ce0-133">C#</span><span class="sxs-lookup"><span data-stu-id="c2ce0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2ce0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2ce0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2ce0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2ce0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2ce0-136">Java</span><span class="sxs-lookup"><span data-stu-id="c2ce0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2ce0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2ce0-137">Response</span></span>
<span data-ttu-id="c2ce0-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2ce0-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
