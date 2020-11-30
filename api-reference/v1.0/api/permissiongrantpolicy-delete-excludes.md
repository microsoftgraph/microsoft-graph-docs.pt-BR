---
title: Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy
description: Exclui um conjunto de condições excluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 981693c50cfc2784cdb48a6eeecf00cab1910123
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377136"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="7eb2a-103">Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="7eb2a-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="7eb2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7eb2a-105">Exclui [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção **Excludes** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7eb2a-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7eb2a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7eb2a-106">Permissions</span></span>

<span data-ttu-id="7eb2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eb2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7eb2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7eb2a-109">Permission type</span></span>      | <span data-ttu-id="7eb2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7eb2a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="7eb2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7eb2a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7eb2a-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7eb2a-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="7eb2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7eb2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eb2a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7eb2a-114">Not supported.</span></span>    |
| <span data-ttu-id="7eb2a-115">Application</span><span class="sxs-lookup"><span data-stu-id="7eb2a-115">Application</span></span> | <span data-ttu-id="7eb2a-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7eb2a-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7eb2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="7eb2a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb2a-118">Request headers</span></span>

| <span data-ttu-id="7eb2a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7eb2a-119">Name</span></span>       | <span data-ttu-id="7eb2a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eb2a-120">Type</span></span> | <span data-ttu-id="7eb2a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb2a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7eb2a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7eb2a-122">Authorization</span></span>  | <span data-ttu-id="7eb2a-123">string</span><span class="sxs-lookup"><span data-stu-id="7eb2a-123">string</span></span>  | <span data-ttu-id="7eb2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7eb2a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7eb2a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb2a-126">Request body</span></span>

<span data-ttu-id="7eb2a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7eb2a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eb2a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb2a-128">Response</span></span>

<span data-ttu-id="7eb2a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb2a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7eb2a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7eb2a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7eb2a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb2a-132">Request</span></span>

<span data-ttu-id="7eb2a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7eb2a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```

### <a name="response"></a><span data-ttu-id="7eb2a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb2a-134">Response</span></span>

<span data-ttu-id="7eb2a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb2a-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
