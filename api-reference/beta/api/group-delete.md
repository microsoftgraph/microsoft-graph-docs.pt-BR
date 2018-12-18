---
title: Excluir grupo
description: Exclui um grupo.
author: dkershaw10
ms.openlocfilehash: ba159e5ce603d1da75b424f69a01f7bf8a3b2332
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341864"
---
# <a name="delete-group"></a><span data-ttu-id="35e44-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="35e44-103">Delete group</span></span>

> <span data-ttu-id="35e44-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="35e44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35e44-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="35e44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35e44-106">Exclui um grupo.</span><span class="sxs-lookup"><span data-stu-id="35e44-106">Deletes a group.</span></span>

<span data-ttu-id="35e44-107">Quando um grupo é excluído, o item é adicionado à [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="35e44-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="35e44-108">O grupo permanecerá em itens excluídos por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="35e44-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="35e44-109">Um grupo pode ser restaurado totalmente de itens excluídos durante os 30 dias.</span><span class="sxs-lookup"><span data-stu-id="35e44-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="35e44-110">Após 30 dias, itens excluídos são excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="35e44-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="35e44-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="35e44-111">Permissions</span></span>
<span data-ttu-id="35e44-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35e44-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35e44-114">Permission type</span></span>      | <span data-ttu-id="35e44-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35e44-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35e44-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35e44-116">Delegated (work or school account)</span></span> | <span data-ttu-id="35e44-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35e44-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="35e44-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35e44-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35e44-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35e44-119">Not supported.</span></span>    |
|<span data-ttu-id="35e44-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35e44-120">Application</span></span> | <span data-ttu-id="35e44-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35e44-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35e44-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35e44-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35e44-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35e44-123">Request headers</span></span>
| <span data-ttu-id="35e44-124">Nome</span><span class="sxs-lookup"><span data-stu-id="35e44-124">Name</span></span>       | <span data-ttu-id="35e44-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="35e44-125">Type</span></span> | <span data-ttu-id="35e44-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="35e44-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="35e44-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="35e44-127">Authorization</span></span>  | <span data-ttu-id="35e44-128">string</span><span class="sxs-lookup"><span data-stu-id="35e44-128">string</span></span>  | <span data-ttu-id="35e44-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35e44-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35e44-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35e44-131">Request body</span></span>
<span data-ttu-id="35e44-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35e44-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35e44-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="35e44-133">Response</span></span>
<span data-ttu-id="35e44-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35e44-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35e44-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35e44-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="35e44-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35e44-137">Request</span></span>
<span data-ttu-id="35e44-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35e44-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="35e44-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="35e44-139">Response</span></span>
<span data-ttu-id="35e44-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35e44-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->