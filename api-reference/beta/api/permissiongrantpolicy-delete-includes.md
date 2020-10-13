---
title: Excluir permissionGrantConditionSet da coleção de inclusões de permissionGrantPolicy
description: Exclui um conjunto de condições incluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4fb9fb913698bcee6c788c3a6cbbd22eaf7db6c5
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433510"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="85d5e-103">Excluir permissionGrantConditionSet da coleção de inclusões de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="85d5e-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="85d5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85d5e-105">Exclui um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção de **inclusões** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="85d5e-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85d5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="85d5e-106">Permissions</span></span>

<span data-ttu-id="85d5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85d5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85d5e-109">Permission type</span></span>      | <span data-ttu-id="85d5e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="85d5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="85d5e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85d5e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85d5e-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85d5e-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="85d5e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85d5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85d5e-114">Not supported.</span></span>    |
| <span data-ttu-id="85d5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85d5e-115">Application</span></span> | <span data-ttu-id="85d5e-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="85d5e-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85d5e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85d5e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="85d5e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85d5e-118">Request headers</span></span>

| <span data-ttu-id="85d5e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="85d5e-119">Name</span></span>       | <span data-ttu-id="85d5e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="85d5e-120">Type</span></span> | <span data-ttu-id="85d5e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="85d5e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85d5e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85d5e-122">Authorization</span></span>  | <span data-ttu-id="85d5e-123">string</span><span class="sxs-lookup"><span data-stu-id="85d5e-123">string</span></span>  | <span data-ttu-id="85d5e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85d5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85d5e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85d5e-126">Request body</span></span>

<span data-ttu-id="85d5e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="85d5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85d5e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d5e-128">Response</span></span>

<span data-ttu-id="85d5e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85d5e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85d5e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="85d5e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85d5e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85d5e-132">Request</span></span>

<span data-ttu-id="85d5e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="85d5e-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```

### <a name="response"></a><span data-ttu-id="85d5e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="85d5e-134">Response</span></span>

<span data-ttu-id="85d5e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="85d5e-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
