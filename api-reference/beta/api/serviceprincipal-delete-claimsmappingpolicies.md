---
title: Remover claimsMappingPolicy
description: Remover um claimsMappingPolicy de um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b653ff06950fcba1851afffa7d09fb5d3296d3bf
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234111"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="f8ee9-103">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="f8ee9-103">Remove claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8ee9-104">Remover um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="f8ee9-104">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8ee9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8ee9-105">Permissions</span></span>

<span data-ttu-id="f8ee9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8ee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8ee9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8ee9-108">Permission type</span></span>                        | <span data-ttu-id="f8ee9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8ee9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8ee9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8ee9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8ee9-111">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8ee9-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="f8ee9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8ee9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8ee9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-113">Not supported.</span></span> |
| <span data-ttu-id="f8ee9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8ee9-114">Application</span></span>                            | <span data-ttu-id="f8ee9-115">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8ee9-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8ee9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8ee9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="f8ee9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8ee9-117">Request headers</span></span>

| <span data-ttu-id="f8ee9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f8ee9-118">Name</span></span>          | <span data-ttu-id="f8ee9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8ee9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f8ee9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8ee9-120">Authorization</span></span> | <span data-ttu-id="f8ee9-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f8ee9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8ee9-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8ee9-122">Request body</span></span>

<span data-ttu-id="f8ee9-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8ee9-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8ee9-124">Response</span></span>

<span data-ttu-id="f8ee9-125">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-125">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f8ee9-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8ee9-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8ee9-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8ee9-127">Request</span></span>

<span data-ttu-id="f8ee9-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="f8ee9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8ee9-129">Response</span></span>

<span data-ttu-id="f8ee9-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-130">The following is an example of the response.</span></span>

> <span data-ttu-id="f8ee9-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->