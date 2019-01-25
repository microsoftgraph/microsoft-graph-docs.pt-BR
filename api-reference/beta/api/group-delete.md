---
title: Excluir grupo
description: Exclui um grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 349900cffa4b0df1763e1ed8b8213ce81ec27351
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529961"
---
# <a name="delete-group"></a><span data-ttu-id="5e2ab-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="5e2ab-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e2ab-104">Exclui um grupo.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-104">Deletes a group.</span></span>

<span data-ttu-id="5e2ab-105">Quando um grupo é excluído, o item é adicionado à [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="5e2ab-105">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="5e2ab-106">O grupo permanecerá em itens excluídos por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-106">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="5e2ab-107">Um grupo pode ser restaurado totalmente de itens excluídos durante os 30 dias.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-107">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="5e2ab-108">Após 30 dias, itens excluídos são excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-108">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e2ab-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e2ab-109">Permissions</span></span>
<span data-ttu-id="5e2ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e2ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e2ab-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e2ab-112">Permission type</span></span>      | <span data-ttu-id="5e2ab-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e2ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e2ab-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e2ab-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5e2ab-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e2ab-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e2ab-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e2ab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e2ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-117">Not supported.</span></span>    |
|<span data-ttu-id="5e2ab-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e2ab-118">Application</span></span> | <span data-ttu-id="5e2ab-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e2ab-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e2ab-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2ab-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e2ab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2ab-121">Request headers</span></span>
| <span data-ttu-id="5e2ab-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5e2ab-122">Name</span></span>       | <span data-ttu-id="5e2ab-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e2ab-123">Type</span></span> | <span data-ttu-id="5e2ab-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e2ab-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5e2ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e2ab-125">Authorization</span></span>  | <span data-ttu-id="5e2ab-126">string</span><span class="sxs-lookup"><span data-stu-id="5e2ab-126">string</span></span>  | <span data-ttu-id="5e2ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e2ab-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2ab-129">Request body</span></span>
<span data-ttu-id="5e2ab-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e2ab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e2ab-131">Response</span></span>
<span data-ttu-id="5e2ab-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e2ab-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e2ab-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5e2ab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e2ab-135">Request</span></span>
<span data-ttu-id="5e2ab-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="5e2ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e2ab-137">Response</span></span>
<span data-ttu-id="5e2ab-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5e2ab-138">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
