---
title: Excluir delegatedPermissionClassification
description: Excluir uma classificação de permissão delegada da entidade de serviço de uma API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 53e3f249ffe909310b446687ffba720752557b63
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377116"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="a7997-103">Excluir delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="a7997-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="a7997-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7997-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a7997-105">Exclui um [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) que tinha sido definido anteriormente para uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="a7997-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7997-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a7997-106">Permissions</span></span>

<span data-ttu-id="a7997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7997-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7997-109">Permission type</span></span>      | <span data-ttu-id="a7997-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7997-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7997-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7997-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7997-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a7997-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="a7997-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7997-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7997-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7997-114">Not supported.</span></span>    |
|<span data-ttu-id="a7997-115">Application</span><span class="sxs-lookup"><span data-stu-id="a7997-115">Application</span></span> | <span data-ttu-id="a7997-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a7997-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7997-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7997-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7997-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7997-118">Request headers</span></span>

| <span data-ttu-id="a7997-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a7997-119">Name</span></span>       | <span data-ttu-id="a7997-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7997-120">Type</span></span> | <span data-ttu-id="a7997-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7997-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a7997-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7997-122">Authorization</span></span>  | <span data-ttu-id="a7997-123">string</span><span class="sxs-lookup"><span data-stu-id="a7997-123">string</span></span>  | <span data-ttu-id="a7997-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7997-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7997-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7997-126">Request body</span></span>

<span data-ttu-id="a7997-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7997-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7997-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7997-128">Response</span></span>

<span data-ttu-id="a7997-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7997-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7997-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a7997-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7997-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7997-132">Request</span></span>

<span data-ttu-id="a7997-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7997-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

### <a name="response"></a><span data-ttu-id="a7997-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7997-134">Response</span></span>

<span data-ttu-id="a7997-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7997-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
