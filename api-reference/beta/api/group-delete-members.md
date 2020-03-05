---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 495548a2503b1c93486f6dbb590ffe85ab59676d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420441"
---
# <a name="remove-member"></a><span data-ttu-id="645a3-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="645a3-104">Remove member</span></span>

<span data-ttu-id="645a3-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="645a3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="645a3-106">Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.</span><span class="sxs-lookup"><span data-stu-id="645a3-106">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="645a3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="645a3-107">Permissions</span></span>
<span data-ttu-id="645a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="645a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="645a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="645a3-110">Permission type</span></span>      | <span data-ttu-id="645a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="645a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="645a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="645a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="645a3-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="645a3-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="645a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="645a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="645a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="645a3-115">Not supported.</span></span> |
|<span data-ttu-id="645a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="645a3-116">Application</span></span> | <span data-ttu-id="645a3-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="645a3-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="645a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="645a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="645a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="645a3-119">Request headers</span></span>
| <span data-ttu-id="645a3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="645a3-120">Name</span></span>       | <span data-ttu-id="645a3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="645a3-121">Type</span></span> | <span data-ttu-id="645a3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="645a3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="645a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="645a3-123">Authorization</span></span>  | <span data-ttu-id="645a3-124">string</span><span class="sxs-lookup"><span data-stu-id="645a3-124">string</span></span>  | <span data-ttu-id="645a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="645a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="645a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="645a3-127">Request body</span></span>
<span data-ttu-id="645a3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="645a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="645a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="645a3-129">Response</span></span>
<span data-ttu-id="645a3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="645a3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="645a3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="645a3-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="645a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="645a3-133">Request</span></span>
<span data-ttu-id="645a3-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="645a3-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="645a3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="645a3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="645a3-136">C#</span><span class="sxs-lookup"><span data-stu-id="645a3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="645a3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="645a3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="645a3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="645a3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="645a3-139">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="645a3-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="645a3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="645a3-140">Response</span></span>
<span data-ttu-id="645a3-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="645a3-141">The following is an example of the response.</span></span>
><span data-ttu-id="645a3-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="645a3-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="645a3-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="645a3-143">All the properties will be returned from an actual call.</span></span>
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
