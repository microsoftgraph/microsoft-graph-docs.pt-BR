---
title: Excluir grupo
description: Excluir o grupo.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b9d2e9cbe3a86906c815178b570cd6d7980ac89e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808306"
---
# <a name="delete-group"></a><span data-ttu-id="01ce9-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="01ce9-103">Delete group</span></span>
<span data-ttu-id="01ce9-104">Excluir o grupo.</span><span class="sxs-lookup"><span data-stu-id="01ce9-104">Delete group.</span></span>

## <a name="permissions"></a><span data-ttu-id="01ce9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="01ce9-105">Permissions</span></span>
<span data-ttu-id="01ce9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01ce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01ce9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01ce9-108">Permission type</span></span>      | <span data-ttu-id="01ce9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01ce9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01ce9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01ce9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01ce9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ce9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01ce9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01ce9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01ce9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01ce9-113">Not supported.</span></span>    |
|<span data-ttu-id="01ce9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01ce9-114">Application</span></span> | <span data-ttu-id="01ce9-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01ce9-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01ce9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01ce9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="01ce9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01ce9-117">Request headers</span></span>
| <span data-ttu-id="01ce9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="01ce9-118">Name</span></span>       | <span data-ttu-id="01ce9-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="01ce9-119">Type</span></span> | <span data-ttu-id="01ce9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="01ce9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01ce9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="01ce9-121">Authorization</span></span>  | <span data-ttu-id="01ce9-122">string</span><span class="sxs-lookup"><span data-stu-id="01ce9-122">string</span></span>  | <span data-ttu-id="01ce9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01ce9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01ce9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01ce9-125">Request body</span></span>
<span data-ttu-id="01ce9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01ce9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01ce9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="01ce9-127">Response</span></span>
<span data-ttu-id="01ce9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01ce9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01ce9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01ce9-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="01ce9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01ce9-131">Request</span></span>
<span data-ttu-id="01ce9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01ce9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="01ce9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="01ce9-133">Response</span></span>
<span data-ttu-id="01ce9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01ce9-134">The following is an example of the response.</span></span> 
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
