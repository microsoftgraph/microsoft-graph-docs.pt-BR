---
title: Remover appliesTo
description: Remover um directoryObject da adoção de recursos.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 04327bd52f34de054bbb5451ed4c53a3695afa34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955942"
---
# <a name="remove-appliesto"></a><span data-ttu-id="837fd-103">Remover appliesTo</span><span class="sxs-lookup"><span data-stu-id="837fd-103">Remove appliesTo</span></span>

<span data-ttu-id="837fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="837fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="837fd-105">Remova um appliesTo em um [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) para remover [o directoryObject](../resources/directoryobject.md) da rolagem de recursos.</span><span class="sxs-lookup"><span data-stu-id="837fd-105">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="837fd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="837fd-106">Permissions</span></span>

<span data-ttu-id="837fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="837fd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="837fd-109">Permission type</span></span>                        | <span data-ttu-id="837fd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="837fd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="837fd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="837fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="837fd-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837fd-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="837fd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="837fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="837fd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="837fd-114">Not supported.</span></span> |
| <span data-ttu-id="837fd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="837fd-115">Application</span></span>                            | <span data-ttu-id="837fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="837fd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="837fd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="837fd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{policyId}/appliesTo/{directoryObjectId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="837fd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="837fd-118">Request headers</span></span>

| <span data-ttu-id="837fd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="837fd-119">Name</span></span>          | <span data-ttu-id="837fd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="837fd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="837fd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="837fd-121">Authorization</span></span> | <span data-ttu-id="837fd-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="837fd-122">Bearer {token}.</span></span> <span data-ttu-id="837fd-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="837fd-123">Required</span></span> |

## <a name="response"></a><span data-ttu-id="837fd-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="837fd-124">Response</span></span>

<span data-ttu-id="837fd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="837fd-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="837fd-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="837fd-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="837fd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="837fd-128">Request</span></span>

<span data-ttu-id="837fd-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="837fd-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```

### <a name="response"></a><span data-ttu-id="837fd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="837fd-130">Response</span></span>

<span data-ttu-id="837fd-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="837fd-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


