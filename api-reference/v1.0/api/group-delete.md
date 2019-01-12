---
title: Excluir grupo
description: Excluir o grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 65fd34fe01a2543389356e86334e986332210b08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968607"
---
# <a name="delete-group"></a><span data-ttu-id="0ac7e-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="0ac7e-103">Delete group</span></span>
<span data-ttu-id="0ac7e-104">Excluir o grupo.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-104">Delete group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac7e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ac7e-105">Permissions</span></span>
<span data-ttu-id="0ac7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ac7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac7e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ac7e-108">Permission type</span></span>      | <span data-ttu-id="0ac7e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ac7e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ac7e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ac7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ac7e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac7e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ac7e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ac7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac7e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-113">Not supported.</span></span>    |
|<span data-ttu-id="0ac7e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ac7e-114">Application</span></span> | <span data-ttu-id="0ac7e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac7e-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ac7e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ac7e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac7e-117">Request headers</span></span>
| <span data-ttu-id="0ac7e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0ac7e-118">Name</span></span>       | <span data-ttu-id="0ac7e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ac7e-119">Type</span></span> | <span data-ttu-id="0ac7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ac7e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ac7e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ac7e-121">Authorization</span></span>  | <span data-ttu-id="0ac7e-122">string</span><span class="sxs-lookup"><span data-stu-id="0ac7e-122">string</span></span>  | <span data-ttu-id="0ac7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ac7e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac7e-125">Request body</span></span>
<span data-ttu-id="0ac7e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ac7e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac7e-127">Response</span></span>
<span data-ttu-id="0ac7e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac7e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ac7e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0ac7e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac7e-131">Request</span></span>
<span data-ttu-id="0ac7e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="0ac7e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac7e-133">Response</span></span>
<span data-ttu-id="0ac7e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac7e-134">The following is an example of the response.</span></span> 
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
