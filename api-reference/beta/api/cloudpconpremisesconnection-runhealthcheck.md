---
title: CloudPcOnPremisesConnection-RunHealthChecks
description: Executar verificações de integridade na conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 949d9d01d7706f878b19702f811b4838f4e6bfe8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563287"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="e1d77-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="e1d77-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="e1d77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1d77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d77-105">Executar verificações de integridade no objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="e1d77-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="e1d77-106">Isso disparará uma nova verificação de integridade para este objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) e alterará as propriedades HealthCheckStatus e [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) quando o check for concluído.</span><span class="sxs-lookup"><span data-stu-id="e1d77-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="e1d77-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e1d77-107">Permissions</span></span>

<span data-ttu-id="e1d77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1d77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1d77-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1d77-110">Permission type</span></span>|<span data-ttu-id="e1d77-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1d77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1d77-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1d77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1d77-113">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1d77-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="e1d77-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1d77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1d77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1d77-115">Not supported.</span></span>|
|<span data-ttu-id="e1d77-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1d77-116">Application</span></span>|<span data-ttu-id="e1d77-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1d77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1d77-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1d77-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="e1d77-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1d77-119">Request headers</span></span>

|<span data-ttu-id="e1d77-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e1d77-120">Name</span></span>|<span data-ttu-id="e1d77-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1d77-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e1d77-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1d77-122">Authorization</span></span>|<span data-ttu-id="e1d77-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1d77-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1d77-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1d77-125">Request body</span></span>

<span data-ttu-id="e1d77-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1d77-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1d77-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1d77-127">Response</span></span>

<span data-ttu-id="e1d77-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e1d77-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e1d77-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e1d77-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1d77-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1d77-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e1d77-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1d77-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```
# <a name="c"></a>[<span data-ttu-id="e1d77-132">C#</span><span class="sxs-lookup"><span data-stu-id="e1d77-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1d77-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1d77-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1d77-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1d77-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1d77-135">Java</span><span class="sxs-lookup"><span data-stu-id="e1d77-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1d77-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1d77-136">Response</span></span>

<span data-ttu-id="e1d77-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e1d77-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
