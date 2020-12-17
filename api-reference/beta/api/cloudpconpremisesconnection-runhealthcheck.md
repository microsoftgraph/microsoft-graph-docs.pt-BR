---
title: 'CloudPcOnPremisesConnection: runHealthChecks'
description: Executar verificações de integridade na conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b207be1da6585adcabb76c8f51f048db1e159d77
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705836"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="ca72b-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="ca72b-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="ca72b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca72b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca72b-105">Executar verificações de integridade no objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="ca72b-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="ca72b-106">Isso disparará uma nova verificação de integridade para este objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) e alterará as propriedades HealthCheckStatus e [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) quando o check for concluído.</span><span class="sxs-lookup"><span data-stu-id="ca72b-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ca72b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca72b-107">Permissions</span></span>

<span data-ttu-id="ca72b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca72b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca72b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca72b-110">Permission type</span></span>|<span data-ttu-id="ca72b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca72b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca72b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca72b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca72b-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca72b-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ca72b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca72b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca72b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca72b-115">Not supported.</span></span>|
|<span data-ttu-id="ca72b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca72b-116">Application</span></span>|<span data-ttu-id="ca72b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca72b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca72b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca72b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="ca72b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca72b-119">Request headers</span></span>

|<span data-ttu-id="ca72b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ca72b-120">Name</span></span>|<span data-ttu-id="ca72b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca72b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ca72b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca72b-122">Authorization</span></span>|<span data-ttu-id="ca72b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca72b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca72b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca72b-125">Request body</span></span>

<span data-ttu-id="ca72b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca72b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca72b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca72b-127">Response</span></span>

<span data-ttu-id="ca72b-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ca72b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ca72b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca72b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca72b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca72b-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ca72b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca72b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="ca72b-132">C#</span><span class="sxs-lookup"><span data-stu-id="ca72b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca72b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca72b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca72b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca72b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca72b-135">Java</span><span class="sxs-lookup"><span data-stu-id="ca72b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca72b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca72b-136">Response</span></span>

<span data-ttu-id="ca72b-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca72b-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
