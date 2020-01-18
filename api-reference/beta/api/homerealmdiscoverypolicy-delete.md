---
title: Excluir homeRealmDiscoveryPolicy
description: Exclua homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc54623f6b30226adc493511c1dc8413b5e96421
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234093"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="242bf-103">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="242bf-103">Delete homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="242bf-104">Excluir um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="242bf-104">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="242bf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="242bf-105">Permissions</span></span>

<span data-ttu-id="242bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="242bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="242bf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="242bf-108">Permission type</span></span>                        | <span data-ttu-id="242bf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="242bf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="242bf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="242bf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="242bf-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="242bf-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="242bf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="242bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="242bf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="242bf-113">Not supported.</span></span> |
| <span data-ttu-id="242bf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="242bf-114">Application</span></span>                            | <span data-ttu-id="242bf-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="242bf-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="242bf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="242bf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="242bf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="242bf-117">Request headers</span></span>

| <span data-ttu-id="242bf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="242bf-118">Name</span></span>          | <span data-ttu-id="242bf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="242bf-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="242bf-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="242bf-120">Authorization</span></span> | <span data-ttu-id="242bf-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="242bf-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="242bf-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="242bf-122">Request body</span></span>

<span data-ttu-id="242bf-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="242bf-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="242bf-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="242bf-124">Response</span></span>

<span data-ttu-id="242bf-125">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="242bf-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="242bf-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="242bf-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="242bf-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="242bf-127">Request</span></span>

<span data-ttu-id="242bf-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="242bf-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="242bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="242bf-129">Response</span></span>

<span data-ttu-id="242bf-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="242bf-130">The following is an example of the response.</span></span>

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
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->