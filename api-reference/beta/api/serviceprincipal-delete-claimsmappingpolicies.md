---
title: Remover claimsMappingPolicy
description: Remover um claimsMappingPolicy de um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 077476c07e5df3804b67ff7b8974f79e715551bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453503"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="c40e8-103">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="c40e8-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="c40e8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c40e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c40e8-105">Remover um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c40e8-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c40e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c40e8-106">Permissions</span></span>

<span data-ttu-id="c40e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c40e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c40e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c40e8-109">Permission type</span></span>                        | <span data-ttu-id="c40e8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c40e8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c40e8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c40e8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c40e8-112">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c40e8-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c40e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c40e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c40e8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c40e8-114">Not supported.</span></span> |
| <span data-ttu-id="c40e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c40e8-115">Application</span></span>                            | <span data-ttu-id="c40e8-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c40e8-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c40e8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c40e8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="c40e8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c40e8-118">Request headers</span></span>

| <span data-ttu-id="c40e8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c40e8-119">Name</span></span>          | <span data-ttu-id="c40e8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c40e8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c40e8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c40e8-121">Authorization</span></span> | <span data-ttu-id="c40e8-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c40e8-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c40e8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c40e8-123">Request body</span></span>

<span data-ttu-id="c40e8-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c40e8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c40e8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c40e8-125">Response</span></span>

<span data-ttu-id="c40e8-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c40e8-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c40e8-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c40e8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c40e8-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c40e8-128">Request</span></span>

<span data-ttu-id="c40e8-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c40e8-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="c40e8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c40e8-130">Response</span></span>

<span data-ttu-id="c40e8-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c40e8-131">The following is an example of the response.</span></span>

> <span data-ttu-id="c40e8-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c40e8-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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