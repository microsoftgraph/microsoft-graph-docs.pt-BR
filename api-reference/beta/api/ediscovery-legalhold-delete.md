---
title: Excluir legalHold
description: Exclua um objeto legalHold.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 90a7600f972a08220579dec56b1e0f738459c283
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445791"
---
# <a name="delete-legalhold"></a><span data-ttu-id="f2dd7-103">Excluir legalHold</span><span class="sxs-lookup"><span data-stu-id="f2dd7-103">Delete legalHold</span></span>

<span data-ttu-id="f2dd7-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f2dd7-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2dd7-105">[Exclua um objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="f2dd7-105">Delete a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2dd7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2dd7-106">Permissions</span></span>

<span data-ttu-id="f2dd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2dd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2dd7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2dd7-109">Permission type</span></span>|<span data-ttu-id="f2dd7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2dd7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2dd7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2dd7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2dd7-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2dd7-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f2dd7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2dd7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2dd7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2dd7-114">Not supported.</span></span>|
|<span data-ttu-id="f2dd7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2dd7-115">Application</span></span>|<span data-ttu-id="f2dd7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2dd7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2dd7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2dd7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/legalHolds/{legalHoldId}
```

## <a name="request-headers"></a><span data-ttu-id="f2dd7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dd7-118">Request headers</span></span>

|<span data-ttu-id="f2dd7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f2dd7-119">Name</span></span>|<span data-ttu-id="f2dd7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dd7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2dd7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2dd7-121">Authorization</span></span>|<span data-ttu-id="f2dd7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2dd7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2dd7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dd7-124">Request body</span></span>

<span data-ttu-id="f2dd7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2dd7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2dd7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2dd7-126">Response</span></span>

<span data-ttu-id="f2dd7-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2dd7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2dd7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2dd7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2dd7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dd7-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_legalhold"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

### <a name="response"></a><span data-ttu-id="f2dd7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2dd7-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
