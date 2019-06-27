---
title: Excluir permanentemente item
description: Exclui permanentemente um item de itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb2738de749cf5b35188792c440d7189d788dc3a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260897"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="69204-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="69204-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69204-104">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="69204-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="69204-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="69204-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="69204-106">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="69204-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="69204-107">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="69204-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="69204-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="69204-108">Permissions</span></span>
<span data-ttu-id="69204-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69204-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="69204-111">Para usuários: user. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="69204-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="69204-112">Para grupos: Group. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="69204-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="69204-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69204-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="69204-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69204-114">Request headers</span></span>
| <span data-ttu-id="69204-115">Nome</span><span class="sxs-lookup"><span data-stu-id="69204-115">Name</span></span>       | <span data-ttu-id="69204-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="69204-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69204-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="69204-117">Authorization</span></span>  | <span data-ttu-id="69204-118">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="69204-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="69204-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69204-119">Accept</span></span>  | <span data-ttu-id="69204-120">application/json</span><span class="sxs-lookup"><span data-stu-id="69204-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="69204-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69204-121">Request body</span></span>
<span data-ttu-id="69204-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69204-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69204-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="69204-123">Response</span></span>

<span data-ttu-id="69204-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69204-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69204-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69204-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69204-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69204-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="69204-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="69204-128">Response</span></span>
<span data-ttu-id="69204-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69204-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="69204-131">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="69204-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="69204-132">C#</span><span class="sxs-lookup"><span data-stu-id="69204-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69204-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="69204-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="69204-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="69204-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
