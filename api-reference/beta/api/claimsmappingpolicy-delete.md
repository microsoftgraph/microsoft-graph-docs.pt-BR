---
title: Excluir claimsMappingPolicy
description: Exclua claimsMappingPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b60c3cc3b49fb486c31d36030b6722347f90f75a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234082"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="639d8-103">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="639d8-103">Delete claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="639d8-104">Excluir um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="639d8-104">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="639d8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="639d8-105">Permissions</span></span>

<span data-ttu-id="639d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="639d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="639d8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="639d8-108">Permission type</span></span>                        | <span data-ttu-id="639d8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="639d8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="639d8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="639d8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="639d8-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="639d8-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="639d8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="639d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="639d8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="639d8-113">Not supported.</span></span> |
| <span data-ttu-id="639d8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="639d8-114">Application</span></span>                            | <span data-ttu-id="639d8-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="639d8-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="639d8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="639d8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="639d8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="639d8-117">Request headers</span></span>

| <span data-ttu-id="639d8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="639d8-118">Name</span></span>          | <span data-ttu-id="639d8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="639d8-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="639d8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="639d8-120">Authorization</span></span> | <span data-ttu-id="639d8-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="639d8-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="639d8-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="639d8-122">Request body</span></span>

<span data-ttu-id="639d8-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="639d8-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="639d8-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="639d8-124">Response</span></span>

<span data-ttu-id="639d8-125">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="639d8-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="639d8-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="639d8-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="639d8-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="639d8-127">Request</span></span>

<span data-ttu-id="639d8-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="639d8-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="639d8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="639d8-129">Response</span></span>

<span data-ttu-id="639d8-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="639d8-130">The following is an example of the response.</span></span>

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