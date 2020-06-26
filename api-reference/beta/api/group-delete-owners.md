---
title: Remover proprietário
description: Use esta API para remover um proprietário de um grupo do Microsoft 365, um grupo de segurança ou um grupo de segurança habilitado para email por meio da propriedade de navegação owners.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 89e400b56bb4fd3aa318e29d3863c63a3e0af5f6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895857"
---
# <a name="remove-owner"></a><span data-ttu-id="6b5dd-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="6b5dd-103">Remove owner</span></span>

<span data-ttu-id="6b5dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b5dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b5dd-105">Use esta API para remover um proprietário de um grupo do Microsoft 365, um grupo de segurança ou um grupo de segurança habilitado para email por meio da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b5dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b5dd-106">Permissions</span></span>
<span data-ttu-id="6b5dd-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6b5dd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b5dd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b5dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b5dd-109">Permission type</span></span>      | <span data-ttu-id="6b5dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b5dd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b5dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b5dd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b5dd-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b5dd-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b5dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b5dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b5dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-114">Not supported.</span></span>    |
|<span data-ttu-id="6b5dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b5dd-115">Application</span></span> | <span data-ttu-id="6b5dd-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b5dd-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b5dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6b5dd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5dd-118">Request headers</span></span>
| <span data-ttu-id="6b5dd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b5dd-119">Name</span></span>       | <span data-ttu-id="6b5dd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b5dd-120">Type</span></span> | <span data-ttu-id="6b5dd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b5dd-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b5dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b5dd-122">Authorization</span></span>  | <span data-ttu-id="6b5dd-123">string</span><span class="sxs-lookup"><span data-stu-id="6b5dd-123">string</span></span>  | <span data-ttu-id="6b5dd-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-124">Bearer {token}.</span></span> <span data-ttu-id="6b5dd-125">Required.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b5dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5dd-126">Request body</span></span>
<span data-ttu-id="6b5dd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b5dd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b5dd-128">Response</span></span>
<span data-ttu-id="6b5dd-129">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="6b5dd-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-130">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b5dd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b5dd-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6b5dd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5dd-132">Request</span></span>
<span data-ttu-id="6b5dd-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b5dd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5dd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6b5dd-135">C#</span><span class="sxs-lookup"><span data-stu-id="6b5dd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b5dd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b5dd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b5dd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b5dd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6b5dd-138">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="6b5dd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b5dd-139">Response</span></span>
<span data-ttu-id="6b5dd-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-140">The following is an example of the response.</span></span>
><span data-ttu-id="6b5dd-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6b5dd-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b5dd-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
