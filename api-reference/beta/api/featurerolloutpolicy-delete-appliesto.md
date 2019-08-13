---
title: Remover aplica-se
description: Remover um directoryobject da distribuição de recursos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9d1c6046ab108313cf040293e66209f4492f45
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325250"
---
# <a name="remove-appliesto"></a><span data-ttu-id="a3975-103">Remover aplica-se</span><span class="sxs-lookup"><span data-stu-id="a3975-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3975-104">Remova um aplicato em um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para remover o [directoryobject](../resources/directoryobject.md) da distribuição de recursos.</span><span class="sxs-lookup"><span data-stu-id="a3975-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3975-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3975-105">Permissions</span></span>

<span data-ttu-id="a3975-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3975-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3975-108">Permission type</span></span>                        | <span data-ttu-id="a3975-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3975-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a3975-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3975-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3975-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="a3975-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="a3975-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3975-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3975-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3975-113">Not supported.</span></span> |
| <span data-ttu-id="a3975-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3975-114">Application</span></span>                            | <span data-ttu-id="a3975-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3975-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3975-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3975-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a3975-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3975-117">Request headers</span></span>

| <span data-ttu-id="a3975-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a3975-118">Name</span></span>          | <span data-ttu-id="a3975-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3975-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a3975-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3975-120">Authorization</span></span> | <span data-ttu-id="a3975-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a3975-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3975-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3975-122">Request body</span></span>

<span data-ttu-id="a3975-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/directoryobject.md) objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="a3975-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a3975-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3975-124">Response</span></span>

<span data-ttu-id="a3975-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3975-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3975-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a3975-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3975-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3975-128">Request</span></span>

<span data-ttu-id="a3975-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3975-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3975-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3975-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3975-131">C#</span><span class="sxs-lookup"><span data-stu-id="a3975-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3975-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3975-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3975-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3975-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3975-134">Java</span><span class="sxs-lookup"><span data-stu-id="a3975-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3975-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3975-135">Response</span></span>

<span data-ttu-id="a3975-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3975-136">The following is an example of the response.</span></span>

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
