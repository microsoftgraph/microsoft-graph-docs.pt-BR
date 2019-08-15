---
title: Remover aplica-se
description: Remover um directoryobject da distribuição de recursos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 020dd8bcd01e78cfe194df148cb57a3307dbe6ed
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419794"
---
# <a name="remove-appliesto"></a><span data-ttu-id="35e37-103">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="35e37-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35e37-104">Remova um aplicato em um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para remover o [directoryobject](../resources/directoryobject.md) da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="35e37-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="35e37-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="35e37-105">Permissions</span></span>

<span data-ttu-id="35e37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35e37-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35e37-108">Permission type</span></span>                        | <span data-ttu-id="35e37-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35e37-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="35e37-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35e37-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="35e37-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="35e37-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="35e37-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35e37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35e37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35e37-113">Not supported.</span></span> |
| <span data-ttu-id="35e37-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35e37-114">Application</span></span>                            | <span data-ttu-id="35e37-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35e37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35e37-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35e37-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="35e37-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35e37-117">Request headers</span></span>

| <span data-ttu-id="35e37-118">Nome</span><span class="sxs-lookup"><span data-stu-id="35e37-118">Name</span></span>          | <span data-ttu-id="35e37-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="35e37-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="35e37-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="35e37-120">Authorization</span></span> | <span data-ttu-id="35e37-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="35e37-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="35e37-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35e37-122">Request body</span></span>

<span data-ttu-id="35e37-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/directoryobject.md) objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="35e37-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="35e37-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="35e37-124">Response</span></span>

<span data-ttu-id="35e37-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35e37-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35e37-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="35e37-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35e37-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35e37-128">Request</span></span>

<span data-ttu-id="35e37-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35e37-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35e37-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="35e37-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35e37-131">C#</span><span class="sxs-lookup"><span data-stu-id="35e37-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35e37-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35e37-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35e37-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="35e37-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35e37-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="35e37-134">Response</span></span>

<span data-ttu-id="35e37-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35e37-135">The following is an example of the response.</span></span>

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
