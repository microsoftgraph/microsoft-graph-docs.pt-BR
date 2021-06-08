---
title: 'group: renew'
description: Renova a expiração de um grupo. Quando um grupo é renovado, a expiração do grupo é estendida pelo número de dias definido na política.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 05fde82e6ae9bc3e3d7662e140605391ab08abdb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787762"
---
# <a name="group-renew"></a><span data-ttu-id="fdad7-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="fdad7-104">group: renew</span></span>

<span data-ttu-id="fdad7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdad7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdad7-p102">Renova a expiração de um grupo. Quando um grupo é renovado, a expiração do grupo é estendida pelo número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="fdad7-p102">Renews a group's expiration. When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdad7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdad7-108">Permissions</span></span>

<span data-ttu-id="fdad7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdad7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="fdad7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdad7-111">Permission type</span></span>      | <span data-ttu-id="fdad7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdad7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdad7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdad7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fdad7-114">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdad7-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="fdad7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdad7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdad7-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fdad7-116">Not supported</span></span> |
|<span data-ttu-id="fdad7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdad7-117">Application</span></span> | <span data-ttu-id="fdad7-118">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdad7-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdad7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdad7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="fdad7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdad7-120">Request headers</span></span>
| <span data-ttu-id="fdad7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fdad7-121">Name</span></span>       | <span data-ttu-id="fdad7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdad7-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fdad7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdad7-123">Authorization</span></span>  | <span data-ttu-id="fdad7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdad7-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="fdad7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdad7-126">Request body</span></span>

<span data-ttu-id="fdad7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdad7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdad7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdad7-128">Response</span></span>

<span data-ttu-id="fdad7-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdad7-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdad7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdad7-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fdad7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdad7-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fdad7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdad7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="fdad7-134">C#</span><span class="sxs-lookup"><span data-stu-id="fdad7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdad7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdad7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdad7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdad7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdad7-137">Java</span><span class="sxs-lookup"><span data-stu-id="fdad7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fdad7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdad7-138">Response</span></span>
<span data-ttu-id="fdad7-139">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fdad7-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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

