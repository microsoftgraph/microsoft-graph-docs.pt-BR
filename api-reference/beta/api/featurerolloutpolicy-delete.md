---
title: Excluir featureRolloutPolicy
description: Exclua um objeto featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 62395dec00e5a7713ffb959f1a871eedd1da50c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471184"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="bea00-103">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bea00-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="bea00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bea00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bea00-105">[Exclua um objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bea00-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bea00-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bea00-106">Permissions</span></span>

<span data-ttu-id="bea00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bea00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bea00-109">Permission type</span></span>                        | <span data-ttu-id="bea00-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bea00-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bea00-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bea00-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bea00-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bea00-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="bea00-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bea00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bea00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bea00-114">Not supported.</span></span> |
| <span data-ttu-id="bea00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bea00-115">Application</span></span>                            | <span data-ttu-id="bea00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bea00-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bea00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bea00-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bea00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bea00-118">Request headers</span></span>

| <span data-ttu-id="bea00-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bea00-119">Name</span></span>          | <span data-ttu-id="bea00-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bea00-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bea00-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bea00-121">Authorization</span></span> | <span data-ttu-id="bea00-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bea00-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bea00-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bea00-123">Request body</span></span>

<span data-ttu-id="bea00-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bea00-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bea00-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bea00-125">Response</span></span>

<span data-ttu-id="bea00-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bea00-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bea00-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bea00-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bea00-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bea00-129">Request</span></span>

<span data-ttu-id="bea00-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bea00-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="bea00-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bea00-131">Response</span></span>

<span data-ttu-id="bea00-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bea00-132">The following is an example of the response.</span></span>

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


