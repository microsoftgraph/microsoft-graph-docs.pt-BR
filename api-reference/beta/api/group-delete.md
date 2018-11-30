---
title: Excluir grupo
description: Exclui um grupo.
ms.openlocfilehash: 92a15366fefb6ab70c45f664daa28b75bcea5891
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036176"
---
# <a name="delete-group"></a><span data-ttu-id="7ec2f-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="7ec2f-103">Delete group</span></span>

> <span data-ttu-id="7ec2f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ec2f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ec2f-106">Exclui um grupo.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-106">Deletes a group.</span></span>

<span data-ttu-id="7ec2f-107">Quando um grupo é excluído, o item é adicionado à [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="7ec2f-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="7ec2f-108">O grupo permanecerá em itens excluídos por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="7ec2f-109">Um grupo pode ser restaurado totalmente de itens excluídos durante os 30 dias.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="7ec2f-110">Após 30 dias, itens excluídos são excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ec2f-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="7ec2f-111">Permissions</span></span>
<span data-ttu-id="7ec2f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ec2f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ec2f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ec2f-114">Permission type</span></span>      | <span data-ttu-id="7ec2f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ec2f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ec2f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ec2f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7ec2f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ec2f-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ec2f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ec2f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ec2f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-119">Not supported.</span></span>    |
|<span data-ttu-id="7ec2f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ec2f-120">Application</span></span> | <span data-ttu-id="7ec2f-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ec2f-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ec2f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ec2f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ec2f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ec2f-123">Request headers</span></span>
| <span data-ttu-id="7ec2f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7ec2f-124">Name</span></span>       | <span data-ttu-id="7ec2f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ec2f-125">Type</span></span> | <span data-ttu-id="7ec2f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ec2f-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ec2f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ec2f-127">Authorization</span></span>  | <span data-ttu-id="7ec2f-128">string</span><span class="sxs-lookup"><span data-stu-id="7ec2f-128">string</span></span>  | <span data-ttu-id="7ec2f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ec2f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ec2f-131">Request body</span></span>
<span data-ttu-id="7ec2f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ec2f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ec2f-133">Response</span></span>
<span data-ttu-id="7ec2f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ec2f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ec2f-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7ec2f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ec2f-137">Request</span></span>
<span data-ttu-id="7ec2f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="7ec2f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ec2f-139">Response</span></span>
<span data-ttu-id="7ec2f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ec2f-140">The following is an example of the response.</span></span> 
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