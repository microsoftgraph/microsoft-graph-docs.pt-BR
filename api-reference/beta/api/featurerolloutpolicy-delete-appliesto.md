---
title: Remover aplica-se
description: Remover um directoryobject da distribuição de recursos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56738d8d2059b4324f287f34d08e9b7a11d5567f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421771"
---
# <a name="remove-appliesto"></a><span data-ttu-id="057d0-103">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="057d0-103">Remove appliesTo</span></span>

<span data-ttu-id="057d0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="057d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="057d0-105">Remova um aplicato em um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para remover o [directoryobject](../resources/directoryobject.md) da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="057d0-105">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="057d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="057d0-106">Permissions</span></span>

<span data-ttu-id="057d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="057d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="057d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="057d0-109">Permission type</span></span>                        | <span data-ttu-id="057d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="057d0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="057d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="057d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="057d0-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="057d0-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="057d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="057d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="057d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="057d0-114">Not supported.</span></span> |
| <span data-ttu-id="057d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="057d0-115">Application</span></span>                            | <span data-ttu-id="057d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="057d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="057d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="057d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="057d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="057d0-118">Request headers</span></span>

| <span data-ttu-id="057d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="057d0-119">Name</span></span>          | <span data-ttu-id="057d0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="057d0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="057d0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="057d0-121">Authorization</span></span> | <span data-ttu-id="057d0-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="057d0-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="057d0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="057d0-123">Request body</span></span>

<span data-ttu-id="057d0-124">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="057d0-124">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="057d0-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="057d0-125">Response</span></span>

<span data-ttu-id="057d0-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="057d0-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="057d0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="057d0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="057d0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="057d0-129">Request</span></span>

<span data-ttu-id="057d0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="057d0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="057d0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="057d0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="c"></a>[<span data-ttu-id="057d0-132">C#</span><span class="sxs-lookup"><span data-stu-id="057d0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="057d0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="057d0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="057d0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="057d0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="057d0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="057d0-135">Response</span></span>

<span data-ttu-id="057d0-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="057d0-136">The following is an example of the response.</span></span>

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
