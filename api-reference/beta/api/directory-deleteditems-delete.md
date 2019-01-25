---
title: Excluir permanentemente item
description: Exclui permanentemente um item de itens excluídos.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 048008e31bc5cd7884dd3d7e9259412070404d9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528197"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="bc5c3-103">Excluir permanentemente item</span><span class="sxs-lookup"><span data-stu-id="bc5c3-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc5c3-104">Exclui permanentemente um item de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="bc5c3-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="bc5c3-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="bc5c3-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="bc5c3-106">É possível excluir permanentemente um item de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="bc5c3-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="bc5c3-107">Mas, uma vez que um item é excluído permanentemente, ele **não pode** ser restaurado.</span><span class="sxs-lookup"><span data-stu-id="bc5c3-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc5c3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc5c3-108">Permissions</span></span>
<span data-ttu-id="bc5c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="bc5c3-111">Para usuários: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc5c3-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="bc5c3-112">Para grupos: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc5c3-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="bc5c3-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5c3-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bc5c3-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5c3-114">Request headers</span></span>
| <span data-ttu-id="bc5c3-115">Nome</span><span class="sxs-lookup"><span data-stu-id="bc5c3-115">Name</span></span>       | <span data-ttu-id="bc5c3-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5c3-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc5c3-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc5c3-117">Authorization</span></span>  | <span data-ttu-id="bc5c3-118">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="bc5c3-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="bc5c3-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc5c3-119">Accept</span></span>  | <span data-ttu-id="bc5c3-120">application/json</span><span class="sxs-lookup"><span data-stu-id="bc5c3-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc5c3-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5c3-121">Request body</span></span>
<span data-ttu-id="bc5c3-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc5c3-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc5c3-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5c3-123">Response</span></span>

<span data-ttu-id="bc5c3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc5c3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc5c3-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc5c3-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc5c3-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5c3-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="bc5c3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5c3-128">Response</span></span>
<span data-ttu-id="bc5c3-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc5c3-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
