---
title: 'group: renew'
description: Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 533f82fa737c85fd816da04d75b712072d95a46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042006"
---
# <a name="group-renew"></a><span data-ttu-id="90455-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="90455-104">group: renew</span></span>

<span data-ttu-id="90455-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90455-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90455-106">Renova o período de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="90455-106">Renews a group's expiration.</span></span> <span data-ttu-id="90455-107">Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="90455-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="90455-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="90455-108">Permissions</span></span>

<span data-ttu-id="90455-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90455-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="90455-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90455-111">Permission type</span></span>      | <span data-ttu-id="90455-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90455-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90455-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90455-113">Delegated (work or school account)</span></span> | <span data-ttu-id="90455-114">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90455-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="90455-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90455-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90455-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="90455-116">Not supported</span></span> |
|<span data-ttu-id="90455-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90455-117">Application</span></span> | <span data-ttu-id="90455-118">Group.ReadWrite.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90455-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90455-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90455-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="90455-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90455-120">Request headers</span></span>
| <span data-ttu-id="90455-121">Nome</span><span class="sxs-lookup"><span data-stu-id="90455-121">Name</span></span>       | <span data-ttu-id="90455-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="90455-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90455-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90455-123">Authorization</span></span>  | <span data-ttu-id="90455-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90455-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="90455-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90455-126">Request body</span></span>

<span data-ttu-id="90455-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90455-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90455-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="90455-128">Response</span></span>

<span data-ttu-id="90455-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90455-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90455-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90455-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90455-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90455-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="90455-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90455-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="90455-134">C#</span><span class="sxs-lookup"><span data-stu-id="90455-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90455-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90455-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90455-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90455-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90455-137">Java</span><span class="sxs-lookup"><span data-stu-id="90455-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="90455-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="90455-138">Response</span></span>
<span data-ttu-id="90455-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90455-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

