---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 12e26fb08f12f0cf177836baf0b5906237953f56
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263326"
---
# <a name="remove-member"></a><span data-ttu-id="65a3f-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="65a3f-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65a3f-105">Use essa API para remover um membro de um grupo por meio \*\*\*\* da propriedade de navegação Members.</span><span class="sxs-lookup"><span data-stu-id="65a3f-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="65a3f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65a3f-106">Permissions</span></span>
<span data-ttu-id="65a3f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65a3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65a3f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65a3f-109">Permission type</span></span>      | <span data-ttu-id="65a3f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65a3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65a3f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65a3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="65a3f-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65a3f-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="65a3f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65a3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65a3f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65a3f-114">Not supported.</span></span> |
|<span data-ttu-id="65a3f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65a3f-115">Application</span></span> | <span data-ttu-id="65a3f-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a3f-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65a3f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65a3f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="65a3f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65a3f-118">Request headers</span></span>
| <span data-ttu-id="65a3f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="65a3f-119">Name</span></span>       | <span data-ttu-id="65a3f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="65a3f-120">Type</span></span> | <span data-ttu-id="65a3f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="65a3f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="65a3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="65a3f-122">Authorization</span></span>  | <span data-ttu-id="65a3f-123">string</span><span class="sxs-lookup"><span data-stu-id="65a3f-123">string</span></span>  | <span data-ttu-id="65a3f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65a3f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65a3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65a3f-126">Request body</span></span>
<span data-ttu-id="65a3f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65a3f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65a3f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="65a3f-128">Response</span></span>
<span data-ttu-id="65a3f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65a3f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65a3f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65a3f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="65a3f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65a3f-132">Request</span></span>
<span data-ttu-id="65a3f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65a3f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="65a3f-134">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="65a3f-134">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="65a3f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="65a3f-135">Response</span></span>
<span data-ttu-id="65a3f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65a3f-136">The following is an example of the response.</span></span>
><span data-ttu-id="65a3f-137">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65a3f-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65a3f-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65a3f-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="65a3f-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="65a3f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="65a3f-140">C#</span><span class="sxs-lookup"><span data-stu-id="65a3f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65a3f-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="65a3f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="65a3f-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="65a3f-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
