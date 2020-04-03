---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7beced25495b7dfdf98951a7cfa8c93bfc633649
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123843"
---
# <a name="remove-member"></a><span data-ttu-id="f4072-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="f4072-104">Remove member</span></span>

<span data-ttu-id="f4072-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4072-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4072-106">Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.</span><span class="sxs-lookup"><span data-stu-id="f4072-106">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4072-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4072-107">Permissions</span></span>
<span data-ttu-id="f4072-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4072-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4072-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4072-110">Permission type</span></span>      | <span data-ttu-id="f4072-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4072-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4072-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4072-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4072-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4072-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f4072-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4072-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4072-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4072-115">Not supported.</span></span> |
|<span data-ttu-id="f4072-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4072-116">Application</span></span> | <span data-ttu-id="f4072-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4072-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4072-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4072-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f4072-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4072-119">Request headers</span></span>
| <span data-ttu-id="f4072-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f4072-120">Name</span></span>       | <span data-ttu-id="f4072-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4072-121">Type</span></span> | <span data-ttu-id="f4072-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4072-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4072-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4072-123">Authorization</span></span>  | <span data-ttu-id="f4072-124">string</span><span class="sxs-lookup"><span data-stu-id="f4072-124">string</span></span>  | <span data-ttu-id="f4072-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4072-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4072-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4072-127">Request body</span></span>
<span data-ttu-id="f4072-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4072-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4072-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4072-129">Response</span></span>
<span data-ttu-id="f4072-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4072-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4072-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4072-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f4072-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4072-133">Request</span></span>
<span data-ttu-id="f4072-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4072-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4072-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4072-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f4072-136">C#</span><span class="sxs-lookup"><span data-stu-id="f4072-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4072-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4072-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4072-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4072-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f4072-139">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="f4072-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="f4072-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4072-140">Response</span></span>
<span data-ttu-id="f4072-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f4072-141">The following is an example of the response.</span></span>
><span data-ttu-id="f4072-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4072-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f4072-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4072-143">All the properties will be returned from an actual call.</span></span>
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
