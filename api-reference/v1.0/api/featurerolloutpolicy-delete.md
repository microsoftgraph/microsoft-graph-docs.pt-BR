---
title: Excluir featureRolloutPolicy
description: Exclua um objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 351e0a78f52491118ba89b19cc8d3de44793b5c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964595"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="dc719-103">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="dc719-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="dc719-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc719-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc719-105">[Exclua um objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dc719-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc719-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc719-106">Permissions</span></span>

<span data-ttu-id="dc719-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc719-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc719-109">Permission type</span></span>                        | <span data-ttu-id="dc719-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc719-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dc719-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc719-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc719-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc719-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="dc719-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc719-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc719-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc719-114">Not supported.</span></span> |
| <span data-ttu-id="dc719-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc719-115">Application</span></span>                            | <span data-ttu-id="dc719-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc719-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc719-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc719-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc719-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc719-118">Request headers</span></span>

| <span data-ttu-id="dc719-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dc719-119">Name</span></span>          | <span data-ttu-id="dc719-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc719-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dc719-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc719-121">Authorization</span></span> | <span data-ttu-id="dc719-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="dc719-122">Bearer {token}.</span></span> <span data-ttu-id="dc719-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="dc719-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc719-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc719-124">Request body</span></span>

<span data-ttu-id="dc719-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc719-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc719-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc719-126">Response</span></span>

<span data-ttu-id="dc719-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc719-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc719-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc719-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc719-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc719-130">Request</span></span>

<span data-ttu-id="dc719-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc719-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="dc719-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc719-132">Response</span></span>

<span data-ttu-id="dc719-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc719-133">The following is an example of the response.</span></span>

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


