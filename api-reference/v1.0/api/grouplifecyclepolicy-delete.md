---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
ms.openlocfilehash: af154d2ff5e7b61a245f3b99d22f10d26f0204fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007155"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="35816-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="35816-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="35816-104">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="35816-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35816-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="35816-105">Permissions</span></span>

<span data-ttu-id="35816-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35816-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35816-108">Permission type</span></span>      | <span data-ttu-id="35816-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35816-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35816-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35816-110">Delegated (work or school account)</span></span> | <span data-ttu-id="35816-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35816-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="35816-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35816-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35816-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35816-113">Not supported.</span></span>    |
|<span data-ttu-id="35816-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35816-114">Application</span></span> | <span data-ttu-id="35816-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35816-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35816-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35816-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="35816-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35816-117">Request headers</span></span>

| <span data-ttu-id="35816-118">Nome</span><span class="sxs-lookup"><span data-stu-id="35816-118">Name</span></span> | <span data-ttu-id="35816-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="35816-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="35816-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="35816-120">Authorization</span></span> | <span data-ttu-id="35816-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35816-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35816-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35816-123">Content-Type</span></span>  | <span data-ttu-id="35816-124">application/json</span><span class="sxs-lookup"><span data-stu-id="35816-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="35816-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35816-125">Request body</span></span>
<span data-ttu-id="35816-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35816-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="35816-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="35816-127">Response</span></span>

<span data-ttu-id="35816-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35816-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35816-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35816-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="35816-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35816-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="35816-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="35816-132">Response</span></span>

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