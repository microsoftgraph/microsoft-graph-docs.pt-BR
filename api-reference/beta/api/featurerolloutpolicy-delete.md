---
title: Excluir featureRolloutPolicy
description: Excluir um objeto featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 078af77e9b3cffa63e7a86b22aec49c7d98b3dee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006759"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="7ddd1-103">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7ddd1-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="7ddd1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ddd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ddd1-105">Excluir um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7ddd1-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ddd1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ddd1-106">Permissions</span></span>

<span data-ttu-id="7ddd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ddd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ddd1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ddd1-109">Permission type</span></span>                        | <span data-ttu-id="7ddd1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ddd1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ddd1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ddd1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ddd1-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="7ddd1-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="7ddd1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ddd1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ddd1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ddd1-114">Not supported.</span></span> |
| <span data-ttu-id="7ddd1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ddd1-115">Application</span></span>                            | <span data-ttu-id="7ddd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ddd1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ddd1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ddd1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ddd1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddd1-118">Request headers</span></span>

| <span data-ttu-id="7ddd1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7ddd1-119">Name</span></span>          | <span data-ttu-id="7ddd1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ddd1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7ddd1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ddd1-121">Authorization</span></span> | <span data-ttu-id="7ddd1-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7ddd1-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ddd1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddd1-123">Request body</span></span>

<span data-ttu-id="7ddd1-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ddd1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ddd1-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ddd1-125">Response</span></span>

<span data-ttu-id="7ddd1-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ddd1-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ddd1-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7ddd1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ddd1-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddd1-129">Request</span></span>

<span data-ttu-id="7ddd1-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ddd1-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="7ddd1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ddd1-131">Response</span></span>

<span data-ttu-id="7ddd1-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ddd1-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


