---
title: Excluir permissionGrantPolicy
description: Excluir um objeto permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 5c977da45c2e640e041dc37c8be2fb17c49a8424
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377168"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="55c65-103">Excluir permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="55c65-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="55c65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55c65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55c65-105">Excluir um objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="55c65-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55c65-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="55c65-106">Permissions</span></span>

<span data-ttu-id="55c65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55c65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55c65-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55c65-109">Permission type</span></span>                        | <span data-ttu-id="55c65-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55c65-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55c65-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55c65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55c65-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="55c65-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="55c65-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55c65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55c65-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55c65-114">Not supported.</span></span> |
| <span data-ttu-id="55c65-115">Application</span><span class="sxs-lookup"><span data-stu-id="55c65-115">Application</span></span>                            | <span data-ttu-id="55c65-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="55c65-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="55c65-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55c65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55c65-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55c65-118">Request headers</span></span>

| <span data-ttu-id="55c65-119">Nome</span><span class="sxs-lookup"><span data-stu-id="55c65-119">Name</span></span>           | <span data-ttu-id="55c65-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c65-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="55c65-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55c65-121">Authorization</span></span>  | <span data-ttu-id="55c65-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55c65-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55c65-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55c65-124">Request body</span></span>

<span data-ttu-id="55c65-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55c65-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55c65-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="55c65-126">Response</span></span>

<span data-ttu-id="55c65-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55c65-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55c65-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55c65-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55c65-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55c65-130">Request</span></span>

<span data-ttu-id="55c65-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55c65-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
```

### <a name="response"></a><span data-ttu-id="55c65-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="55c65-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
