---
title: Excluir permissionGrantConditionSet da coleção de inclusões de permissionGrantPolicy
description: Exclui um conjunto de condições incluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ca7a37c0cbcb67aa2bf8fc961c8f3211a85a4256
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377114"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="9b60d-103">Excluir permissionGrantConditionSet da coleção de inclusões de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="9b60d-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="9b60d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b60d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b60d-105">Exclui um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção de **inclusões** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9b60d-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b60d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9b60d-106">Permissions</span></span>

<span data-ttu-id="9b60d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b60d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b60d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b60d-109">Permission type</span></span>      | <span data-ttu-id="9b60d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b60d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="9b60d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b60d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b60d-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9b60d-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="9b60d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b60d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b60d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b60d-114">Not supported.</span></span>    |
| <span data-ttu-id="9b60d-115">Application</span><span class="sxs-lookup"><span data-stu-id="9b60d-115">Application</span></span> | <span data-ttu-id="9b60d-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9b60d-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b60d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b60d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="9b60d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b60d-118">Request headers</span></span>

| <span data-ttu-id="9b60d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9b60d-119">Name</span></span>       | <span data-ttu-id="9b60d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b60d-120">Type</span></span> | <span data-ttu-id="9b60d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b60d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b60d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b60d-122">Authorization</span></span>  | <span data-ttu-id="9b60d-123">string</span><span class="sxs-lookup"><span data-stu-id="9b60d-123">string</span></span>  | <span data-ttu-id="9b60d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b60d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b60d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b60d-126">Request body</span></span>

<span data-ttu-id="9b60d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b60d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b60d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b60d-128">Response</span></span>

<span data-ttu-id="9b60d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b60d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b60d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b60d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b60d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b60d-132">Request</span></span>

<span data-ttu-id="9b60d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b60d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```

### <a name="response"></a><span data-ttu-id="9b60d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b60d-134">Response</span></span>

<span data-ttu-id="9b60d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b60d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
