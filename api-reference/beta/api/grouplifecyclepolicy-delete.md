---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
ms.openlocfilehash: 41c679a9fa2a55a0137d1197f08515e64750d4dc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361961"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="d85dc-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d85dc-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="d85dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d85dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d85dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d85dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d85dc-106">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d85dc-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d85dc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d85dc-107">Permissions</span></span>

<span data-ttu-id="d85dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d85dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d85dc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d85dc-110">Permission type</span></span>      | <span data-ttu-id="d85dc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d85dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d85dc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d85dc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d85dc-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85dc-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d85dc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d85dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d85dc-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d85dc-115">Not supported</span></span> |
|<span data-ttu-id="d85dc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d85dc-116">Application</span></span> | <span data-ttu-id="d85dc-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85dc-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d85dc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d85dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="d85dc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d85dc-119">Request headers</span></span>

| <span data-ttu-id="d85dc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d85dc-120">Name</span></span> | <span data-ttu-id="d85dc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d85dc-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d85dc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d85dc-122">Authorization</span></span> | <span data-ttu-id="d85dc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d85dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d85dc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d85dc-125">Content-Type</span></span>  | <span data-ttu-id="d85dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d85dc-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d85dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d85dc-127">Request body</span></span>
<span data-ttu-id="d85dc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d85dc-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d85dc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d85dc-129">Response</span></span>

<span data-ttu-id="d85dc-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d85dc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d85dc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d85dc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d85dc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d85dc-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="d85dc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d85dc-134">Response</span></span>

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