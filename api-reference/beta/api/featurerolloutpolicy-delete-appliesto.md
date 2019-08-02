---
title: Remover aplica-se
description: Remover um directoryobject da distribuição de recursos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1247cc352103bce040dc994feccd23ab9ba5a1bc
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062087"
---
# <a name="remove-appliesto"></a><span data-ttu-id="7746d-103">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="7746d-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7746d-104">Remova um aplicato em um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para remover o [directoryobject](../resources/directoryobject.md) da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="7746d-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="7746d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7746d-105">Permissions</span></span>

<span data-ttu-id="7746d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7746d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7746d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7746d-108">Permission type</span></span>                        | <span data-ttu-id="7746d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7746d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7746d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7746d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7746d-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="7746d-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="7746d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7746d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7746d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7746d-113">Not supported.</span></span> |
| <span data-ttu-id="7746d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7746d-114">Application</span></span>                            | <span data-ttu-id="7746d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7746d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7746d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7746d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7746d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7746d-117">Request headers</span></span>

| <span data-ttu-id="7746d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7746d-118">Name</span></span>          | <span data-ttu-id="7746d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7746d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7746d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7746d-120">Authorization</span></span> | <span data-ttu-id="7746d-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7746d-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7746d-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7746d-122">Request body</span></span>

<span data-ttu-id="7746d-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/directoryobject.md) objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="7746d-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7746d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7746d-124">Response</span></span>

<span data-ttu-id="7746d-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7746d-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7746d-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7746d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7746d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7746d-128">Request</span></span>

<span data-ttu-id="7746d-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7746d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```

### <a name="response"></a><span data-ttu-id="7746d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7746d-130">Response</span></span>

<span data-ttu-id="7746d-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7746d-131">The following is an example of the response.</span></span>

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