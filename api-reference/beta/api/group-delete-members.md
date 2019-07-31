---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b73ed8d1fc599a3c65b9b08e3caffcfc272bb332
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954043"
---
# <a name="remove-member"></a><span data-ttu-id="0ceed-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="0ceed-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ceed-105">Use essa API para remover um membro de um grupo por meio \*\*\*\* da propriedade de navegação Members.</span><span class="sxs-lookup"><span data-stu-id="0ceed-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ceed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ceed-106">Permissions</span></span>
<span data-ttu-id="0ceed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ceed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ceed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ceed-109">Permission type</span></span>      | <span data-ttu-id="0ceed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ceed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ceed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ceed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ceed-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ceed-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0ceed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ceed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ceed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ceed-114">Not supported.</span></span> |
|<span data-ttu-id="0ceed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ceed-115">Application</span></span> | <span data-ttu-id="0ceed-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceed-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ceed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ceed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0ceed-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ceed-118">Request headers</span></span>
| <span data-ttu-id="0ceed-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0ceed-119">Name</span></span>       | <span data-ttu-id="0ceed-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ceed-120">Type</span></span> | <span data-ttu-id="0ceed-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ceed-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ceed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ceed-122">Authorization</span></span>  | <span data-ttu-id="0ceed-123">string</span><span class="sxs-lookup"><span data-stu-id="0ceed-123">string</span></span>  | <span data-ttu-id="0ceed-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ceed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ceed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ceed-126">Request body</span></span>
<span data-ttu-id="0ceed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ceed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ceed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ceed-128">Response</span></span>
<span data-ttu-id="0ceed-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ceed-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ceed-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ceed-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0ceed-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ceed-132">Request</span></span>
<span data-ttu-id="0ceed-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ceed-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ceed-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ceed-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ceed-135">C#</span><span class="sxs-lookup"><span data-stu-id="0ceed-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ceed-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ceed-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ceed-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ceed-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ceed-138">Java</span><span class="sxs-lookup"><span data-stu-id="0ceed-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0ceed-139">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="0ceed-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="0ceed-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ceed-140">Response</span></span>
<span data-ttu-id="0ceed-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ceed-141">The following is an example of the response.</span></span>
><span data-ttu-id="0ceed-142">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ceed-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ceed-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ceed-143">All the properties will be returned from an actual call.</span></span>
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
