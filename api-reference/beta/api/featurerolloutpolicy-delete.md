---
title: Excluir featureRolloutPolicy
description: Excluir um objeto featureRolloutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: defcc190f67dc7a78a0069445401e6f624a9a878
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419738"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="25cc0-103">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="25cc0-103">Delete featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25cc0-104">Excluir um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="25cc0-104">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25cc0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="25cc0-105">Permissions</span></span>

<span data-ttu-id="25cc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25cc0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25cc0-108">Permission type</span></span>                        | <span data-ttu-id="25cc0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25cc0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25cc0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25cc0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="25cc0-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="25cc0-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="25cc0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25cc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25cc0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25cc0-113">Not supported.</span></span> |
| <span data-ttu-id="25cc0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25cc0-114">Application</span></span>                            | <span data-ttu-id="25cc0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25cc0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25cc0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25cc0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="25cc0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25cc0-117">Request headers</span></span>

| <span data-ttu-id="25cc0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="25cc0-118">Name</span></span>          | <span data-ttu-id="25cc0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="25cc0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="25cc0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="25cc0-120">Authorization</span></span> | <span data-ttu-id="25cc0-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="25cc0-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="25cc0-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25cc0-122">Request body</span></span>

<span data-ttu-id="25cc0-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25cc0-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25cc0-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cc0-124">Response</span></span>

<span data-ttu-id="25cc0-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25cc0-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25cc0-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="25cc0-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25cc0-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cc0-128">Request</span></span>

<span data-ttu-id="25cc0-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25cc0-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="25cc0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cc0-130">Response</span></span>

<span data-ttu-id="25cc0-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25cc0-131">The following is an example of the response.</span></span>

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
