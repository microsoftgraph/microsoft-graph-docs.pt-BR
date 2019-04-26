---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 24d80596194dd83b78f3eca73531b48e0181fbf3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328493"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="69120-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="69120-103">Delete groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69120-104">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="69120-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69120-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="69120-105">Permissions</span></span>

<span data-ttu-id="69120-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69120-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69120-108">Permission type</span></span>      | <span data-ttu-id="69120-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69120-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69120-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69120-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69120-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69120-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="69120-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69120-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69120-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="69120-113">Not supported</span></span> |
|<span data-ttu-id="69120-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69120-114">Application</span></span> | <span data-ttu-id="69120-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69120-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69120-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69120-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="69120-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69120-117">Request headers</span></span>

| <span data-ttu-id="69120-118">Nome</span><span class="sxs-lookup"><span data-stu-id="69120-118">Name</span></span> | <span data-ttu-id="69120-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="69120-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="69120-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="69120-120">Authorization</span></span> | <span data-ttu-id="69120-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69120-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69120-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69120-123">Content-Type</span></span>  | <span data-ttu-id="69120-124">application/json</span><span class="sxs-lookup"><span data-stu-id="69120-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="69120-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69120-125">Request body</span></span>
<span data-ttu-id="69120-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69120-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="69120-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="69120-127">Response</span></span>

<span data-ttu-id="69120-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69120-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69120-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69120-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69120-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69120-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="69120-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="69120-132">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
