---
title: Excluir claimsMappingPolicy
description: Exclua claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4d9a94261d0c4a308eb03c532b954bf18150550
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846214"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="fc3c3-103">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="fc3c3-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="fc3c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc3c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc3c3-105">Excluir um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fc3c3-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc3c3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc3c3-106">Permissions</span></span>

<span data-ttu-id="fc3c3-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fc3c3-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fc3c3-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc3c3-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc3c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc3c3-109">Permission type</span></span>                        | <span data-ttu-id="fc3c3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc3c3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc3c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc3c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc3c3-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc3c3-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="fc3c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc3c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc3c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc3c3-114">Not supported.</span></span> |
| <span data-ttu-id="fc3c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc3c3-115">Application</span></span>                            | <span data-ttu-id="fc3c3-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc3c3-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc3c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3c3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fc3c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3c3-118">Request headers</span></span>

| <span data-ttu-id="fc3c3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc3c3-119">Name</span></span>          | <span data-ttu-id="fc3c3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc3c3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fc3c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc3c3-121">Authorization</span></span> | <span data-ttu-id="fc3c3-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="fc3c3-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc3c3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3c3-123">Request body</span></span>

<span data-ttu-id="fc3c3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc3c3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc3c3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3c3-125">Response</span></span>

<span data-ttu-id="fc3c3-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fc3c3-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fc3c3-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc3c3-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc3c3-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc3c3-128">Request</span></span>

<span data-ttu-id="fc3c3-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc3c3-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc3c3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3c3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="fc3c3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc3c3-131">Response</span></span>

<span data-ttu-id="fc3c3-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc3c3-132">The following is an example of the response.</span></span>

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
  "description": "Delete claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
