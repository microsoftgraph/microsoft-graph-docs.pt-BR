---
title: Excluir marca
description: Exclua um objeto tag.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1ec395a45ee3720797228952b1f9047822fed11c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445731"
---
# <a name="delete-tag"></a><span data-ttu-id="981dd-103">Excluir marca</span><span class="sxs-lookup"><span data-stu-id="981dd-103">Delete tag</span></span>

<span data-ttu-id="981dd-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="981dd-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="981dd-105">Exclua [um objeto tag.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="981dd-105">Delete a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="981dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="981dd-106">Permissions</span></span>

<span data-ttu-id="981dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="981dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="981dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="981dd-109">Permission type</span></span>|<span data-ttu-id="981dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="981dd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="981dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="981dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="981dd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="981dd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="981dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="981dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="981dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="981dd-114">Not supported.</span></span>|
|<span data-ttu-id="981dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="981dd-115">Application</span></span>|<span data-ttu-id="981dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="981dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="981dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="981dd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/tags/{tagId}?forcedelete=true
```

## <a name="query-parameters"></a><span data-ttu-id="981dd-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="981dd-118">Query parameters</span></span>

<span data-ttu-id="981dd-119">Na URL de solicitação, forneça o seguinte parâmetro de consulta necessário.</span><span class="sxs-lookup"><span data-stu-id="981dd-119">In the request URL, provide the following required query parameter.</span></span>

| <span data-ttu-id="981dd-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="981dd-120">Parameter</span></span>     | <span data-ttu-id="981dd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="981dd-121">Type</span></span>    | <span data-ttu-id="981dd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="981dd-122">Description</span></span>                                                                              |
|:--------------|:--------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="981dd-123">forcedelete</span><span class="sxs-lookup"><span data-stu-id="981dd-123">forcedelete</span></span>   | <span data-ttu-id="981dd-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="981dd-124">Boolean</span></span> | <span data-ttu-id="981dd-125">Se definido como true, a marca e os filhos serão excluídos, se false, e a marca tiver filhos, a exclusão falhará.</span><span class="sxs-lookup"><span data-stu-id="981dd-125">If set to true, the tag and children will be deleted, if false, and the tag has children, the delete will fail.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="981dd-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="981dd-126">Request headers</span></span>

|<span data-ttu-id="981dd-127">Nome</span><span class="sxs-lookup"><span data-stu-id="981dd-127">Name</span></span>|<span data-ttu-id="981dd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="981dd-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="981dd-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="981dd-129">Authorization</span></span>|<span data-ttu-id="981dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="981dd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="981dd-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="981dd-132">Request body</span></span>

<span data-ttu-id="981dd-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="981dd-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="981dd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="981dd-134">Response</span></span>

<span data-ttu-id="981dd-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="981dd-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="981dd-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="981dd-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="981dd-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="981dd-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tag"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true
```

### <a name="response"></a><span data-ttu-id="981dd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="981dd-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
