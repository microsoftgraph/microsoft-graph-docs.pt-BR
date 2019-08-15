---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6100e85ec3088eea6d7ad491be69b6d718ae0a43
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420321"
---
# <a name="remove-member"></a><span data-ttu-id="bcddd-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="bcddd-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcddd-105">Use essa API para remover um membro de um grupo por meio \*\*\*\* da propriedade de navegação Members.</span><span class="sxs-lookup"><span data-stu-id="bcddd-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcddd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcddd-106">Permissions</span></span>
<span data-ttu-id="bcddd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcddd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcddd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcddd-109">Permission type</span></span>      | <span data-ttu-id="bcddd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcddd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcddd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcddd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bcddd-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bcddd-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bcddd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcddd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcddd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcddd-114">Not supported.</span></span> |
|<span data-ttu-id="bcddd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcddd-115">Application</span></span> | <span data-ttu-id="bcddd-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcddd-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcddd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcddd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bcddd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcddd-118">Request headers</span></span>
| <span data-ttu-id="bcddd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bcddd-119">Name</span></span>       | <span data-ttu-id="bcddd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcddd-120">Type</span></span> | <span data-ttu-id="bcddd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcddd-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcddd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcddd-122">Authorization</span></span>  | <span data-ttu-id="bcddd-123">string</span><span class="sxs-lookup"><span data-stu-id="bcddd-123">string</span></span>  | <span data-ttu-id="bcddd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcddd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcddd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcddd-126">Request body</span></span>
<span data-ttu-id="bcddd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcddd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcddd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcddd-128">Response</span></span>
<span data-ttu-id="bcddd-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcddd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcddd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcddd-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bcddd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcddd-132">Request</span></span>
<span data-ttu-id="bcddd-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcddd-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcddd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcddd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcddd-135">C#</span><span class="sxs-lookup"><span data-stu-id="bcddd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcddd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcddd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcddd-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bcddd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bcddd-138">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="bcddd-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="bcddd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcddd-139">Response</span></span>
<span data-ttu-id="bcddd-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcddd-140">The following is an example of the response.</span></span>
><span data-ttu-id="bcddd-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bcddd-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bcddd-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcddd-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
