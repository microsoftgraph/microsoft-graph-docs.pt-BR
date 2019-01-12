---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9d58eca82c72008cb30095fe4fbfacf5a382111a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922778"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="23588-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="23588-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="23588-104">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="23588-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23588-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="23588-105">Permissions</span></span>

<span data-ttu-id="23588-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23588-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23588-108">Permission type</span></span>      | <span data-ttu-id="23588-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23588-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23588-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23588-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23588-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23588-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="23588-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23588-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23588-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23588-113">Not supported.</span></span>    |
|<span data-ttu-id="23588-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23588-114">Application</span></span> | <span data-ttu-id="23588-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23588-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23588-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23588-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="23588-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23588-117">Request headers</span></span>

| <span data-ttu-id="23588-118">Nome</span><span class="sxs-lookup"><span data-stu-id="23588-118">Name</span></span> | <span data-ttu-id="23588-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="23588-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="23588-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="23588-120">Authorization</span></span> | <span data-ttu-id="23588-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23588-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23588-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23588-123">Content-Type</span></span>  | <span data-ttu-id="23588-124">application/json</span><span class="sxs-lookup"><span data-stu-id="23588-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="23588-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23588-125">Request body</span></span>
<span data-ttu-id="23588-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23588-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="23588-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="23588-127">Response</span></span>

<span data-ttu-id="23588-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23588-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23588-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23588-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23588-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23588-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="23588-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="23588-132">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
