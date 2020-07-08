---
title: Remover tokenIssuancePolicy
description: Remover um tokenIssuancePolicy de um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5f795000414ebecfbb002b96feb490207b44a94
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081271"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="8edb3-103">Remover tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="8edb3-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="8edb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8edb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8edb3-105">Remover um [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="8edb3-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8edb3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8edb3-106">Permissions</span></span>

<span data-ttu-id="8edb3-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8edb3-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8edb3-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edb3-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8edb3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8edb3-109">Permission type</span></span>                        | <span data-ttu-id="8edb3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8edb3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8edb3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8edb3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8edb3-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8edb3-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="8edb3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8edb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8edb3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8edb3-114">Not supported.</span></span> |
| <span data-ttu-id="8edb3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8edb3-115">Application</span></span>                            | <span data-ttu-id="8edb3-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8edb3-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8edb3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8edb3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8edb3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8edb3-118">Request headers</span></span>

| <span data-ttu-id="8edb3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8edb3-119">Name</span></span>          | <span data-ttu-id="8edb3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8edb3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8edb3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8edb3-121">Authorization</span></span> | <span data-ttu-id="8edb3-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8edb3-122">Bearer {token}.</span></span> <span data-ttu-id="8edb3-123">Required.</span><span class="sxs-lookup"><span data-stu-id="8edb3-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8edb3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8edb3-124">Request body</span></span>

<span data-ttu-id="8edb3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8edb3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8edb3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edb3-126">Response</span></span>

<span data-ttu-id="8edb3-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8edb3-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8edb3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8edb3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8edb3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8edb3-129">Request</span></span>

<span data-ttu-id="8edb3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8edb3-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8edb3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8edb3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="8edb3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edb3-132">Response</span></span>

<span data-ttu-id="8edb3-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8edb3-133">The following is an example of the response.</span></span>

> <span data-ttu-id="8edb3-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="8edb3-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8edb3-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8edb3-135">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
