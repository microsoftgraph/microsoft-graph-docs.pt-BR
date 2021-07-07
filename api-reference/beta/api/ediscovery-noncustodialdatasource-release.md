---
title: 'noncustodialDataSource: release'
description: Libera a fonte de dados não custodiada do caso.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 190845ea64a545b29c2de60028ca22746ba8b91f
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316955"
---
# <a name="noncustodialdatasource-release"></a><span data-ttu-id="30636-103">noncustodialDataSource: release</span><span class="sxs-lookup"><span data-stu-id="30636-103">noncustodialDataSource: release</span></span>

<span data-ttu-id="30636-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="30636-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30636-105">Libera a fonte de dados não custodiada do caso.</span><span class="sxs-lookup"><span data-stu-id="30636-105">Releases the non-custodial data source from the case.</span></span>

## <a name="permissions"></a><span data-ttu-id="30636-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="30636-106">Permissions</span></span>

<span data-ttu-id="30636-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30636-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30636-109">Permission type</span></span>|<span data-ttu-id="30636-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30636-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30636-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30636-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30636-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30636-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="30636-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30636-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30636-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30636-114">Not supported.</span></span>|
|<span data-ttu-id="30636-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30636-115">Application</span></span>|<span data-ttu-id="30636-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30636-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30636-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30636-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/release
```

## <a name="request-headers"></a><span data-ttu-id="30636-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30636-118">Request headers</span></span>

|<span data-ttu-id="30636-119">Nome</span><span class="sxs-lookup"><span data-stu-id="30636-119">Name</span></span>|<span data-ttu-id="30636-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="30636-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="30636-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="30636-121">Authorization</span></span>|<span data-ttu-id="30636-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30636-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30636-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30636-124">Request body</span></span>

<span data-ttu-id="30636-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30636-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30636-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="30636-126">Response</span></span>

<span data-ttu-id="30636-127">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="30636-127">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="30636-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30636-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30636-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30636-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="30636-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="30636-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "noncustodialdatasource_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/release
```
# <a name="c"></a>[<span data-ttu-id="30636-131">C#</span><span class="sxs-lookup"><span data-stu-id="30636-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/noncustodialdatasource-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30636-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30636-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/noncustodialdatasource-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30636-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30636-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/noncustodialdatasource-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30636-134">Java</span><span class="sxs-lookup"><span data-stu-id="30636-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/noncustodialdatasource-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30636-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="30636-135">Response</span></span>

<span data-ttu-id="30636-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="30636-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
