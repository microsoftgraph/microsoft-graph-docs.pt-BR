---
title: Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy
description: Exclui um conjunto de condições excluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7cafcdfb6ee92a3913fd82f338c3607dec9c00bd
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433501"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="613ae-103">Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="613ae-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="613ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="613ae-105">Exclui [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção **Excludes** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="613ae-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="613ae-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="613ae-106">Permissions</span></span>

<span data-ttu-id="613ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="613ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="613ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="613ae-109">Permission type</span></span>      | <span data-ttu-id="613ae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="613ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="613ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="613ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="613ae-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="613ae-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="613ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="613ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="613ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="613ae-114">Not supported.</span></span>    |
| <span data-ttu-id="613ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="613ae-115">Application</span></span> | <span data-ttu-id="613ae-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="613ae-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="613ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="613ae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="613ae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="613ae-118">Request headers</span></span>

| <span data-ttu-id="613ae-119">Nome</span><span class="sxs-lookup"><span data-stu-id="613ae-119">Name</span></span>       | <span data-ttu-id="613ae-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="613ae-120">Type</span></span> | <span data-ttu-id="613ae-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="613ae-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="613ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="613ae-122">Authorization</span></span>  | <span data-ttu-id="613ae-123">string</span><span class="sxs-lookup"><span data-stu-id="613ae-123">string</span></span>  | <span data-ttu-id="613ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="613ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="613ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="613ae-126">Request body</span></span>

<span data-ttu-id="613ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="613ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="613ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="613ae-128">Response</span></span>

<span data-ttu-id="613ae-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="613ae-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="613ae-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="613ae-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="613ae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="613ae-132">Request</span></span>

<span data-ttu-id="613ae-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="613ae-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```

### <a name="response"></a><span data-ttu-id="613ae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="613ae-134">Response</span></span>

<span data-ttu-id="613ae-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="613ae-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
