---
title: 'CloudPcOnPremisesConnection: runHealthChecks'
description: Execute verificações de saúde na conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: da78bd5117f8795b7fc26c3be0d45d24d83e0acc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947594"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="45a1b-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="45a1b-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="45a1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45a1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a1b-105">Execute verificações de saúde no [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="45a1b-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="45a1b-106">Isso disparará uma nova verificação de saúde para este objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) e alterará as propriedades healthCheckStatus e [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) quando a verificação for concluída.</span><span class="sxs-lookup"><span data-stu-id="45a1b-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="45a1b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="45a1b-107">Permissions</span></span>

<span data-ttu-id="45a1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45a1b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45a1b-110">Permission type</span></span>|<span data-ttu-id="45a1b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45a1b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a1b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45a1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45a1b-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a1b-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="45a1b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45a1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a1b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a1b-115">Not supported.</span></span>|
|<span data-ttu-id="45a1b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45a1b-116">Application</span></span>|<span data-ttu-id="45a1b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a1b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a1b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="45a1b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a1b-119">Request headers</span></span>

|<span data-ttu-id="45a1b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="45a1b-120">Name</span></span>|<span data-ttu-id="45a1b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a1b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45a1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a1b-122">Authorization</span></span>|<span data-ttu-id="45a1b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a1b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45a1b-125">Request body</span></span>

<span data-ttu-id="45a1b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45a1b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45a1b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a1b-127">Response</span></span>

<span data-ttu-id="45a1b-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45a1b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="45a1b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45a1b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45a1b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a1b-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="45a1b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="45a1b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck_2"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="45a1b-132">C#</span><span class="sxs-lookup"><span data-stu-id="45a1b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45a1b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45a1b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45a1b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45a1b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45a1b-135">Java</span><span class="sxs-lookup"><span data-stu-id="45a1b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45a1b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a1b-136">Response</span></span>

<span data-ttu-id="45a1b-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="45a1b-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
