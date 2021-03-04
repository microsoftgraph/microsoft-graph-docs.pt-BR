---
title: Excluir sourceCollection
description: Exclua um objeto sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 38debc57e715b735e56be154f57bbef8861cae05
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445759"
---
# <a name="delete-sourcecollection"></a><span data-ttu-id="e322b-103">Excluir sourceCollection</span><span class="sxs-lookup"><span data-stu-id="e322b-103">Delete sourceCollection</span></span>

<span data-ttu-id="e322b-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e322b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e322b-105">Exclua [um objeto sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="e322b-105">Delete a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e322b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e322b-106">Permissions</span></span>

<span data-ttu-id="e322b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e322b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e322b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e322b-109">Permission type</span></span>|<span data-ttu-id="e322b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e322b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e322b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e322b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e322b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e322b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e322b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e322b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e322b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e322b-114">Not supported.</span></span>|
|<span data-ttu-id="e322b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e322b-115">Application</span></span>|<span data-ttu-id="e322b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e322b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e322b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e322b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="e322b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e322b-118">Request headers</span></span>

|<span data-ttu-id="e322b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e322b-119">Name</span></span>|<span data-ttu-id="e322b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e322b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e322b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e322b-121">Authorization</span></span>|<span data-ttu-id="e322b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e322b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e322b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e322b-124">Request body</span></span>

<span data-ttu-id="e322b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e322b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e322b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e322b-126">Response</span></span>

<span data-ttu-id="e322b-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e322b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e322b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e322b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e322b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e322b-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_sourcecollection"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

### <a name="response"></a><span data-ttu-id="e322b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e322b-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
